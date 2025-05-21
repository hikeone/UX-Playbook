---
description: >-
  Responsive design is adapting the looks and behaviour of a product to the
  device it’s used on, and making components and pages accordingly.
---

# Responsive

## Description

Digital products such as websites and apps are used on a wide range of devices: from smartwatches to fridges, from a small ‘smart feature’ phone to an ultrawide 4K or 8K monitor. Keeping the design and layout of a product the same across all those screen sizes would lead to [horrible user experience](https://www.nngroup.com/articles/mobile-first-not-mobile-only/). Here’s where [responsive design](https://alistapart.com/article/responsive-web-design/) comes in.

The idea of responsive design is that the design adapts to the device the product is viewed on. The most important variable is the viewport: the screen size and orientation of devices like phones, or the window size on a laptop/desktop. A common method is to make a default design for 3 standard sizes: mobile, tablet and desktop. However, to support a range of screen sizes and to be future proof, it is best practice to design for continuous scaling (and not for three static sizes). Additionally, you could also consider something like dark mode, by _responding_ to a device setting or the amount of light in the device’s surroundings.

\
![](https://paper-attachments.dropbox.com/s_42EAED51978CBA89AA763A0ECE487B9C94120C5E271D7D73CB3377DDC417C020_1530003758768_breakpoints-01.jpg)![](https://paper-attachments.dropbox.com/s_42EAED51978CBA89AA763A0ECE487B9C94120C5E271D7D73CB3377DDC417C020_1530003831855_breakpoints-02.jpg)\


## Viewport responsiveness

It’s easiest to start with the smallest viewport (width) first, which could be 320 pixels wide. That will pose the most restrictions, while forcing you to order content and interactive elements based on the user’s priority (this might remind you of priority guides). Then, change the design where needed for larger screens: make rules for resizing, reflowing and just changing elements. Don’t try to draw out all possible screen sizes, though.

* **Resizing:** font sizes, paddings and margins, images, etc. can be increased when there is more space.
* **Reflowing:** elements could be moved next to each other. But remember that it’s sometimes better to have one vertical list of elements to keep it scannable.
* **Changing:** a hidden hamburger menu can become an always-visible menu bar.

![](https://paper-attachments.dropbox.com/s_42EAED51978CBA89AA763A0ECE487B9C94120C5E271D7D73CB3377DDC417C020_1530005294544_layout-01.jpg)![](https://paper-attachments.dropbox.com/s_42EAED51978CBA89AA763A0ECE487B9C94120C5E271D7D73CB3377DDC417C020_1530005298282_layout-02.jpg)

### Tips

* Think about ‘touch’ and ‘non-touch’ input. A larger screen resolution does not necessarily mean non-touch. Preferably, you should make all behaviour work in all conditions. So, for example, showing information on hover is probably not smart.
* Keep the amount of breakpoints to a minimum. Start with the smallest components & templates, and only add a larger variation (so a breakpoint) when the smallest component starts to look weird or does not work anymore.
* It is (or used to be) good practice to keep the order of elements the same across screen sizes, such as in this [Google Weather example](https://googlesamples.github.io/web-fundamentals/fundamentals/design-and-ux/responsive/weather-2.html). Over the past few years though, web developers have gotten more and more tools to make components and pages responsive. So feel free to discuss the possibilities with your colleagues!

### Learn more

* [The article](https://alistapart.com/article/responsive-web-design/) which coined the term _responsive web design_
* [Nielsen Norman Group’s definition](https://www.nngroup.com/articles/responsive-web-design-definition/) and [mobile-first is not mobile-only](https://www.nngroup.com/articles/mobile-first-not-mobile-only/)
* [Mobile First](https://abookapart.com/products/mobile-first) by Luke Wroblewski (available in our library)
* [Responsive web design basics](https://web.dev/responsive-web-design-basics/) by web.dev
* [‘User first’ design](https://www.uxbooth.com/articles/where-do-we-go-from-mobile-first/) on making designs context dependent
* [Screen resolution statistics](https://gs.statcounter.com/screen-resolution-stats)
