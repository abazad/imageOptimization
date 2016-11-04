# Image Optimization for Web Images
Best practices and general techniques

## What do you mean by 'optimize'?
Once you design an image, graphic, or icon for a website, a developer has to take it and put it online. This can cause some problems:

- Images - even little ones - have file sizes many times larger than a text document or piece of code. For instance, compare the file size of cat.jpg in this repo to the 8000 line main.css file. 

- Images have different file types, each with their own unique pros and cons

## Can't the developers do it themselves?
Sometimes - but usually, no. Most developers have as much design knowledge as you have development knowledge. Even those that have more design experience might not have the tools at their job, as many companies only buy Sketch/Adobe liscences for designers. Basically, most employers will consider this your responsibility.

## How do I export an image in Sketch?
Luckily, this part is fairly simple - Sketch has a button for it:
https://www.sketchapp.com/learn/documentation/11-exporting/1-exporting-layers.html

## What options should I choose?
It depends. Here's some General Rules:

### Cropping:
Choose the exact layer your image is on, and only export what you need - trim the object so that there's no needless whitespace or other objects attached to it.

### Format:

#### Rasterized: 

- JPG = Use for photographs only. These tend to be much higher file sizes, as the format was created to specifically reproduce highly complex digital camera images.

- PNG = Standard for most icons/graphics. Has background opacity, so that circular/non-square icons do not have a solid color background, but instead pick up the color of whatever is behind it

- GIF = Not used for much anymore. [Except for animated gifs, of course](https://media.giphy.com/media/Y8ocCgwtdj29O/giphy.gif).

#### Vector:

- SVG = Best for vector art of any kind. Can be scaled infintely.

- SVG Code = The greatest thing ever. Can't be directly exported from Sketch, but developers can open .SVG files in their code editors to grab it. Same benefits as SVG, but can also be manipulated with CSS and JavaScript.

### Size:

#### Rasterized:

1x = Normal size. Exactly how it is in the artboard.

2x = Double the dimensions of the width and height - so technically 4x the size. This is how you make retina images - the developer will then use CSS to squish the image back down to half the size, making the image super dense with pixels. The result is a super clean rasterized image.

#### Vector:

Vector images like SVGs are not affected by size - they're infinitely scalable.

## What should I name it?
- **Something logical.** The name should tell you what the image is without opening it.
- **No Version numbers.** Don't make developers compare versions, that's your job. Also, version numbers make for bad, inspecific code.
- **No Spaces.** Spaces are hard to recreate in code. It will almost always cause some kind of error. 

























