---
layout: post
title: Participate on an opensource Github project, iOctocat
comments: true
share: true
category: opensource
tags:
- iOS
- development
---

I always love to know whether there are new watchers and forkers for my [Opensource][] projects, even when I'm on the go. So what I do is to use  my iPhone and browse [github.com][] using safari, __the ONLY problem__ is the page just not optimized for mobile experience.

` > There is an app for that!`

Right, the closest official app I found is the [Github Issues][], which lets me browse my own repos issues, others issues, just missing the details I wanted to know, __my activity feed__ and __forkers/watchers count__.

I tried further to see if there's any third party apps for that, and yes there are a few free ones like [GitHubby][], [GithubView][], etc, hmm... can't expect too much.

I was going to start my own Github mobile client, and went to look for some existing API wrappers. A search on the keyword "github" brought me to this. ![ioctocat](/images/2012-04-15-ioctocat-enhancement/github-screenshot.png). 

[iOctocat][1] is a paid app on App Store, yet open source and welcome contributions.  I immediately cloned it from [dennisreimann / ioctocat][] and see if it fits my needs... __Pretty close!__

It got the Activity feed I wanted to see, list of repos of a particular user, but those numbers are missing from the list view. _(YES I JUST CARE!)_

![numbers](/images/2012-04-15-ioctocat-enhancement/numbers.png)

It's __open source__ anyway, I can just patch it :) The code is clean enough for me to find where I should begin working with, so after about an hour of focused work, here I introduce my enhancement on ioctocat.

![enhanced](/images/2012-04-15-ioctocat-enhancement/ioctocat-enchanced.png)

Thanks for [Dennis Reimann] for creating this wonderful app, you can find my fork here at [mystcolor / ioctocat][], and please [support][1] it from the App Store!


### Update: 16 Apr 2012 ###
This feature has been merged to the [main repo][dennisreimann / ioctocat], so I expect everyone would see it in the next version of their app release!


James


[Opensource]:http://github.com/mystcolor
[github.com]:http://github.com
[Github Issues]:http://itunes.apple.com/hk/app/github-issues/id453833494?mt=8
[GitHubby]:http://itunes.apple.com/hk/app/githubby/id413672549?mt=8
[GithubView]:http://itunes.apple.com/hk/app/githubview/id441062536?mt=8
[1]:http://itunes.apple.com/hk/app/ioctocat/id310429782?mt=8
[dennisreimann / ioctocat]:http://dennisreimann.github.com/ioctocat/
[Dennis Reimann]:http://twitter.com/dennisreimann
[mystcolor / ioctocat]:https://github.com/mystcolor/ioctocat

