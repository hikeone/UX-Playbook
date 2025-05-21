# Scalable Vector Graphic (SVG)

## In short, what are SVG’s?

Saving a file as SVG (Scalable Vector Graphic) will create a code that tells the browser how to draw your graphic. It simply is a plain text file that describes lines, curves, shapes, colours and text.&#x20;

## Why SVG’s?

* **Performance**

An important aspect for webperformance is the size of a file on a webpage. The size of an SVG depends on how complex it is. The simpler the shape, the less lines of code you'll need to describe it. This results in a smaller file size and a faster loading graphic.\


* **Scalability**

As the name indicates, SVG’s are vector graphics; meaning they use code to describe shapes, resulting in scalable and resolution-independent graphics. The SVG retain sharpness no matter what the size is unlike pixels and its limitation. \


* **Flexibility and Interactivity**

An SVG can be used wherever an image can be used, however it can also be used directly in HTML. The latter makes it possible to style and animate the SVG based on user actions on the page.

## When to use SVG's as file format

* Logo's and icons
* Line-based illustrations or simple graphics
* Animations

\
SVG's are not suitable for photo's or raster graphics. It is possible however to include photo's (e.g. JPG) in your SVG file, but they will either enlarge the file size significantly or they will link to an outside file.

## Before exporting SVG's

### First of all, talk with your developer

Especially when you want to animate your graphic, it’s best to sit down with the developer and talk about how you want to use or motion the graphic. Sometimes this can influence the way you want to design your graphics, which can save you time. &#x20;

### Converting strokes

Before you export your file to SVG, make sure to convert your strokes or fonts into outlines. This prevents having wrong proportions when scaling your design. There are however some exceptions for not converting your strokes to outlines. You should use strokes if you want to:\


* **Use different colours**

When you use strokes in your design, you’re able to easily give it a different colour. For example: The animations on the website of De Voorhoede.\


* **Animate (drawing)**

A huge benefit of SVG animations over GIFs or videos is that they are super lightweight and load very fast. Keep the original lines and shapes before saving your SVG because once it's converted to outlines / filled shapes they are not longer usable for animations.\


* **Use smaller sizes**

A stroke exists out of 1 line with two coordinates, where a filled shape has a boundary with 4 coordinates which makes it automatically bigger.&#x20;

\
When you’re not sure what to do, **ask the developer** for the best solution.&#x20;

### Don’ts

Don’t use masks, gradients or any other complex effects. Your graphic has to be described in code that will be rendered in different browsers that have different feature sets. So keep your file organised and simple.&#x20;

Also, don't use Sketch to export SVG's. The reason to choose Illustrator over Sketch is because Sketch can sometimes mess up your SVG. For example; Graphics with stroke alignment inside or outside don’t convert to code as a stroke, but as a mask. Some browsers don’t support these masks within code which eventually leads to showing the graphic not the way it should be. You can work on your graphic in Sketch if that is what you prefer, but make sure to export it to SVG in Illustrator.

## Exporting SVG’s in Adobe Illustrator

1. File > Export > Export As …
2. Choose SVG as the format and check the ‘Use artboards’-box. When you have multiple artboards, select ‘range’ and fill in the right artboardnumber(s). Click on the Export-button to export.
3. Before the file will export, a window with SVG options appears.

![Most common settings when exporting a SVG](https://lh6.googleusercontent.com/BfN4kIcxJFSx1yZBLuGSdKcGv108ntZ-iI0jsap2XteD00zMCJzvaUwX9w9tCiS8qNd8pIObMzgo8oNXmmNmm3riXfyyf-6PVFwomXV0HpfDMHWxjIsfWBOinmb0YOQJhwzsVuWE)

**Styling**&#x20;

Choose presentation attributes in the styling options. It makes it easier later to define new colours using css overwrites.

\
**Font**

Talk to your developer when you want dynamic or animating text. Choosing SVG is the most efficient option. Choose convert to outlines if you’re having trouble with how typography is rendered in your export.

\
**Images**&#x20;

Discuss with your developer when you want to include a raster graphic (like a JPG). If you’re going to use a raster graphic in your SVG, you have 3 options.&#x20;

* Choosing ‘Preserve’ means the image linking behaviour will be preserved from the original illustrator file.&#x20;
* Choosing ‘Link’ will link the document to the raster graphic exported from the original Illustrator file. This is useful for multiple SVG files that share common raster graphics.&#x20;
* Choosing ‘Embed’ will make it part of the SVG.&#x20;

\
**Object ID’s**&#x20;

This is what is used by CSS or JavaScript to target parts of the graphic for adjusting.&#x20;

* ‘Minimal’ is usually the best choice because it’s great for file size.&#x20;
* Choosing ‘Unique’ will create long strings of text, but it’s a struggle to copy those strings to CSS or JavaScript.&#x20;
* You can choose ‘Layernames’ if you’ve named all your layers in Illustrator.

&#x20;**Decimal**&#x20;

When you have a complex file, make the number bigger for more precision. If you make the number smaller, it will use less lines of code to describe the shapes and lines in your file. This results in a smaller file size, but also in rougher shapes. Leaving it at 3 is usually your best choice. You can decrease the precision with online checking tool [SVG OMG](https://jakearchibald.github.io/svgomg/) later and see the effect it has.

\
**Minify**&#x20;

When you run your SVG through SVG OMG you don’t have to select ‘Minify’ to generate SVG code with minimal IDs, indents, lines and white spaces because the tool will do it for you. So, only select ‘Minify' if you’re not going to use the tool.&#x20;

\
**Responsive**&#x20;

When you check this box, the SVG doesn’t have any width or height. In most cases this means that it automatically will fill as much space as possible. By turning off responsive, you’re adding the width and height from the artboard to the base SVG, so the SVG does know what to do. We usually advice to turn it off.\


4\. Click on the OK-button to export your SVG!

## One last thing, check your file!

Use the online tool [SVG OMG](https://jakearchibald.github.io/svgomg/) to inspect and optimise your SVG.

* Load the SVG export from illustrator
* Does it look the same as the original Illustrator file? If not; try adjusting the decimal export setting. Do not go mad zooming in.
* Does it look good in the web browser? Try at least two different browsers. Pick one you think it can be problematic, Internet Explorer 11 for instance.
* Inspect the code in the ‘Markup’ tab. See how many lines of code are used to describe the shape and decide wether it corresponds to the complexity of your shape. (e.g. a hundred lines for describing a cirkel means something's off)
* Check the file size (shown in bottom right). Most SVG's only take up a few bytes, up to a few kilobytes for complex shapes. Is your file is very large, check it in the code editor and figure out if it perhaps included unwanted images or shapes that are not visible within the boundaries of your artboard.
* If the PNG version is smaller in file size, then maybe just use PNG instead of SVG.

