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

At the top of the CSS file is a set of variables you can use to customize the theme. Just change the color values to suit your preference.

Below is an example of the variables available for customizing the theme.

**Note: this is not the entire style sheet, just a snippet that contains the variables. The entire CSS file can be found [here](https://github.com/jmharris903/Railscast-for-Roam-Research/blob/master/RailsRoam.css).**

```
/* RR change: added variables to easily change the theme */
:root {
  /* Roam default variables */
  --primary-color: #137cbd;
  --s1: 8px;
  --background-color: #e1e8ed;

  /* Primary fonts */
  --main-font: 'Inter', sans-serif;
  --main-font-color:#999;
  --main-font-size: 1.0em;
  --code-font: 'Source Code Pro', 'Courier New', Courier, monospace;
  --code-font-color: #6d9cbe;
  --code-font-size: 1.0em;

  /* font colors */
  --page-link-color: #eb9854;
  --daily-notes-link-color:#eb9854;
  --external-link-color: #8DBB40;
  --sidebar-link-color: #8DBB40;
  --page-brackets: rgba(228, 124, 67, 0.25);
  --h1-font-color: #1189BD;
  --h2-font-color: #1189BD;
  --h3-font-color: #1189BD;
  --strong: #508BB5;
  --emphasis: #FC5963;
  --tag-font-color: #777;
  --tag-font-color-hover:#fff;
  --tag-hover-bg:#e98924;
  --sidebar-font-color: #1189BD;
  --sidebar-font-color-hover:#e98924;
  --sidebar-hover-bg:#1f1f1f;
  --block-ref-bg: none;
  --block-ref-border: rgba(254, 207, 43, .6);
  --block-ref-hover: #eb9854;
  --block-ref-hover-bg:#111;
  --block-ref-font-size: 1.0em;
  --highlight-font-color: #222;
  --highlight-background-color: #fef09f;
  --highlight-link-color: #ff6000;
  --search-font-color: #af671c;
  --search-body-font-color: #8a9ba8;
  --new-page-color: #8DBB40;
  --popover-font-color: #e98924;
  --ref-count-font-size: 12px;
  --breadcrumb-color: #5c7080;
  --breadcrumb-font-size: 13px;
  --breadcrumb-line-height: 0.85em;

  /* Saving icon colors */
  --saving-local: #99280f;
  --saving-remote: #d9822b;
  --synched: #0f9960;

  /* backgrounds and outlines */
  --body-bg: #232323;
  --left-sidebar-bg: #2b2b2b;
  --right-sidebar-bg: #2b2b2b;
  --icon-color: #e78924;
  --icon-bg-hover: rgba(167,182,194,0.3);
  --icon-color-hover: #e78924;
  /* --h1-bg: #1189BD1a; */
  --hr: rgba(225, 117, 28, 0.50);
  --code-bg: #333;
  --checkmark-color: #137cbd;
  --pages-row-highlight: #292929;
  --pages-header-row: #2d2d2d;
  --reference-item-bg: #f2c98f1a;
  --bullet: rgba(225, 117, 28, 0.30);
  --bullet-closed: rgba(225, 117, 28, 0.70);
  --bullet-outline: #404040;
  --bullet-position: 4px;
  --block-highlight: #00588e;
  --block-highlight-bg: rgba(0, 0, 0, 0.4);
  --current-block-highlight: rgba(255, 255, 255, 0.05);
  --search-outline: #e9892475;
  --search-bg: #252525;
  --search-selected-row: #4c4c4c;
  --inline-search-bg: #333;
  --popover-bg:#333;
  --select-bg:#444;
  --datepicker-bg: transparent;
  --datepicker-day-wrapper: #d9822b7a;

  /* fragile styles that may break with the next update */
  --block-embed-bg: #3f3f3f;
  --block-embed-font-size: 0.85em;
  --alias-font-color: #FECF2B;
  --alias-bg: transparent;
  /*RR change: no longer needed? Already broken?*/
  /* --filter-bg-subtract: rgba(228, 33, 35, 0.6);
  --filter-bg-add: rgba(141, 187, 64, 0.5); */

  /* Misc */
  --kanban-board-bg: #333333;
  --kanban-column-bg: #454545;
  --kanban-card-bg: #555555;
  --kanban-column-font-color: #e98924;
  --kanban-card-font-color: #6d9cbe;

  --table-border: #444;

  --blockquote-font-color: rgba(109, 156, 190, 0.89);
  --blockquote-border-color: #444;
  --blockquote-bg: none;
  --blockquote-cite: #777;

  --encrypted-font-color:#ff6000;
  --encrypted-bg:#353535;

  --emoji-bg: #2d2d2d;
  --emoji-border: rgba(225, 117, 28, 0.40);
  --emoji-color: #aaa;

  --no-query-results: "Query returned no results";
  --no-query-results-color: #FC5963;
  --query-results-border: #f2c98f1a;

  /* Scrollbar settings - to disable set values to none */
  --scrollbar-track: #2b2b2b;
  --scrollbar-thumb: rgba(153, 153, 153, 0.1);

  /* JH overrides */
  /* --main-font: 'Calendas Plus', serif;
  --main-font-size: 16px;
  --code-font-size: 0.9em;
  */

}

/* ----------------------------------------- */

/*RR change: CHECKBOX ALGINMENT - adjust the 'top' value to move the checkbox up or down to better align with the font selected above - the default font Inter uses -6px*/
.check-container {
  top: -6px;
  padding-right: 4px;
}

/* ----------------------------------------- */

/* JH overrides for Calendas font*/
/*
.check-container {
  top: -10px;
}
.rm-reference-item div.rm-block-text{
  font-size: 16px;
}
#right-sidebar .rm-reference-item div[style*="display: flex;"] {

}

.roam-block div[style*="background-color: rgb(235, 241, 245);" ],
.roam-block div[style*="background-color: rgb(235, 241, 245);" ] div {
  font-size: 0.8em;
  font-size: 16px;
}
.rm-reference-item textarea {
  font-size: 16px;
}
*/

/* ----------------------------------------- */



/* RR change: MINIMIZE QUERIES: add any one of the following tags before the beginning of your query (in the same block):

    #min-title = hides the page reference link / page title
    #min-con = hides the contextual reference information (breadcrumbs)
    #minimal = hides both the title and the context
    #min-q = hides the query string, similar to legacy behavior
    #min-all = hides everything — title, context, and query string



```

## Other great themes worth checking out

https://github.com/vandermerwed/Roam-Research-Dark

https://github.com/apg-dev/roam-theme-bear

https://www.roamtips.com/home/roam-research-css-styles
