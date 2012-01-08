--- 
layout: post
title: NSStringf. Simpler printf styled +[NSString stringWithFormat:]
category: ioscodesnippet
comments: true
share: true
tags: 
- ioscodesnippet
- NSString
- printf
- NSLog
- iOS
- tutorial
- cocoa
- objective-c
---
If you thinks that +[NSString stringWithFormat:] is simply annoying.

If you missed the C style string formatter like printf() or NSLog().

[NSString stringWithFormat:@"Why should I type this long?"];

<script src="https://gist.github.com/1578509.js?file=JTStringAddition.h"> </script>    
<script src="https://gist.github.com/1578509.js?file=JTStringAddition.m"> </script>
  
NSStringf(@"It's just so much easier. %@", @"Really.");

