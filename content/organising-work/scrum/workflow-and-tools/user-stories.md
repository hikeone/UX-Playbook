# User stories

User stories are a way of describing your application in actions your users should be able to carry out. An example of a user story (for an e-commerce project) could be “To checkout multiple products at once, as a shopper, I want to be able to add a product to my shopping cart.”\
**User stories should focus on a feature’s value for the users of your product**. This prevents features making it into the product which have no relevance to that user. By also defining the business value of each story, a Product Owner can determine which stories have most priority.

### In short

The key to writing meaningful user stories:

* Define your **user roles**
* Agree on a common **user story format**
* Make sure each **user story meets requirements**
* Define **acceptance criteria** per story
* Group stories into **epics**

### User roles

A product will (probably) be used by different types of users. A few generic examples are: _a new visitor, a returning visitor, a registered user, a pro account user, a content editor, a site administrator or a sales assistant_. It’s important to distinguish user roles and write user stories from their perspective. Be as specific as you can.

### User story format

Writing user stories in a consistent format makes them easy to use and understand and assures a story contains all important ingredients. Different teams use different formats. The most common ones are:

#### As a ..., I want to ..., so that ...

> **\<Title of user story>**
>
> As a \<type of user>, I want \<to perform some task> so that I can \<achieve some goal/benefit/value>.

_Example:_

> **Customer withdraws cash**\
> As a customer,\
> I want to withdraw cash from an ATM,\
> so that I don’t have to wait in line at the counter.

#### In order to ..., as a ..., I want to ...

> **\<Title of user story>**
>
> In order to \<achieve some goal/benefit/value>, as a \<type of user>, I want \<to perform some task>

_Example:_

> **Customer withdraws cash**\
> To prevent waiting in line at the counter,\
> as a customer,\
> I want to withdraw cash from an ATM.

_Examples borrowed from_ [_Agile User Stories on Scrum Alliance_](https://web.archive.org/web/20160414152515/https://www.scrumalliance.org/community/articles/2013/september/agile-user-stories)**.**

Benefit of the _As a user, I..._ format is that everyone directly empathizes with the user and starts thinking from the user’s perspective. This helps in focusing on the added value for the user. When it feels like user stories are written with too much focus on user tasks without clear goals you should consider the _In order to..._ format as it’s focus is on the goal/value from the start.

### Requirements of a user story

To check if your story is acceptable, use the INVEST mnemonic:

* **I** - Independent
* **N** - Negotiable
* **V** - Valuable
* **E** - Estimable
* **S** - Small
* **T** - Testable

_Source:_ [_INVEST in Good Stories and SMART Tasks, Bill Wake, 2003_](http://xp123.com/articles/invest-in-good-stories-and-smart-tasks/)_._

#### **Independent**

We want to be able to develop our product in small increments in any sequence and shift priorities during the process. A story should therefore depend on other stories as little as possible, so it is more easy to prioritise them.

* Example of (too) **dependent stories**; both require the same login form which isn’t described in a separate story.
  1. To check the order of my status, as a registered user, I want to be able to log in from the homepage.
  2. To use my saved shipping information, as a registered user, I want to be able to log in from the checkout page.
* Example of **Independent stories**
  1. To access and use personal information, as a registered user, I want to be able to log in.
  2. ...
  3. ...

#### **Negotiable**

A user story is not a written contract, but an ambition to fill a need.

* Example of a **Non-negotiable story**\
  To make sure I buy the tablet best suited to my needs, as a customer, I want to know the name, product number, price, operating system, device-aspect-ratio and ...
* Example of a **Negotiable story**\
  To make sure I buy the tablet best suited to my needs, as a customer, I want to be able to see and compare product specifications.

So, first focus on the need you wish to fulfill. Prevent being too specific, just make sure you have the same goal in mind. Later, you can add the specifications as acceptance criteria, like “product specs should include operating system,” etc.

#### **Valuable**

Each story should be valuable to the client or the users: instead of “Connect to the database through a connection pool,” you have “With a five-user database license up to fifty users should be able to use this application.”

#### **Estimable**

There is enough domain knowledge and technical knowledge and the size is overseeable. Not: “The HR Person can post jobs and pay for the online...,” which is way too complicated and vague. (Post jobs? How many forms does that take? What are the payment options?)

#### **Small**

It can be coded and tested within half a day to two weeks, by one or two programmers. Also see[ 8 useful strategies for splitting large user stories](https://web.archive.org/web/20150512164007/http://www.christiaanverwijs.nl/8-useful-strategies-for-splitting-large-user-stories-and-a-cheatsheet).

#### **Testable**

It is clear what the definition of done is.

#### **Exceptions**

Not all issues are or should be user stories. Only issues which have user value should be written as a user story. As an exception, issues which have clear business value, may be written as a user story. For example “To monetize my content, as a company owner, I want to place ads next to my content.”&#x20;

Requirement for design or development can be written as simple or technical tasks and should not be written in user story format. These are for example simply “Define layer names convention for design files.” or “Setup Continuous Integration server for automated build & deploy.”

### Acceptance criteria

Using acceptance criteria is an effective way to ensure focus and make stories testable.&#x20;

#### **Acceptance Criterion 1**

> **Given** that the account is credit worthy and the card is valid and the dispenser contains cash,\
> **When** the customer requests the cash\
> **Then** ensure the account is debited and ensure cash is dispensed and ensure the card is returned.

#### **Acceptance Criterion 2**

> **Given** that the account is overdrawn and the card is valid,\
> **When** the customer requests the cash\
> **Then** ensure the rejection message is displayed and ensure cash is not dispensed.

_Examples borrowed from_ [_Agile User Stories on Scrum Alliance_](https://web.archive.org/web/20160414152515/https://www.scrumalliance.org/community/articles/2013/september/agile-user-stories)_._

Writing the acceptance criteria beforehand helps team members to design and develop a feature and makes reviewing and testing much easier.

### Epics

Features too large to be write in a single user story meeting the INVEST requirements can be described as an epic. An epic can be split into multiple user stories, or several stories can be grouped into an epic. For example, all user stories related to login, logout, user permissions, changing username & password and password recovery could be grouped into an epic called ‘user auth’. This is especially convenient for scheduling releases and long term planning.
