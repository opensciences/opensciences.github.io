---
title: Related Work
layout: journal1
---


RELATED WORK: Journals and Conferences:
There are many such open access journals that allow free access to all content -- providing that that authors pay some up-front fees.
The famed Public Library of
Open Science (PLOS) publishes journals 





 

that offer open access to
all published papers, but only after authors pay 
 fees ranging from 2,250
to 2,900 USD.  

In the field of software engineering, several of our journals offer the same ``free if you pay a fee'' service.
For example, the current ``open access'' fee for the Empirical
Software Engineering Journal is 3000 USD.
What these fees pay for is a fuzzy question,
but in the case of the ACM, publication fees subsidize
the rest of the organization .
We view this as questionnable use of often publicly-funded research
output.


































Apart from charging authors to make their content open access, another issue with current open access journals 
is that, in our view, they are an incomplete response to the problem
of sharing research products.
The rhetoric for the open access journal community is 
focused primarily on the publication of ``paper'':


The manifesto of the 2001  Budapest Open Access Initiative 
focused solely on papers .

The recent  handbook ``How Open is It'' from the Public Library of Science (PLOS) group refers mostly to papers .

A  2013 survey by Soergel et al.  shows many
``open access'' conferences and journals share the text of the paper but not the ``notebooks, code  data''
used to generate those paper.

We posit that it is not enough to merely publish paper.
If a goal of science is to check, extend, apply or refute some research, then
we need to share a much wider range research products (see the list if types).
Standard forms of publishing allow for a detailed
review of the paper, but not of the research
products used to generate that paper.


















































53.4in
tabularl@ : l
Bug Prediction Dataset &http://bug.inf.usi.ch 

Eclipse Bug Data &http://goo.gl/tYKahN 

FLOSSMetrics& http://flossmetrics.org 

FLOSSMole &http://flossmole.org 

IBSBSG& http://www.isbsg.org 

ohloh& http://www.openhub.net 

PROMISE &http://promisedata.googlecode.com 

Qualitas Corpus &http://qualitascorpus.com 

Software Artifact Repository &http://sir.unl.edu 

SourceForge Research Data &http://zerlot.cse.nd.edu 

Sourcerer Project &http://sourcerer.ics.uci.edu 

Tukutuku &http://www.metriq.biz/tukutuku 

Ultimate Debian Database &http://udd.debian.org


Some repositories of software engineering data.


RELATED WORK: Open Access Repositories:
Another unique feature of our proposed infrastucture is the synergy of
repository + journal + templates.
There are many websites of SE data (see sedata). None come with an associated
 peer-reviewed discussion forum. Hence, 
it is difficult to  browse those repositories and discover
what products have proven to be most or least valuable.

Further, another significant difference of this
proposal to related work is what we would
store in our repository.  The contents of other
repositories are not so diverse as types.  For
example, the PROMISE repository contains mostly
defect and effort data, while lacking nearly all the
types of research products of types.  As
another example, the Nebraska Software Artifact
Repository is focused on source code and samples of
test cases.


RELATED WORK: Artifact Evaluation: Apart from open source journals, there have also been some related initiatives
at the conference level. 
For example, several conferences now support artifact evaluations
such as
PLDI, 
SPLASH,  
FSE,  and 
POPL. .
Artifact evaluations are generally performed by a committee separately from the 
program committee, where the artifact evaluation committee reviews artifacts such as 
tools or data provided in a paper.
Authors are encouraged to provide artifacts that can be reused by future 
researchers but 
there are no requirements for how the artifacts are archived, if at all.
While our work shares the same goal as artifact evaluations,
it differs in important aspects. 
Firstly, our intent is to permanently archive all the research products, thus allowing future researchers full access to past research products. Secondly, 
the artifact evaluation committees only offer a very coarse grained
evaluation of the artifacts-- after trying to execute
the artifacts according to the authors' instructions, they mark each artifact
as  ``certified'' or ``not certified.''. 
Our approach, on the other hand, is to generate a much longer
and much more reflective evaluation of all the research products.
Nonetheless, we appreciate the important role of artifact evaluation initiatives,
and can imagine our infrastructure co-evolving with them.




































RELATED WORK: Experience with the PROMISE Repository:
This proposal was designed after a careful
assessment of the strengths and weaknesses of the
old PROMISE repository for repeatable software
engineering experiments (see prom).  Founded in 2005 by PI
Menzies and Jelber Sayyad, this was one of the first
widely-used repositories of software engineering
project data (mostly, static code attributes linked
to defect and effort information).  A key feature of
the repository was that it was linked to an annual
conference. Activity and contributions to the
repository became linked to paper publication (both at
the conference and at the seven journal special
issues where the authors of best conference papers
were invited to submit extended versions of their
conference papers).

Submissions to the repository and conference grew to 2010. The conference received
(10,16,34,53) submissions in (2007,2008,2009,2010)
which was an annual growth of (160,212,156).
As of 2010, the repository was in widespread use.  In that year,
PI Menzies spent two hours on IEEE Explorer and found 73 papers
that used the repository 
. 
Since 2010, the PROMISE repository's contents has
changed very little. While many research papers
still use the PROMISE data, the number of
submissions to the annual PROMISE conference has not
grown past the 2010 levels. 

Many factors contributed
this plateau of interest in PROMISE  including the storage limitations of that service
(due to limitations with where it was hosted, PROMISE could only hold a few gigabytes of files).
One the main problems was that it failed to
build an effective Internet presence. As more and
more researchers rely on social media to study their
field of research, it is important to have a web
presence that is dynamic and constantly evolving.
Our proposed infrastructure would
create a web site for the journal where many
researchers are exchanging information and
monitoring each others' work.

To state this second problem in a more general way,
PROMISE failed to offer the social and contextual
information required for effective sharing of
research products.  Basili et al.  cautions that any
repository of products from software engineering
projects needs to record the context of each
product since, without that context, newcomers might make inappropriate decisions about the 
products in the repository. To illustrate that point, he records one example where a group
from Brazil reported that a certain NASA software module was more bug prone that the rest.
With contextual knowledge, Basili could see that this conclusion was an error. The module
in question was so simple that it was always given to project newcomers. Hence, it tended to
have more errors as the newcomers ascended the learning curve of that project.

To build and record such context, the original authors of a research product need to interact
with newcomers as they make their tentative explorations of that product. We propose two mechanisms, to facilitate
this interaction:


The quick turn around
time we propose for our journal would enable more information sharing and context recording about artifacts
in our repository.

