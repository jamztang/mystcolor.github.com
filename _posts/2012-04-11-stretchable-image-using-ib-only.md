---
layout: post
title: Stretchable images in UIImageView using IB only
comments: true
share: true
category: slides
tags:
- iOS
- development
- Interface Builder
- UIImageView
- stretchable images
---

So maybe you wonder if there's any way to use stretchable images without coding, but using Interface Builder only.

The problem is there seems to have no option for you to pre-configure your UIImage while you're assigning an UIImage in IB, so here is how you can achieve the same thing by assigning the correct property to your UIImageView.


<div style="width:425px" id="__ss_12339589"> <strong style="display:block;margin:12px 0 4px"><a href="http://www.slideshare.net/mystcolor/stretchable-images-in-uiimageview-using-ib-only" title="Stretchable images in UIImageView using IB only" target="_blank">Stretchable images in UIImageView using IB only</a></strong> <iframe src="http://www.slideshare.net/slideshow/embed_code/12339589" width="425" height="355" frameborder="0" marginwidth="0" marginheight="0" scrolling="no"> </iframe> <div style="padding:5px 0 12px"> View more <a href="http://www.slideshare.net/" target="_blank">presentations</a> from <a href="http://www.slideshare.net/mystcolor" target="_blank">mystcolor</a> </div> </div>


Say goodbye to

    - (UIImage *)stretchableImageWithLeftCapWidth:(NSInteger)leftCapWidth topCapHeight:(NSInteger)topCapHeight; 

And you don’t need to use a custom UIView subclass to override the drawRect: method anymore! 


James
