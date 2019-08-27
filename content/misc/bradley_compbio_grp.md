---
title: new branch
parent: misc
nav_order: 2
---

# Recap Comp Bio Student/Post-doc meeting: Rob Bradley
SKH 20190318

## Overview

Rob's presentation was titled "The promise and peril of analyses of primary patient data" but it ended up being a rather informal discussion of statistical practices in biology.
We talked about power analysis and false discovery rate.

## Power analysis

A good portion of the discussion was on power analysis.
Rob talked about how this is standard practice and knowledge for biostatisticians but rarely taught in molecular biology courses.

Rob gave the example of you are designing an experiment with some perturbation (mutation) and some phenotype (worm speed).
We are taught or it is intuitive to ask *does my perturbation cause my phenotype?* where power analysis asks *how big does my phenotype (effect size) need to be in order to see an effect with my experimental design?*

We walked informally through an another example where you have a mutation which causes a cancer to grow twice as fast but the variability (mouse-to-mouse) is 0.5 times the effect size.
How many mice should you use? People in the room guessed 3-5 but Rob said it is about 10 mice and there is still a 1/5 chance you don't see the anticipated effect (with statistical significance) at all.

The overarching idea being that a hypothesis might be true but you cannot detect it without a very large experiment.

The exact formula is online but the idea is that the sample size you should use is a function of  
1. the effect size (signal)
2. noise/standard deviation between experimental replicates
3. desired power
4. desired significance level
5. alternative hypothesis (one-sided vs two-sided)

## Controlling false discovery rates

We then spent time talking about ways to control your false discovery rate (multiple hypothesis testing).

The three main things we talked about were
1. cross-validation. Are your results robust?
2. limit the number of tests. Decide the number of hypotheses you are going to test and stop at that number.
3. Correct your pvalues.

We also discussed "meta FDR".
This is the idea that there are "hot topics" in fields and that the hypothesis you are testing is probably being tested by many other people.
That is you could be caught with a high FDR through "no fault of your own".
A concrete example of this is a drug companies all testing similar molecules at the same time.

## Resources

Finally, Rob suggested the blog https://simplystatistics.org/ by
Rafa Irizarry, Roger Peng, and Jeff Leek
