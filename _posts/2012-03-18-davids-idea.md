---
layout: post
title: Pop-Under and Powerslide in iOS
comments: true
share: true
category: ux
---

> [Please Steal My Ideas][]

A blog post by [David][] contains a nice video demonstration on their Wikipedia app built in 2010 (which they've abandoned it), showing off two UX ideas including __Pop-Under__ and __Powerslide__.

Using the technique of __Pop-Under__ to avoid moving users away from current context while browsing external links is indeed a good solution, the same concept is exactly indential to the __Folder__ pattern officially introduced by Apple which used to categorize apps at homescreen into folders. An open source project [jwilling / JWFolders][] on [Github][] has been out for a while to imitate SpringBoard's "folders".

I agreed the one finger horizontal reveal gesture (liked the Path/Sparrow for iOS app) could be easily activated by scrolling through content vertically without intend. But I am afraid the __Powerslide__ which required two fingers horizontal sliding doesn't really work for one hand navigation while you're on-the-go, and it's even harder to discover. Navigation bar only panning gesture recognition like the Facebook app could do the job, or we can simply steeper the panning gesture degree range like under 30 degrees down from which the author mentioned 45 degrees, I think that could be enough to reduce accidental activations. 

Just note that there's nothing against David, but because I loved to discuss things :).

[Please Steal My Ideas]:http://appcubby.com/blog/please-steal-my-ideas/
[David]:http://twitter.com/drbarnard
[jwilling / JWFolders]:https://github.com/jwilling/JWFolders
[Github]:http://www.github.com
