--- 
layout: post
title: Loading a Nib file programmatically using NSObject category
category: ioscodesnippet
comments: true
share: true
tags: 
- UITableViewCell
- UIView
- category
- iOS
- loading nib file programmatically
- nib
- nsobject
- objective-c
- xib
- isocodesnippet
---
Maybe you've an IB created uitableviewcell.xib, or some kind of uiview.xib
wanted to load to your code-based view controller, and you come out finding
it's not that straight forward just to do this simple job according to the
official [Resource Programming Guide](http://developer.apple.com/library/ios/#
documentation/Cocoa/Conceptual/LoadingResources/CocoaNibs/CocoaNibs.html)

Isn't it ideal to load a nib file using one line like

    
    MyTableViewCell *cell = [MyTableViewCell objectWithNibNamed:@"MyTableViewCellNibName"];
    

  

Add this NSObject category make this possible

<script src="https://gist.github.com/1578429.js?file=NSObject%2BJTNibLoader.h"> </script>
<script src="https://gist.github.com/1578429.js?file=NSObject%2BJTNibLoader.m"> </script>

  
Easy enough?

