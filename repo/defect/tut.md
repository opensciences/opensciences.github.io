---
title: Tutorial on Defect Prediction
layout: repo-content
category: defect
excerpt: Generating defect predictors
---


McCabe and Halstead features were defined in the 70s in an attempt to
objectively characterize code features that are associated with software
quality. The McCabe and Halstead measures are "module"-based where a
"module" is the smallest unit of functionality. In C or Smalltalk,
"modules" would be called "function" or "method" respectively.

For notes on the specifics of these metrics, see [here](ck/tut.html)
and [here](mccabehalsted/tut.html).

Defect detectors can be assessed according to the following measures:

+ accuracy = acc = (a+d)/(a+b+c+d)
+ probability of detection = pd = recall = d/(b+d)
+ probability of false alarm = pf = c/(a+c)
+ precision = prec = d/(c+d)
+ effort = amount of code selected by detector
  = (c.LOC + d.LOC)/(Total LOC)

For notes on variables a, b, c, d that are used above, see the following table:

```
                                                module actually has defects
                                               +-------------+------------+
                                               |     no      |     yes    |
                                         +-----+-------------+------------+
          classifier predicts no defects |  no |      a      |      b     |
                                         +-----+-------------+------------+
        classifier predicts some defects | yes |      c      |      d     |
                                         +-----+-------------+------------+
```

Ideally, detectors have high PDs, low PFs, and low effort. This ideal state rarely happens:

+ PD and effort are linked. The more modules that trigger the detector, the higher the PD. However, in that case the effort also increases.
+ High PD or low PF comes at the cost of high PF or low PD (respectively). This linkage can be seen in a standard receiver operator curve (ROC). Suppose, for example, LOC> x is used as the detector (i.e. we assume large modules have more errors). LOC > x represents a family of detectors. At x=0, EVERY module is predicted to have errors. This detector has a high PD but also a high false alarm rate. At x=0, NO module is predicted to have errors. This detector has a low false alarm rate but won't detect anything at all. At 0<x<1, a set of detectors are generated as shown below:

```
                 pd
               1 |           x  x  x                KEY:
                 |        x     .                   "."  denotes the line PD=PF
                 |     x      .                     "x"  denotes the roc curve 
                 |   x      .                            for a set of detectors
                 |  x     .
                 | x    . 
                 | x  .
                 |x .
                 |x
                 x------------------ pf    
                0                   1
```

Note that:

+ The only way to make no mistakes (PF=0) is to do nothing (PD=0)
+ The only way to catch more detects is to make more mistakes (increasing PD means increasing PF).
+ Our detector bends towards the "sweet spot" of <PD=1, PF=0> but does not reach it.
+ The line pf=pd on the above graph represents the "no information" line. If pf=pd then the detector is pretty useless. The better the detector, the more it rises above PF=PD towards the "sweet spot".

## Notes On McCabe & Halstead Features

McCabe argued that code with complicated pathways are more error-prone. His metrics therefore reflect the pathways within a code module. Bibtex reference for further notes is given below:

```
       @Article{mccabe76,
                title   = "A Complexity Measure",
                author  = "T.J. McCabe",
                pages   = "308--320",
                journal = "IEEE Transactions on Software Engineering",
                year    = "1976",
                volume  = "2",
                month   = "December",
                number  = "4"}
```

Halstead argued that code that is hard to read is more likely to be fault prone. Halstead estimates reading complexity by counting the number of concepts in a module; e.g. number of unique operators. Further notes on Halstead features can be found in:

```
       @Book{halstead77,
                Author    = "M.H. Halstead",
                Title     = "Elements of Software Science",
                Publisher = "Elsevier ",
                Year      = 1977}
```

McCabe and Halstead static code measures are convenient to use since they are useful, easy to use, and widely used:

+ _Useful:_ The data sets using McCabe and Halstead features can generate highly accurate predictors for defects (e.g. pc1, pc2 and other defect data sets in this website).
+ _Easy to Use:_ Static code measures (e.g. lines of code, the McCabe/Halstead measures) can be automatically and cheaply collected.
+ _Widely Used:_ Many researchers use static measures to guide software quality predictions. Verification and validation (V\&V) textbooks advise using static code complexity measures to decide which modules are worthy of manual inspections. Further, we know of several large government software contractors that won't review software modules unless tools like McCabe predict that they are fault prone. Hence, defect detectors have a major economic impact when they may force programmers to rewrite code.

Nevertheless, the merits of these metrics has been widely criticized. Static code measures are hardly a complete characterization of the internals of a function. Fenton offers an insightful example where the same functionality is achieved using different programming language constructs resulting in different static measurements for that module. Fenton uses this example to argue the uselessness of static code measures:

```
          @book{fenton97,
            author    = "N.E. Fenton and S.L. Pfleeger",
            title     = {Software metrics: a Rigorous \& Practical Approach},
            publisher = {International Thompson Press},
            year      = {1997}}
```
An alternative interpretation of Fenton's example is that static measures can never be a definite and certain indicator of the presence of a fault. Rather, defect detectors based on static measures are best viewed as probabilistic statements that the frequency of faults tends to increase in code modules that trigger the detector. By definition, such probabilistic statements are not categorical claims with some a non-zero false alarm rate. The research challenge for data miners is to ensure that these false alarms do not cripple their learned theories.
