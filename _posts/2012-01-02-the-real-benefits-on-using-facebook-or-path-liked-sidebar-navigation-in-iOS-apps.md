---
layout: post
title: The real benefits on using Facebook/Path liked sidebar navigation in iOS apps
comments: true
---

![Path and Facebook](/images/2012-01-02-the-real-benefits-on-using-facebook-or-path-liked-sidebar-navigation-in-iOS-apps/path_facebook.png)

We don't have an official name for it, so I will called it the "Sidebar" at this moment.


The "Sidebar" navigation isn't something that provided by the official SDK. Is it worth to spend time and effort to follow this trend and forget about common solutions, like the UITabBar or the old Facebook style dashboard launcher?


Before, we already have similar discussions as the [iPhone App: Tab Bar vs. Dashboard (aka Grid Navigation). Or both?][] thread, and now the "Sidebar" is definately a new player.

First, let us have a quick remind on the original UITabBar and the Facebook dashboard launcher.


UITabBar
--------

![UITabBar in Music app](/images/2012-01-02-the-real-benefits-on-using-facebook-or-path-liked-sidebar-navigation-in-iOS-apps/music.png)

The problem of using the UITabBar is that it's always there no matter the user needs it or not, which is waste of screen pixels especially on the iPhone and the iPod touch.

Another property is that assigning more than 5 view controllers to the UITabBarController would collapse the last tab into a "More" tab, which some may think it complicates the application hierachy.


Dashboard Launcher (Facebook app)
---------------------------------

![Old Facebook](/images/2012-01-02-the-real-benefits-on-using-facebook-or-path-liked-sidebar-navigation-in-iOS-apps/facebook.jpg)

Using the dashboard, we gain back the precious screen spaces while the dashboard is only there when the app launches or until the user returns back to the main page.

However, some suggested it could still be insufficient even we got 9 icons at a page, and once it requires user to swipe between pages, it is not really much better than comparing with the "More" tab.


Why using the "Sidebar"?
----------------------

Unlike the above approaches, that users would expect as simple as to see a new view controller, the "Sidebar" can provide a lot more info while presenting list of options, including pushing a new view controller, categories, browsing submenus, and even custom user actions, etc.


![Facebook Sidebar Navigation](/images/2012-01-02-the-real-benefits-on-using-facebook-or-path-liked-sidebar-navigation-in-iOS-apps/facebook_sidebar_navigation.png)
![Path Sidebar Actino](/images/2012-01-02-the-real-benefits-on-using-facebook-or-path-liked-sidebar-navigation-in-iOS-apps/path_sidebar_action.png)


Consider the flexibility on using the "Sidebar", custom accessory view, selected indexPath indication, section header and footer for descriptions, basically all goodies from using a UITableView.


Conclusion
----------

The default UITabBar is definately good for situation that the tab bar is needed to be always there. But if you think you needed more screen estate, maybe you'd now really consider using the "Sidebar" for navigation.


Open Source
-----------

Since we don't have an official implementation for it, maybe you'd like to checkout the few open source library on Github that aimed to provide this function, including my own implementation [JTRevealSidebarV2][] or others good work in [my bit.ly bundle][].


Let me know what you think!

James

[iPhone App: Tab Bar vs. Dashboard (aka Grid Navigation). Or both?]:http://ux.stackexchange.com/questions/6584/iphone-app-tab-bar-vs-dashboard-aka-grid-navigation-or-both
[JTRevealSidebarV2]:http://bitly.com/uOeTc0
[my bit.ly bundle]:http://bitly.com/t5XkS2

