---
layout: page
title: Badger Maps Responsive Webapp Design
excerpt: How we designed and built a responsive webapp
permalink: /portfolio/badger-maps/badger-maps-responsive-webapp/
featured-image: images/badger-webapp-desktop-current.png
---

Designing responsive web applications is absurdly difficult. Do you fluidly adapt? Do you use certain breakpoints? What things do you throw away, and which do you keep? Lets say the core of your experience is a map. How do you keep that map available/surfaceable easily by the user?

I managed to come up with a solution that kept almost all of our templates/components intact while adapting them for mobile at a single breakpoint. Once implemented, it immediately offered a mobile solution across all devices that, while not quite at the level of native, was pretty dang good.

This design has held strong for 4 years, remaining intuitive and allowing us to add features easily.

Let's dig in.

## The Metaphor

I wanted a simple structure on desktop that I could easily adapt down to the mobile level. 

I decided that there were four things I really had to worry about:
- The Menu
- The Map
- The Menu Details (ie what is exposed when you click on a menu button)
- The Account Details

On desktop, I had the room to have a beefier menu, but on mobile I didn't. So I decided that I'd likely have to toss the menu and recreate it for mobile since the differences would be so stark. However, the rest of it I could re-use if I could wrap my head around it.

I decided to use a 'pane' metaphor, where each pane would be more or less the width of a cell phone. The menu details would be a pane, and the account details would be a pane. This would mean I could re-use the panes on mobile very easily by setting all their element widths to 100% (plus a few other tweaks)

Here's what it looks like on Desktop:

{% include image.html url="/images/badger-webapp-desktop-wireframe.png" description="Here is the desktop view broken down into it's main structural components." %}

{% include image.html url="/images/badger-webapp-desktop-current.png" description="And this is what the desktop version looks like fully designed" %}

On desktop this is a normal workflow:
1. Base State (The map and the menu are the primary interaction mechanisms)
2. Menu State (A menu button has been tapped. All menu items are accessible.)
3. Detail State (Account detail is being viewed, but menu and menu-detail is still accessible)

And here's how it collapses down for mobile:

{% include image.html url="/images/badger-webapp-mobile-metaphor-wireframe.png" description="The wireframe broke down the app design structure into three main states: Base, Menu Selected, and Detail. Detail is only triggered when an item inside a selected-menu view needed to expand to another view." %}

{% include image.html url="/images/badger-webapp-mobile-metaphor.png" description="And now the mobile structure in practice" %}

On mobile, things collapse like this:
1. Base State (The map and the menu are the primary interaction mechanisms)
2. Menu State (A menu button has been tapped. All menu items are still accessible but the map isn't any longer)
3. Detail State (Account detail is being viewed, it must be closed before menu is accessible again)

Once I understood the mechanics, collapsing things down to the mobile state via CSS was absurdly simple and the number of tweaks via CSS almost felt too easy. 


## Webapp Feature Dive

Let's do a quick dive into a single feature just to get a sense of what I was going for with a particular part of the app.

Of all the areas of the app that people interact with, the route list is easily the most complex. There are tons of buttons and things you can adjust. Lets break down all the potential chrome on the route pane:

- Enter start location
- Adjust start time
- Manually re-order route list
- Change an appointment to a fixed time
- Change an appointment's meeting length
- Remove an appointment
- Enter end location
- Optimize the route
- Save the route
- Clear the route
- Add a location to the route from your accounts
- Add a single-use location where you won't need check-ins, etc
- Reverse the route
- Export the route to PDF, Calendar, GPX

*PHEW!*

But we don't need to do that all at once!

One thing I really wanted to focus on, especially for new users, was creating a single point of entry for the route list. Could we make it so people could just click a single button to access everything they might need? 

I think we can.

Let's check out what that looks like in practice:

{% include image.html url="/images/badger-webapp-routes.png" description="The routes base-state invites you to get going and provides an insanely simple point-of-entry: a single button" %}

{% include image.html url="/images/badger-webapp-route-add.png" description="Tapping the button reveals a simple popover-like interface that is easy to quickly select accounts from" %}

{% include image.html url="/images/badger-webapp-route-filled.png" description="Once the route is filled, you are presented with many more options like adjusting the duration, time, and stop-order of the route." %}

Now, most users might only use a subset of the available features in the route list. But by boiling everything down to a single point of entry, the path forward feels easy and clear. Further, the design is forgiving. Removing, re-adding, and interacting with the route list through a single button is insanely easy and fluid behavior. 

## Webapp History

Here's an interesting walk down history lane. When we first started, we honestly had no idea what we were building. This category didn't really exist and very few people were building software for outside sales people. You can visually get a sense of how we evolved, slowly understanding the feature sets we'd need. 

You can also see me working though the difficulties of designing around a map. Most applications do it poorly, and of all the things I've done at Badger I'm most proud of how we've layered data on top of the map and made it center stage. 

{% include image.html url="/images/badger-webapp-desktop-early.png" description="Early designs were meant to rapidly expose features and didn't yet have a strong sense of organization or structure" %}

{% include image.html url="/images/badger-webapp-desktop-middle.png" description="As time permitted, we went back to the original and made it more usable on tablets by increasing touch targets. Time was also taken to solidify the design around brand colors and make the app feel more cohesive." %}

{% include image.html url="/images/badger-webapp-desktop-current.png" description="When the limits of the original design were reached, I went back to the drawing board and redesigned the app around a 'pane' metaphor, with a menu state on the left and a detail state on the right. This allowed the map to stay front and center." %}