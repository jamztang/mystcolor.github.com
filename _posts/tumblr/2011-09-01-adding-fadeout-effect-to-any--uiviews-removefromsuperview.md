--- 
layout: post
title: Adding fadeout effect to any -[UIViews removeFromSuperview]
tags: 
- ioscodesnippet
- objective-c
- UIView
- fadeout
- removeFromSuperview
- tutorial
---
Typically you like to do something like below when you wanted to remove a view
from its parent view.

    
    [myView removeFromSuperview];
    

  
Sometimes it's not that please for a user to see an UI component disappearing
suddenly. You'd then consider adding some transition effects, and here's a
little code snippet in the UIView+JTRemoveAnimated category for how you can
get a fade out effect on view removal.

    
    //
    //  UIView+JTRemoveAnimated.h
    //
    //  Created by james on 9/1/11.
    //  [http://ioscodesnippet.tumblr.com/](http://ioscodesnippet.tumblr.com/)
    //
    @interface UIView (JTRemoveAnimated)
    
    - (void)removeFromSuperviewAnimated;
    
    @end
    
    
    //
    //  UIView+JTRemoveAnimated.m
    //
    //  Created by james on 9/1/11.
    //  [http://ioscodesnippet.tumblr.com/](http://ioscodesnippet.tumblr.com/)
    //
    #import <QuartzCore/QuartzCore.h>
    
    @implementation UIView (JTRemoveAnimated)
    
    // remove static analyser warnings
    #ifndef __clang_analyzer__
    
    - (void)animationDidStop:(NSString *)animationID finished:(NSNumber *)finished context:(void *)context {
        if ([animationID isEqualToString:@"fadeout"]) {
            // Restore the opacity
            CGFloat originalOpacity = [(NSNumber *)context floatValue];
            self.layer.opacity = originalOpacity;
            [self removeFromSuperview];
            [(NSNumber *)context release];
        }
    }
    
    - (void)removeFromSuperviewAnimated {
        [UIView beginAnimations:@"fadeout" context:[[NSNumber numberWithFloat:self.layer.opacity] retain]];
        [UIView setAnimationDuration:0.3];
        [UIView setAnimationDidStopSelector:@selector(animationDidStop:finished:context:)];
        [UIView setAnimationDelegate:self];
        self.layer.opacity = 0;
        [UIView commitAnimations];
    }
    
    #endif
    
    @end
    

  

So from now on, you just needed to do this to fade out any UIViews

    
    [myView removeFromSuperviewAnimated]

