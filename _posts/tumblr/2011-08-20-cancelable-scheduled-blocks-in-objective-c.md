--- 
layout: post
title: Cancelable Scheduled Blocks in Objective-C
comments: true
share: true
category: ioscodesnippet
tags: 
- blocks
- cancelable scheduled block
- category
- iOS
- nsobject
- nsoperation
- objective-c
- ioscodesnippet
---

Sometimes you'd really want to perform a delayed action for your apps. We'll create a category on NSObject to provide a really handy usage.

The best thing with this snippet is your scheduled operations are cancelable, so you can choose to only perform your latest triggered operation (e.g. for your table view cells maybe?)

    
<script src="https://gist.github.com/1571800.js?file=NSObject%2BJTCancelableScheduledBlock.h"> </script>
<script src="https://gist.github.com/1571800.js?file=NSObject%2BJTCancelableScheduledBlock.m"> </script>


Usage:

    
    
    [self performBlock:^(void) {
         NSLog(@"delayed operation!");
    } afterDelay:2];
    

  
Handy right?

  
  

You may also interest about how others doing in alternative ways.

[Delayed Blocks in Objective-C](http://forrst.com/posts/Delayed_Blocks_in_Objective_C-0Fn)

[Easy Delayed Messaging using NSProxy and NSInvocation](http://atastypixel.com/blog/easy-delayed-messaging-using-nsproxy-and-nsinvocation/)

