---
description: >-
  Accessibility entails designing applications that are usable by everyone,
  regardless of visual, motor, auditory, speech or cognitive abilities,
  situation and identity.
---

# Accessibility

> Related concepts: Inclusive Design, Universal Design

Accessibility of a digital product revolves around making a product usable, or ‘accessible’ for as many people as possible, including those with a (situational) impairment. By taking into account users with impairments from the very start of your design process, you ensure your product works for a much larger group. We call this inclusive design. It also prevents accessibility becomes an afterthought or worse; a separate product for specific target groups. Moreover, an accessible product always leads to improved usability overall, something every user experience should strive for.

{% hint style="info" %}
From 2025, or even earlier, the [European accessibility act](https://ec.europa.eu/social/main.jsp?catId=1202) will require some types of products to be accessible by law.
{% endhint %}

## **General: WCAG**

The Web Content Accessibility Guidelines (WCAG) are often used guidelines for web/digital accessibility. It’s good to know there are three levels and four principles. It’s also a versioned set of guidelines which is updated once in a while, the 2.2 version is to be published somewhere around 2023.

### Levels

The WCAG has three levels of conformance:&#x20;

* A covers the real basics, all products should adhere to this
* AA is the most common level; required for governmental websites and a really good idea for public products
* AAA is quite advanced and only required for specialized audiences

### Principles

All guidelines fall under their four principles; things should be...

* perceivable - users can see/hear/feel all elements
* operable - users can interact with all relevant elements
* understandable - texts are readable, interactions are predictable, errors are helpful
* robust - it works with the iPhone 20, but also an old desktop with a screen reader

## Things to consider

* [Colour](accessibility.md#colour)
* [Typography](accessibility.md#typography)
* [Forms](accessibility.md#forms)
* [Content markup & keyboard navigation](accessibility.md#content-markup-and-keyboard-navigation)
* [Images & videos](accessibility.md#images)
* [Language use](accessibility.md#language-use)
* [Animations & movement](accessibility.md#animations-and-movement)
* [Time limits](accessibility.md#undefined)

### **Colour**

Smart use of colour can aid the usability of an application. High colour contrast generally improves accessibility for users with poor sight. For example: Ensure text has enough contrast with its background (use tools like [Colour Contrast Checker](https://colourcontrast.cc/) or [Contrast in Figma](https://www.figma.com/community/plugin/748533339900865323/Contrast)), and don’t use colour as the only indicator for error states, but instead also add text or icons.

### **Typography**

To make information within an application accessible, it is important to make the text legible. This can be achieved by choosing a legible font, but also by using enough whitespace and contrast. Users can enlarge the font of an application themselves, so make sure your lay-out still works with a larger font.

### **Content Markup & keyboard navigation**

The way you build up the content on the page, influences how a screen reader or keyboard user will navigate through the page. So:

* Build up the content on the page in the (logical) order you want to communicate the message.&#x20;
* Make the application navigable with keyboard input, for people with motor disabilities or screen readers. This means avoiding interaction which requires hover states (like drop down menus which open on hover), and making a logical order of menu items and hyperlinks.
* Moreover, use (informative) and hierarchical headers to break up the text (h1, not just bold large text), because that is how screen readers can ‘scan’ the page.&#x20;

### **Forms**

It is important to always use labels on input fields. Without labels, screen readers ‘miss’ the input field, and even sighted users might not know what it is about.&#x20;

### **Images**

When telling a story with images, always provide clear descriptions for users with screen readers. You could also provide alternative text (the [alt attribute](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/Img#attr-alt)), which is read out loud in place of the image and shown when the image can’t load. Note: when an image is purely decorative, it should have an empty alt attribute (`alt=""`).

Don’t make text into an image, because then the content will be missed by screen readers (and search engines). Lastly, icons are often not widely understood, so make sure there is a always label (only use tooltips when really necessary).

### Audio and video

For videos and audio (like podcasts) there should be captions or transcripts available, as well as controls to play and pause the content.&#x20;

### Animations & movement

Movement can help to make an interface more clear or playful. However, continuous movement (like animated gifs or pulsating animations) can distract users from other content, while large animations can cause vertigo or motion sickness for people with a [vestibular disorder](https://www.a11yproject.com/posts/understanding-vestibular-disorders/). Consider only using small and meaningful animations, or providing alternatives to people who turn on the [reduced motion accessibility setting](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion), when using carousels, parallax, horizontal scrolls, etc.

### **Language use**

To make the content of an application accessible to a wide range of people, it is good practice to use easy to understand language. This means avoiding jargon, academic writing and metaphors. Use short sentences and to the point wording. Also consider that links will be read without their context by screen readers, so avoid ‘read more’, ‘click here’ and similar links. Instead, use descriptive links, like the title of an article. Additionally, be mindful of exclusive language, for example when dealing with gender, ethnicity and disabilities.

### Time limits

In some applications, users have to take action within a certain time frame, for example for security reasons. However, this can lead to stress or even prevent users from being able to complete the action entirely. Try finding other solutions or allow users to extend the time period.

### Research and testing

Take diversity into consideration when selecting participants for research activities and ensure the interviews themselves are inclusive and accessible, too. Make sure participants are justly compensated for their time investment and their privacy is respected. Also consider asking the recruitment agency to select people with specific disabilities or assistive technology uses, and don’t source your participants just from the current user base of a product.

## Tips

* Incorporate accessibility principles from the beginning of the design process, not as an addition later on. You could make a list of hurdles people might face in relation to your product, to keep in mind while designing.
* Start your designs with a bare priority guide, so the entire design has a text-only and keyboard-friendly version. Then, enhance it with colours, visuals, layouts, etc. without replacing/deleting the text-only version.
* Make sure your prototypes are accessible by turning on the [accessibility mode](https://help.figma.com/hc/en-us/articles/7810391964695-Accessible-prototypes-in-Figma) in Figma, making it in something like Webflow, or even coding them yourself in HTML.
* A part of accessibility quality depends on how the code is built up (using headings and lists in HTML, for example). Make developers aware of accessibility issues.&#x20;
* Perform an accessibility audit on the live product to check how your application performs. This can be partly automated with something like [axe](https://www.deque.com/axe/browser-extensions/), but should also be tested manually. An easy place to start would be [using a screen reader yourself](https://yakim.nl/articles/voiceover-testing/) or just navigating through a website with your keyboard.
* Also test the live product with people who use assistive technologies like screen readers on a regular basis.
* Think of how a service you’re designing could be used to harm people (also called [subverted design](https://www.youtube.com/watch?v=r12jEV243Yc)), in order to prevent that from happening. This goes a little further than just accessibility.

## Learn more

* [Designing for accessibility is not that hard](https://uxdesign.cc/designing-for-accessibility-is-not-that-hard-c04cc4779d94) by Pablo Stanley (article) is good to get a really **quick overview**
* [Accessibility for Everyone](https://abookapart.com/products/accessibility-for-everyone) (book) is good to **dive deeper** into it (we’ve got it in the AMS office!)
* The [Intopia Not-Checklist](https://not-checklist.intopia.digital/) and the [Accessibility checklist](https://webflow.com/accessibility/checklist#start) by Webflow both help to **check your work**—both use (part of) the [WCAG](https://www.w3.org/WAI/WCAG21/quickref/)
* We also have our own [lists of responsibilities](https://www.figma.com/file/M7Y59QtTf2QG0Jk5kTolgU/Inclusion-in-design-process?node-id=602%3A2\&t=uwpzQNw1dSXl0Et8-1) per **role in the design process**.
* [Do’s and don’ts on designing for accessibility](https://accessibility.blog.gov.uk/2016/09/02/dos-and-donts-on-designing-for-accessibility/) (posters) help you to **remind yourself** of it often
* [Inclusive language](https://brand-at.webflow.io/voice-and-tone#inclusive-language) as part of the Webflow brand guide helps to **write better copy**
* [Tetralogical](https://tetralogical.com/) has lots of resources, like [foundational explanations](https://tetralogical.com/blog/2022/11/08/foundations-native-versus-custom-components/) and [videos of people using assistive technologies](https://tetralogical.com/blog/2021/12/24/browsing-with-assistive-technology-videos/)
* [Testing/monitoring](https://www.gov.uk/guidance/accessibility-monitoring-how-we-test) by UK.gov

Methods that can help in applying accessibility principles:

* [Copy](../methods/design/copy.md)

## Who to ask

* We have worked with [Visio](https://www.visio.org/home/) in the past, to check our designs on accessibility for the visually impaired. Contact Roderick Trompert for more information.
* In 2022, we had [Digitaal Toegankelijk](https://digitaaltoegankelijk.nl/) organise an accessibility workshop for us. Contact Yvonne Licher for more information.
* Floris Jansen is currently the [topic guide](https://app.holaspirit.com/o/5fca2b9cce82c73a4f26ef80/governance/roles#role-628b7e2bb52c3006211bd462) on accessibility within the Product Design circle.
