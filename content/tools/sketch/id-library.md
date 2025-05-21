---
description: >-
  The Hike One ID library for Sketch will help you build your wireframes faster,
  easier and more consistently. You can think of it as a wireframing kit.
---

# Hike One ID library

The library is maintained by Suzanne Wensveen and everything around it is communicated inside our slack channel #hikeone-id-library.&#x20;

{% hint style="info" %}
If you’re not familiar with sketch libraries, please read about [sketch libraries](sketch-libraries.md) first.
{% endhint %}

![](<../../.gitbook/assets/image (18).png>)

## What’s included?

The library consists of a large collection of wireframing elements, built as resizable symbols:

* Text styles and Colour styles
* Icon set
* Cursors and Gestures
* Basic components like: buttons, inputs, checks, toggles, tabs, labels, segmented controls and notifications
* Placeholders for images, video and graphs

## How to use?

1. [Sync the folder that contains the library](id-library.md#step-1-sync-the-dropbox-folder-that-contains-the-library)
2. [Add the ID library to Sketch](id-library.md#step-2-addthe-idlibrary-to-yoursketch)
3. [Use the symbols in a new Sketch document](id-library.md#step-3-run-the-idlibrary-in-a-new-sketch-document)

### Step 1: Sync the dropbox folder that contains the library

The ID library is a shared library and it is located in our dropbox folder. Sync this folder to use the library and to receive the updates:\
`hike-one_design / 01_templates / sketch / Sketch-libraries / Hike One ID Library`

Alternatively you can download a version here:

{% file src="../../.gitbook/assets/Hike One ID Library.sketch" %}
Hike One ID Library (Build 49)
{% endfile %}

{% file src="../../.gitbook/assets/Hike One ID Textstyles.json" %}
Hike One ID Textstyles (Build 49)
{% endfile %}

### Step 2: Add the IDLibrary to yourSketch

Goto Sketch / preferences, and open the “Libraries” tab. Click the “Add Library…” button. Find the library in the path specified above, and click on “Open"

<img src="https://d2mxuefqeaa7sj.cloudfront.net/s_598DC75F4013E4EE7F43BBC5B705750AC132BFEC91E1DBAE92EA7D1567BFF764_1532343865926_image.png" alt="" data-size="original"><img src="https://d2mxuefqeaa7sj.cloudfront.net/s_598DC75F4013E4EE7F43BBC5B705750AC132BFEC91E1DBAE92EA7D1567BFF764_1532343783146_image.png" alt="" data-size="original">

The Hike One ID Library should now be in your list of libraries, and have a checkmark to indicate it’s active. You can check the time & date of the latest update here as well.

### Step 3: Run the ID Library in a new Sketch document

\
![](https://d2mxuefqeaa7sj.cloudfront.net/s_598DC75F4013E4EE7F43BBC5B705750AC132BFEC91E1DBAE92EA7D1567BFF764_1532338298902_image.png)

Select the elements you want to use via the Symbols menu drilldown. This gives you a preview of the elements you can use. When you’re used to the library (contents) I strongly recommend using the [Runner](http://sketchrunner.com/) plugin. Open it with `Cmd+'`, and set the default to the ‘insert’ functionality to speed up the process\


## FAQ

### How do I get library updates?

The library will be updated via the default Sketch library update process. Check the notifications in the top right hand corner of Sketch to see new updates:\
![](https://d2mxuefqeaa7sj.cloudfront.net/s_598DC75F4013E4EE7F43BBC5B705750AC132BFEC91E1DBAE92EA7D1567BFF764_1532339633746_image.png)![](https://d2mxuefqeaa7sj.cloudfront.net/s_598DC75F4013E4EE7F43BBC5B705750AC132BFEC91E1DBAE92EA7D1567BFF764_1532339660683_image.png)\


Release notes will be available through the library slack channel: #hikeone-id-library\


### Will the elements resize automatically?

Short Answer: No\
Long answer: The elements were designed to be resizable (in most cases in horizontal direction), but will not resize automatically with your content. If needed, an overflow mechanism is built into the element to ensure content does not run ‘out of’ the element. If you’ve changed the size of the elements, and the size of that element is changed in the library, Sketch will keep the sizing as set by you in your file, and override the library element dimensions. If needed, you might need to reset the element to original size by hand.

### How do I change the state of a symbol?

By default, the elements in the library are set up so that the states of the elements are clustered. This means that a different state can be easily be selected through the symbol drop-down.

![](https://d2mxuefqeaa7sj.cloudfront.net/s_598DC75F4013E4EE7F43BBC5B705750AC132BFEC91E1DBAE92EA7D1567BFF764_1532343131470_image.png)\


### Can I add my own symbol to the library?

Short Answer: No\
Long Answer: You can request a new element via the Slack channel. If approved, it will be added to the backlog. To ensure library quality and consistency however, it’s best to keep one person in charge of the content of the library.

### Is my project suitable for using the library?

Suitability depends very much on the requirements of the project you’re in:

ID library is suitable for:&#x20;

* **New projects**\
  There are little to no pre-existing wireframes yet.
* **Collaboration**\
  You need to build consistent wireframes with two or more people.
* **Getting focus on interaction**\
  You want to try removing all the ‘chrome’ to (get your stakeholders to) really focus on the interaction.

ID Library is _not_ suitable for:

* **‘Crystallised’ projects**\
  You already have a large set of components or you can re-use VD components
* **Custom-Custom projects**\
  If you require a lot of custom stuff (why?) the library will not save you time
