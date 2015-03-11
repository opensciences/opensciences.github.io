---
title: energyconsumption
excerpt: Mining Questions about Software Energy Consumption
layout: repo
author: Gustavo Pinto
---

#URL
  * With change log: [https://terapromise.csc.ncsu.edu:8443/svn/repo/other/energyconsumption](https://terapromise.csc.ncsu.edu:8443/svn/repo/other/energyconsumption)

  #Change Log

  When | What
  ---- | ----
  March 11, 2015 | Donated by [Gustavo Pinto](/repo/people)

# About the data

## Abstract
A growing number of software solutions have been proposed to address application-level energy consumption problems in the last few years. However, little is known about how much software developers are concerned about energy consumption, what aspects of energy consumption they consider important, and what solutions they have in mind for improving energy efficiency. In this paper we present the first empirical study on understanding the views of application programmers on software energy consumption problems. Using StackOverflow as our primary data source, we analyze a carefully curated sample of more than 300 questions and 550 answers from more than 800 users. With this data, we observed a number of interesting findings. Our study shows that practitioners are aware of the energy consumption problems: the questions they ask are not only diverse – we found 5 main themes of questions – but also often more interesting and challenging when compared to the control question set. Even though energy consumption-related questions are popular when considering a number of different popularity measures, the same cannot be said about the quality of their answers. In addition, we observed that some of these answers are often flawed or vague. We contrast the advice provided by these answers with the state-of-the-art research on energy consumption. Our summary of software energy consumption problems may help researchers focus on what matters the most to software developers and end users.

This dataset contains 325 Stack Overflow questions and about 550 answers from about 800 users. The extracted questions were asked between July 31, 2008 and September 6, 2013. The questions in this "base set" are related to energy consumption.

## Sample datum
```
Title: Estimating process energy usage on PCs (x86)
Id: 4485153, Count: 54
Tags: <hardware><cpu><cpu-usage><hardware-interface>
Answers: 4
AcceptedAnswer: 5601187
Created: 2010-12-19 21:17:47.0
Body: <p>I'm trying to come up with a heuristic to estimate how much energy (say, in Joules) a process or a thread has 
consumed between two time points... (remainder of question omitted for brevity)</p> 
Popularity: 42.0
```

## Explanation of fields
**Title:** title of question on SO (Stack Overflow)

**Id:** the ID of the question on SO. Navigate to the question by going to `stackoverflow.com/questions/\<Id\>`

**Count:** where count is n, the n-th SO sample question in the dataset. The sample above is the 54th question.

**Tags:** tags applied to the question on SO

**Answers:** the number of answers used on SO.

**AcceptedAnswer:** the id of the accepted answer. Navigate to that answer by going to `stackoverflow.com/questions/\<Id\>/#\<AcceptedAnswer\>`

**Created:** creation timestamp of the question

**Body:** HTML contents of the question

**Popularity:** a normalized measure of question popularity as a comparison between energy consumption questions and average SO questions. Popularity `P = S + A + C + F + V`. S = question score (combination of upvotes and downvotes). A = number of answers, C = number of comments, F = number of favoritizations, V = number of views when question was collected. Each variable is normalized by taking the variable and dividing it by the average of that value for all Stack Overflow questions.
