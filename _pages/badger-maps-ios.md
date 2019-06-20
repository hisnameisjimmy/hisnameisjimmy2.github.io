---
layout: page
title: Badger Maps iOS Design
excerpt: The history of iOS design at Badger
permalink: /portfolio/badger-maps/badger-maps-ios/
featured-image: images/badger-ios-screens.png
---

iOS is our most important client, period. It's been incredible getting feedback and realizing that, given the option, all of our customers would rather never use their computers. 

We have thousands of customers using it every day. It brings in a little less than half of our trial signups. It's incredibly important that it be easy to use, bug free, and a pleasant experience. 

{% include image.html url="/images/badger-ios-screens.png" description="The most consequential screens on iOS" %}

## Route Mode

Certain screens like route-mode deserve more explanation. When our customers built optimized routes, they almost had an experience of 'now what?'. They didn't know how to actually navigate the route. One of our sales reps said the equivalent of "It would be really nice if there was just some sort of 'GO' button". I felt like that was genius! This was especially true because our app packs in a lot of options, and the route creation screen essentially has the most options of any screen.

{% include image.html url="/images/badger-ios-route-list.png" description="Our route creation screen feels a bit complicated, and includes a lot of information that's unnecessary once you are actually executing your day" %}

Route mode essentially splits our app in two, conceptually. 
- Planning Mode: Where you are finding customers, adding them to a route, optimizing it, and then saving it
- Execution Mode: Where you really just want to execute your route, create check-ins, and navigate

I wanted route mode to feel like a different experience. I wanted to eliminate distractions for the end user. What really mattered when you were done planning? 

Not much:
- Viewing account detail
- Creating a check-in
- Navigating to the location

So that's what we did. We put a big GO button below the route you were creating, and when you tapped it the rest of the app fell away. 

{% include image.html url="/images/badger-ios-route-mode.png" description="Once you're in route mode, everything else melts away" %}

It makes the app feel obvious, helpful, and a pleasure to use. This was such a big deal that, before we built a native app for Android and we had users switch from iOS to Android, they complained *loudly* about the lack of 'route mode'.

## History

Just some fun history here. When I originally designed the iOS app we were pre-iOS 7, which means that things hadn't flattened out yet. The heavy use of gradients kinda gives it away.

The original assumptions were made on an iPhone 4 (maybe 4s??), where screen real-estate was *extremely* limited. This led to a lot of companies, including ours, hiding other views behind a hamburger/menu button. Luckily, future generations of the iPhone increased screen real-estate substantially and allowed designers to add the tab-bar back in, increasing usability enormously.

You can also see a transition from using purchased stock icons to custom icons that I made for iOS. 

Another couple interesting things to note here:
- Stock icons in earlier versions vs a custom set I designed
- We didn't even have our core value proposition in the first version! A major customer who was paying for us to build the iPhone client really just wanted check-ins to their accounts and didn't care about route optimization.

{% include image.html url="/images/badger-ios-transition.png" description="Our iOS app through the sands of time (or iOS versions, if you will)" %}