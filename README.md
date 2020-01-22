# AngularStorybook

This sample project goal is to reproduce an issue with storybook for debug purpose.

Run `npm run storybook` or `yarn storybook` to start a local storybook.

Only one story is defined : `testbootstrap.stories.mdx`

The goal of this story is to display a themable component (here, 2 divs) using $primary and $secondary bootstrap variable.

## Testbootstrapcomponent

A basic themable component, with 2 div with 3 sets of colors :
- bootstrap default : blue & grey
- default theme: green & yellow
- theme loaded by storybook : red & orange

## Problem

Case 1 (bootstrap default) and 2 (default theme) are working correctly.
But, I can't surcharge the theme using scss inline loader (defined in preset.js)

## Expected behavior: 

scss-loader.scss is taken in account during sass compilation (variable are used and available in component), story display component in red & orange.