---
layout: post
title: 4 Tips on asking users to rate your app
comments: true
share: true
category: ux
tags:
- iOS
- ux
- Rating
- tips
---

![Ratings](/images/2012-03-22-tips-on-asking-user-to-rate-your-app/rating.png)

While an app having a good rating on app store helps promotes the number of downloads, some developers have been pushing too hard or making some mistakes that make their users have less incentive to rate their apps. Here's some tips for it.


- **Never blocks the users work-flow.** If you're putting any alert box on app launch, while some libraries like [iRate][], [Appirator][] make this insanely easy, I'd still recommend you to disable the app launch event. When I'm getting things done with your app, you know I'd click "No, thanks".

    _Try to ask after the user accomplished some task after a few times, like if your app is a photo processing app, ask them after they finished saving the photo._


- **Understand how the app has been used.** Ask your users directly and collect some data.

    _Check the end point of your app using analytics tools, such as [Flurry][].  your app and by keeping the first point in mind, add to some critical flow which users actually reach._


- **Your users know when is the best time for them to give some credits.** Make sure you have an explict button for them to have easy access to the rate system, the official way is just too cumbersome of anyone.

    _[Juhani][] stated some pretty good suggestions on how to gently remind your users to rate your app at [How to Ask Users to Rate Your App?][].


- **The most important thing - Make your app awesome.**
 
    _Remember after your users has rated your app, they are more easy to change their mind and drop a one star rating. Make your app awesome is always the key to win your users heart._


James

[How to Ask Users to Rate Your App?]:http://www.androiduipatterns.com/2012/02/how-to-ask-users-to-rate-your-app.html
[iRate]:https://github.com/nicklockwood/iRate
[Appirator]:https://github.com/arashpayan/appirater
[Flurry]:http://www.flurry.com/
[Juhani]:http://twitter.com/lehtimaeki

