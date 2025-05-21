# #6 Identifying underlying assumptions

An assumption is **something you believe to be true** (but not necessarily know to be true). In product, when we talk about assumptions, we mean things that need to be true in order for our solution to work.&#x20;

To wrap your head around the concept of assumptions, try phrasing them in different ways:&#x20;

* This solution will only succeed if _\[x]_&#x20;
* This solution will not succeed unless _\[x]_&#x20;
* This solution depends on '_\[x]'_ to succeed&#x20;
* If '_\[x]_' is proven wrong, it will cause this solution to fail.

When deciding which solution to build, we are looking to **mitigate risk** (of shipping the wrong thing, of wasting resources, and of not making our customer happy). We can only mitigate risk, if we know how much risk is involved in our solutions. We can only know how much risk is involved, if we identify what the underlying assumptions of our solutions are.&#x20;

So we make the underlying assumptions of a solution explicit by asking ourselves what we already know about the solution, and what we think we know, but are not sure about. We compare and contrast our assumptions in order to prioritise which to test (first). We start testing the riskiest ones: the ones with **low evidence and high importance**.

<div data-full-width="true"><figure><img src="../../../.gitbook/assets/image (51).png" alt=""><figcaption></figcaption></figure></div>

## Types of assumptions

### Desirability

Why do we think someone will want this solution? And what do we think our customers are willing to do to get value from this solution?

* _"Readers of (paid) articles want to share content with friends through e-mail."_

### Viability

Why do we think this solution will be good for business? Think not only about willingness to pay, but also about costs the business incurs in implementing this solution.

* _"Receivers of a shared (paid) article will pay to read it."_

### Feasibility

Why do we think we can build this solution? Think about skills, knowledge, technical possibilities, compliance, security.

* _"The e-mails about shared (paid) articles will get through the receivers' spam filters."_

### Usability

What is our customer able to find, understand and do?

* _"Readers will notice the option to share a (paid) article."_
* _"Readers will know the e-mail address of the person they want to share the (paid) article with."_

### Ethical

Why do we think there’s no potential harm in offering this solution? Think of things like data usage, inclusion, social dynamics.

* _"Readers won't share (paid) articles that might offend the receiver."_

## Tools

* Research repository such as [Dovetail](https://dovetail.com/) for listing assumptions and keeping track of related solutions, related experiments, and whether or not the assumption is validated
* Either [Dovetail](https://dovetail.com/) or a collaborative tool like Miro or FigJam for 2x2 mapping for prioritisation – use a collaborative tool in case you're identifying and prioritising assumptions in workshop format, with stakeholders

{% hint style="info" %}
For workshop format, see [opportunity-mapping-w-team.md](../workflow/explore/opportunity-mapping-w-team.md "mention")
{% endhint %}
