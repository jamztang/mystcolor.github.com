---
layout: post
title: A note on how Facebook syncs user experience across platforms
comments: true
share: true
category: ux
tags:
- iOS
- ux
- User Experience
- Facebook
- UIPopoverController
---

Facebook has been one of the most popular platform on the web, and their mobile team are also working so hard to ensure everyone can have a great Facebook experience. Since the introduce of Facebook app v4.0, I think they made something worths me a second mention for their effort.



The shared navigation sidebar experience
----------------------------------------

No matter on Facebook's desktop webpage, mobile page, and the mobile apps, we see the same navigation sidebar style.

![Facebook sidebar](/images/2012-01-29-a-note-on-how-facebook-syncs-user-experience-across-platforms/facebook-web-mobile-sidebar.png)

And better yet their sidebar items syncs both ways on the mobile app and web, and you can directly edit your favourite list on v4.1 iOS mobile app.



The popover access to Friend request/Messages/Notification on v4.1
------------------------------------------------------------------

![Facebook popover](/images/2012-01-29-a-note-on-how-facebook-syncs-user-experience-across-platforms/facebook-popover.png)

If you're an iOS developer, you'd know that the [UIPopoverController][] is only available for the iPad SDK, and the Facebook mobile team took the hard path to build their own (or maybe not ;P), they still go for futher unifying the whole user experience across different platforms.

One thing to note is the those list of messages and requests on the app is cached after the first time access, (which you can try to scroll down to load the second page, and re-open the popup again to find page two doesn't need to be load again). And it would be even better if the scrolling offset could be remembered as well.



The chat list, on the same right hand side, only when there's enough screen width
---------------------------------------------------------------------------------

![Facebook chatlist](/images/2012-01-29-a-note-on-how-facebook-syncs-user-experience-across-platforms/facebook-chatlist.png)

This could matter to someone whom are serious Facebook chatter.


Conclusion
----------


The above is just the part of the features that the Facebook team offers to their users, there are more like the new [Bigger, better photos][] on the iPad app, the new [Timeline layout][] available for mobile access, etc.


I really appreciate for their work and attempt to unify all user experience, for the same service across different platform, which we could have equally good product no matter where we are.


Open Source
-----------

If you're interested on how to create the [UIPopoverController] layout on iPhone, you could check out my [iPhone compatible UIPopoverController implementation bit.ly bundle][] for some open source projects on [github.com][]

And there're also some really good list of [iOS Open Source Facebook/Path liked Sidebar Menu implementation][] also hosted on [github.com][]



Let me know if you think there's any other apps that worths some more attention, and you can also find me on twitter!


James

[UIPopoverController]:http://developer.apple.com/library/ios/#documentation/UIKit/Reference/UIPopoverController_class/Reference/Reference.html#//apple_ref/occ/cl/UIPopoverController
[iPhone compatible UIPopoverController implementation bit.ly bundle]:http://bit.ly/ytOgQD
[iOS Open Source Facebook/Path liked Sidebar Menu implementation]:http://bit.ly/t5XkS2
[github.com]:http://github.com
[Bigger, better photos]:http://www.facebook.com/notes/facebook-mobile/introducing-facebook-for-ipad/240833529299007
[Timeline layout]:http://blog.facebook.com/blog.php?post=10150408335607131

