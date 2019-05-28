---
layout: page
title: Badger Maps - Design Work
permalink: /portfolio/badger-maps
---

## Badger Maps
While at Badger I designed and implemented (wrote the templating, html, css, and interaction javascript) a responsive webapp, a native iOS app, and a native Android app. I also revamped the logo, helped implement a brand identity along with another designer, created plenty of collateral, and more. Here's a little sampling.

Badger is a unique application in that its primary interface is a map. Badger ostensibly works as a light weight CRM for outside sales professionals, so being able to spatially reason with where your customers are is paramount. There are few applications out there that are able to layer on a lot of data on top of a map while still making it feel easy to use. Our customers were sales people and had zero patience for an application that felt difficult. Usability was key.

### Responsive Web Application
Early on at Badger we created an MVP that allowed people to pay for and use the application but was otherwise not thoroughly designed. This changed about two years in when I designed and implemented an interface that would allow us to have a much more coherent approach to the web application that collapsed with very, very little code to mobile. This design has carried us for four years, allowing us to adapt to new features and additions with very little trouble.

#### Webapp Evolution

Our web application started as a rough sketch but contained some devices that would end up being carried through to the final design that we work with today. While the menu and overall structure and layout were heavily altered, certain areas like the route list remained largely the same. 

{% include image.html url="/images/badger-webapp-desktop-early.png" description="Early designs were meant to rapidly expose features and didn't yet have a strong sense of organization or structure" %}

{% include image.html url="/images/badger-webapp-desktop-middle.png" description="As time permitted, we went back to the original and made it more usable on tablets by increasing touch targets. Time was also taken to solidify the design around brand colors and make the app feel more cohesive." %}

{% include image.html url="/images/badger-webapp-desktop-current.png" description="When the limits of the original design were reached, I went back to the drawing board and redesigned the app around a 'pane' metaphor, with a menu state on the left and a detail state on the right. This allowed the map to stay front and center." %}


#### Mobile metaphor
With mobile, I wanted a metaphor where each state felt straight forward to the user without having to think about it. In order to incorporate the webapp with as few modifications as possible, I came up with a way for the windows to be structured in a way that felt familiar to iOS/Android users while keeping modifications to CSS just to things like height (aside from the menu which had so many differences as to require a different component on mobile).

1. Base State (The map is the primary interaction mechanism)
2. Menu State (A menu button has been tapped. All menu items are accessible.)
3. Detail State (Account detail is being viewed, it must be closed before menu is accessible)

{% include image.html url="/images/badger-webapp-desktop-wireframe.png" description="Here is the desktop view broken down into it's main structural components. On the next image, you can see how these components collapsed for mobile." %}

{% include image.html url="/images/badger-webapp-mobile-metaphor-wireframe.png" description="The wireframe broke down the app design structure into three main states: Base, Menu Selected, and Detail. Detail is only triggered when an item inside a selected-menu view needed to expand to another view." %}

{% include image.html url="/images/badger-webapp-mobile-metaphor.png" description="Here you can see how this actually was designed in practice. " %}

### Logo
After having been at Badger for a few years, a number of things bothered me about the logo. It was originally purchased from a website similar to 99 Designs to get the job done. While conceptually very cool (combo of a Badger and map pin) and having some good bones, the logo was hastily completed and it showed. I wanted to massage the logo to get it to the point where it felt more strongly designed. 

A few goals I had:

- Make the logo look like it flowed. The curves of the current logo lacked harmony and didn't have a sense that they knew where they were going.
- Make it bolder. I wanted to be able to flip the logo to a black and white form (sans the red interior) and for it to still feel strong. With the original, the thin lines made the logo look strange and incomplete in black and white.
- Make the logo more consistent and balanced. The structure and lines of the original looked almost lopsided and had abruptly ending structures in it. The lines themselves were also not consistent widths without any reasoning to them.

{% include image.html url="/images/badger-logo-before-after.png" description="Thicker lines reduce better, curves flow in harmony, logo overall feels more 'designed'." %}

{% include image.html url="/images/badger-logo-before-after-with-points.png" description="Point reduction, simplification, and consistency makes for a technically easier to work with product." %}

{% include image.html url="/images/badger-logo-three-styles.png" description="Improvements in being able to go black and white" %}