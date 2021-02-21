# Railscast dark theme for Roam Research

This is my personal version of the classic Railscast code syntax theme that I've tweaked over the years. This version has been created to work with [Roam Research](https://roamresearch.com).

## How to install

1. In Roam, create a page called `roam/css` (all lowercase)
2. Create a code block using ` ``` `
3. Paste in the following into the code block
   `@import url('https://jmharris903.github.io/Railscast-for-Roam-Research-Theme/RailsRoam.css');`

4. Then change the menu option to `css`

Other ways to install

Install either [Stylus](https://add0n.com/stylus.html) or [Roam Toolkit](https://chrome.google.com/webstore/detail/roam-toolkit/ebckolanhdjilblnkcgcgifaikppnhba). Then copy and paste the contents of the [RailsRoam.css](https://github.com/jmharris903/Railscast-for-Roam-Research/blob/master/RailsRoam.css) file into the appropriate location for the method you choose.

## Screenshot

![screenshot](https://github.com/jmharris903/Railscast-for-Roam-Research/blob/master/Rails%20Roam%20Screenshot.jpg)

The pictured version uses the beautiful serif font [Calendas Plus](http://atipofoundry.com/fonts/calendas-plus) by Atipo Type Foundry. I have no affiliation, but support them and buy the font. You'll thank yourself later.

The monospaced font is [Source Code Pro](https://github.com/adobe-fonts/source-code-pro)

## Customization

At the top of the [CSS file](https://github.com/jmharris903/Railscast-for-Roam-Research/blob/master/RailsRoam.css) is a set of variables you can use to customize the theme. Just change the color values to suit your preference.

Roam Railscast includes native support for the following optional add-on features:

**Masonry** by @shawnpmurphy8 and @AbhayPrasanna based on the original version by @vandermerwed

Note: For compatibility, the orignal Masonry had to be edited slightly. To work with Railscast, you must use the version below

`@import url('https://jmharris903.github.io/Railscast-for-Roam-Research-Theme/features/masonry-main.css');`

**Bullet Zoom Focus** by @jeffharrissays

When zoomed in on a bullet add the tag #.rm-focus to the parent block to create a minimal writing environment. This only works when zoomed in so there is no need to remove the tag when done.

`@import url('https://jmharris903.github.io/Railscast-for-Roam-Research-Theme/features/bullet-zoom-focus.css');`

### Built in features include

```
/* MINIMIZE QUERIES: add any one of the following tags before the beginning of your query (in the same block):

    #min-title = hides the page reference link / page title
    #min-con = hides the contextual reference information (breadcrumbs)
    #minimal = hides both the title and the context
    #min-q = hides the query string, similar to legacy behavior
    #min-all = hides everything — title, context, and query string
*/



/*  Block Callouts
    Use special tags to create colored callout blocks
    #.rm-block--grey will callout the entire block, including children
    #.rm-self--grey will only callout the block the tag is added to
    #.rm-child--grey will callout the children of the block the tag is added to

    Available colors
    --grey
    --blue
    --red
    --orange
    --yellow
*/



/* Page Date Link
  A fun little feature to change the color of dates to match the seasons, organized by quarter
*/

:root {
  /* Seasonal colors for date links */
  --page-link-date__color_q1: #50b2c0;
  --page-link-date__color_q2: #c5d86d;
  --page-link-date__color_q3: #ff6b6b;
  --page-link-date__color_q4: #ca7d4a;
}



/* Outline Highlight
  Highlights where the curser is currently in the outline and highlights the currently active block using the rm-multibar
*/



/* Full Width Search
  Changes the search bar to be full screen width all the time, no animations
*/

```

## Other great themes worth checking out

https://github.com/vandermerwed/Roam-Research-Dark

https://github.com/apg-dev/roam-theme-bear

https://www.roamtips.com/home/roam-research-css-styles
