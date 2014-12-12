
---
title: Tutorial on McCabe and Halsted
layout: repopage
category: mccabehalsted
---


## McCabe

The McCabe metrics are a collection of four software metrics:

+ Cyclomatic complexity;
+ Essential complexity;
+ Design complexity;
+ Lines of Code (LOC).

Cyclomatic Complexity: a.k.a "v(G)", measures the number of "linearly
independent paths". A set of paths is said to be linearly independent
if no path in the set is a linear combination of any other paths
in the set through a program's "flowgraph". A flowgraph is a directed
graph where each node corresponds to a program statement, and each
arc indicates the flow of control from one statement to another.
"v(G)" is calculated by "v(G) = e - n + 2" where "G" is a program's
flowgraph, "e" is the number of arcs in the flowgraph, and "n" is
the number of nodes in the flowgraph. The standard McCabes rules
("v(G)" over 10), are used to identify fault-prone module.

Essential Complexity: a.k.a "ev(G)" is the extent to
which a flowgraph can be "reduced" by decomposing
all the subflowgraphs of "G" that are "D-structured
primes". Such "D-structured primes" are also
sometimes referred to as "proper one-entry one-exit
subflowgraphs" (for a more thorough discussion of
D-primes, see the Fenton text referenced
above). "ev(G)" is calculated using "ev(G)= v(G) -
m" where "m" is the number of subflowgraphs of "G"
that are D-structured primes.

Design Complexity: a.k.a. "iv(G)", is the cyclomatic
complexity of a module's reduced flowgraph. The
flowgraph, "G", of a module is reduced to eliminate
any complexity which does not influence the
interrelationship between design modules. According
to McCabe, this complexity measurement reflects the
modules calling patterns to its immediate
subordinate modules.

Lines of code (LOC): LOC is measured according to McCabe's line counting conventions.


## Halstead

The Halstead metrics falls into three groups:

+ the base measures,
+ the derived measures,
+ and lines of code measures.

Base measures:

+ mu1 = number of unique operators
+ mu2 = number of unique operands
+ N1 = total occurrences of operators
+ N2 = total occurrences of operands
+ length = N = N1 + N2
+ vocabulary = mu = mu1 + mu2

Constants set for each function:

+ mu1' = potential operator count (just the function name and the "return" operator)
+ mu2' = potential operand count (the number of arguments to the module)

For example, the expression "return max(w+x,x+y)" has "N1=4" operators "return, max, +,+)", "N2=4" operands (w,x,x,y), "mu1=3" unique operators (return, max,+), and "mu2=3" unique operands (w,x,y).

Derived measures:

+ P = volume = V = N x log2(mu) (the number of mental comparisons needed to write a program of length N)
+ V* = volume on minimal implementation = (2 + mu2') x log2(2 + mu2')
+ L = program length = V*/N
+ D = difficulty = 1/L
+ L' = 1/D
+ I = intelligence = L' x V'
+ E = effort to write program = V/L
+ T = time to write program = E/18 seconds

For notes on defect prediction and the relation of Halstead measures to defect predictors, please refer to our short tutorial on defect prediction here.
