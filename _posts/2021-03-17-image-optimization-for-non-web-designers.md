---
title: Image Optimization for Non-web Designers
date: 2021-03-17
categories: reference webdev bestpractices
permalink: /writing/2021/3/17/image-optimization-for-non-web-designers
description: Rules of thumb for the best image formats for your application. Quick primer on the 6 most common image formats on the web
---


Big images can make a page slow. But how big is too big? What kind of image do I use? WTF is a jay-peg anyway? What's wrong with my ping file, it looks great? 

I get these questions often enough that it's worth writing up the answer for posterity. **Here are some rules of thumb for the best image formats by use type, and a quick primer on the 6 most common image formats used on the web.**

There are approximately infinite exception conditions and edge cases – I’m only trying to cover the most common. If you spot an error, please contact me so I can fix it.

* * *

## Rules of thumb: What image type to use for… 

### Logos and Illustrations

* If it's all lines, shapes, and flat colors, no photos, it's a good candidate to replace with an SVG version. Think logos.
* If for some reason it can't be an SVG, or you don’t have a vector version, then PNG is a good choice.

### Photos

* These should be JPEGs, with very rare exceptions. 
* If your CMS supports modern responsive image formats, try WebP too.
* Photo and photo-style images can and should be very aggressively compressed:
	* If the image is less than a quarter of the (desktop) screen, it needs a good reason to be any larger than 100-150kb.
	* If it’s the full width of the page, it should be in the 150–300kb range (and there probably should only be one image this big per page)
	* If it's half a megabyte, send your web engineer back to their room without dinner to think about their poor life choices.

### GIFs

* If it's an animated GIF, your page is bad and should feel bad. **Replace with video.**
* If it's a still (unmoving) image, **replace with PNG.**
* Is there any valid use for a GIF outside of Slack and Twitter? **No. No, there is not.**

### Transparency, Special Effects & Animation

If your design has a sophisticated transparency effect that can only be achieved with a 2 MB PNG, please refactor the page until it doesn't have that dependency. That's just silly. 

If your design has a giant photo which needs to be cut out from its background, consider using [SVG masking](https://developer.mozilla.org/en-US/docs/Web/SVG/Tutorial/Clipping_and_masking) of a JPEG. (You can do some [clever things](https://codepen.io/tutsplus/pen/wyrJqP) with this. It even supports semi-transparency.)

If your design needs animation, consider replacing it with Javascript or CSS animation. You can get better control that way, too. And adapts nicely by device. And your page will be much faster. All kinds of good things happen this way.

* * *

## Image Types and What They're Good For

### JPEG
- **Best for:**
	- Photos and photo-like images
- **Characteristics:**
	- Lossy – some image information is discarded to make the file smaller
	- Full color
	- Does not support transparency
	- Compresses images very well
- **Notes:**
	- JPEG was created for photographers – literally for photojournalists who needed to send images over low-bandwidth links! 
	- Text, logos or illustrations tend to get squiggly little marks\* around lines & sharp transitions. Don't use for that. (\*They’re called compression artifacts.)

### PNG

- **Best for:**
	- Logos, flat illustrations
- **Characteristics:**
	- Lossless - no information is lost (*usually)
	- Full color
	- Transparency is supported
	- Excellent compression of flat colors, text, illustrations.
- **Notes:**
	- Created as a less insane version of TIFF that also would support the web. Do not use for photos for web. Great choice for storage as a creative asset. A number of tricks are available to make these very, very small.

### SVG

- **Best for:**
	- Logos and flat illustrations
- **Characteristics:**
	- Vector format – Doesn't store picture data, instead, it stores instructions that tell the web browser what to draw
	- Scales up & down infinitely while retaining perfect quality
	- Can be styled with CSS, and embedded in a page directly
- **Notes:**
	- A vector file acts something like this: "Go up 1 inch, right 1 inch, then return to starting point. Fill in the shape blue. Give it a light grey drop shadow."
	- All kinds of cool tricks available inside SVGs. Not all of them work with all browsers. Shocker.

### GIF

- **Best for:**
	- Nothing.
- **Characteristics:**
	- Lossy - throws away color data to reduce file size
	- Up to 256 colors, no more (it’s called indexed color)
	- Primitive transparency
- **Notes:**
	- **GIFs were literally invented in the 80's. Do not use. Ever.**
	- Patent disputes over GIF lead to the creation of PNG. Now you win at Nerd Trivia Night! Yay!

### Animated GIF

- **Best for:**
	- Slack, Reddit, Twitter, Tumblr
- **Characteristics:**
	- It's a GIF, but with multiple frames, like video
	- Hilariously terrible compression
	- No audio, either
- **Notes:**
	- Invented 2 years after the original GIF, the GIF89a spec added primitive frame differencing to animate images. 
	- Hilariously bad compression of video, but works in browsers without any plug-ins needed. That's why GIFs became popular again - they suck but they work so well at what they do. For purposes of a web page, these almost always can & should be replaced with a video.

### WebP

- **Best for:**
	- Anything but animation\*
	- Making Google PageSpeed Insights engine happy
- Characteristics:
	- Swiss army knife, can act like PNG or JPEG
	- Full color
	- Transparency supported
- Notes:
	- Great photo compression, but subjectively often looks worse than JPEG at similar file sizes. YMMV. Try it and see how it works for you.
	- \*Technically supports animation. But don’t go there.
	- Created by Google to replace both PNG and JPEG. Until recently had limited cross-browser support due to patent wars and corporations being jerks to each other. Based on a shitty, shitty video format that Google bought a decade ago because it didn't want to pay patent royalties for MP4, H.264, and JPEG.
	- Microsoft Edge and Apple Safari only got WebP support in the past year. Lame. But better late than never.

### What about JPEG 2000?
JPEG 2000 has a lot of technically really clever things. However, for web purposes I rarely recommend it. It does not adapt well to extremely low bitrates required for a fast loading web pages. It’s a great choice where you have very high quality images and you must preserve that quality – which is why it’s popular in medical imaging and digital cinema. Also, Safari is the only mainstream browser that supports it.

If you are trying to wring every last bit of performance out of a site, then sure, try JPEG 2000 along with WebP. But it’s not a panacea.

