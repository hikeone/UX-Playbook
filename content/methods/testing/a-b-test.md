---
description: >-
  An A/B test is a method for comparing two variations of something against each
  other to determine which one performs better. That somethingcan be an image, a
  button, a headline, or some other element.
---

# A/B test

A/B testing is a great tool to optimise conversion. That is, it enables you to make incremental improvements to your website or app. As a designer it helps to have an understanding regarding the underlying theory of A/B testing, and how it works in practice. Just as designers do not have to develop code everyday, it sure helps to have an general understanding of how code is written. The same counts for A/B testing.

## How to

We can define 5 steps for performing an A/B test:

1. [Form a hypothesis](a-b-test.md#1-form-a-hypothesis)
2. [Calculate sample size](a-b-test.md#2-calculate-sample-size)
3. [Create variation](a-b-test.md#3-create-variation)
4. [Set up & run the A/B test](a-b-test.md#4-set-up-and-run-the-a-b-test)
5. [Analyse results](a-b-test.md#5-analyse-results)

### **1.** Form a hypothesis

A hypothesis is a prediction you create prior to running an experiment. Running the experiment will either prove or disprove your hypothesis. These are bold statements, and they are based on prior research. Using hypotheses forces you to answer useful questions, instead of engaging in a wild goose chase.\
There are a number of ways to form your hypothesis. The following framework can help you with that:

```
IF[variable],
THEN[result],
DUE TO[rationale].
```

**Variable**\
An website/app element that can be modified, added, or taken away to produce a desired outcome.

**Result:**\
The predicted outcome(e.g.more landing page conversions, clicks on a button, or another KPI/metric).

**Rationale:**\
Demonstrate that you have informed your hypothesis with research(e.g.surveys, analytics, usability tests).

Let's form a hypothesis with the use of an example: the Ziggo B2B internet(product)page.Prior qualitative research indicated that people were uncertain if Ziggo was the right choice for them. You have dived into the social proof theory, and you predict that a social proof component would make people more certain about Ziggo. So our hypothesis would state:

```
IF[we stimulate more certainty for ordering the product],
THEN[we will generate more successful orders],
DUE TO[priorqualitative research & the social proof theory]
```

### **2.** Calculate sample size

On the internet you will read a lot of magic numbers like“Youneed at least 1000 visitors”. Math is not magic, math is math. And what we are dealing with is slightly more complex than that. So how do you calculate the sample size? That depends on three factors:

**Baseline conversion rate**\
This is the current conversion rate, which can usually be found in the analytics dashboard(e.g.Google analytics). In essence it is the number of successful orders divided by all the visitors who saw the page. Let's say that the conversion rate for our example page is 3%.

**Minimum detectable effect(MDE)**\
The MDE is a calculation that estimates the smallest improvement we would want to detect. Let's say that we want to detect a 15% improvement against the baseline, which makes our outcome 3 \* 1.15 = 3.45%.

**Statistical significance(P-value)**\
Statistical significance answers the question“Howsure do we have to be that the end result is based on changes we made, and not due to chance?”The general accepted value is 95%.

Now that we have these numbers, we can calculate our sample size. There are a number of tools available for this, but they all do the same trick. Let’s use[“Optimizely](https://www.optimizely.com/sample-size-calculator/)[Sample Size Calculator”](https://www.optimizely.com/sample-size-calculator/)for now. When we input our numbers, we see that we need 24.000 people per variation.\
![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524139045197_image.png)

**Understanding the sample size calculator**\
Large baseline conversion rates require lower sample sizes. That is, if your conversion rate baseline is 2% and you want to detect a 10% improvement(i.e.MDE), the outcome would be 2.2%. Now imagine your baseline conversion rate is 8%. With the same 10% MDE, the outcome would be 8.8%. That 0.8% will be easier to detect than the 0.2% difference between 2% and 2.2%.

**How long to A/B test?**\
The answer is quite easy: when you have reached the sample size of each variation. However, when you want to estimate the length of the test, you can take the total sample size and divide it by your average number of visitors per day.\
What you nevershould do is stop a test just because it reaches statistical significance!

### **3.** Create variation

At this step you make your variation. Take the example of Ziggo:

![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524139325438_a1.png)![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524139362888_b1.png)\


### **4.** Set up & run the A/B test

Now we have made our variation, we can set up our A/B test. There are many tools available to perform an A/B test(e.g.Optimizely, VWO, Adobe Target). While this is the first thing many people think about when creating an A/B test, it is actually not the most important thing. By any means, you should first think about the prior steps, before worrying about picking a tool. Let’s pick Optimizely as our tool.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524139981963_image.png)![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524140002955_image.png)![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524140012255_image.png)

At this point we need to define the element to track. In our case, we want to track the pageviews of the“thankyou” page(i.e.the page you see right after you ordered the product) between the variations. This allows us to compare the amount of orders per variation.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524140020199_image.png)

Lastly, ensure the traffic allocation is 50/50 divided. In order for Optimizely to track, a code snippet needs to be implemented in the \<head> code of your website. And then you start the experiment.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524140111916_image.png)

### **5.** Analyse results

After you have reached the sample size of each variation, you can analyse the results. In this case the variation significantly outperformed the control variant.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_CF6B4A2496B9D89998347B9C4451F49A19751252768C9108E7CA19A93A0479DF_1524141097812_image.png)

* **Visitors**: the number of unique visitors who reached the control/variation.
* **Unique Conversions:**&#x74;he number of unique visitors who triggered the goal.
* **Conversion rate:** the percentage of“uniqueconversions” divided by“visitors”.
* **Difference Interval:**&#x74;hink of it as your"marginof error”. The conversion rate is actually a range. In this case it is probably between 4,5% and 5,5%.
* **Improvement:**&#x74;he relative difference between the variation conversion rate and baseline conversion rate.
* **Statistical significance:**&#x74;his measures how sure we are that the difference we see in conversion rates(betweenthe control and variation) is due to the changes we made, and not due to chance.

