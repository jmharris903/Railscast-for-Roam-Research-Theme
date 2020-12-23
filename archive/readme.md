# Railscast dark theme for Roam Research
This is my personal version of the classic Railscast code syntax theme that I've tweaked over the years. This version has been created to work with [Roam Research](https://roamresearch.com). 

## How to install
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

/*RR change: SIDEBAR WIDTH - Comment/un-comment this section to toggle between a 50/50 layout between the main section and the sidebar.
inspried by David Cranall https://davidcrandallwrites.com/split-screen-and-rtl-custom-css-scripts-for-roam/*/

.roam-center {
  flex-basis: 50% !important;
}

/* ----------------------------------------- */

/* RR change: SEARCHBAR - Comment/un-comment this section to make the search bar full width */ 

.rm-find-or-create-wrapper {
  flex: 0 1 100% !important;
}

/* ----------------------------------------- */

/*RR change: SEARCH RESULTS WRAPPING - Wraps text when performing an inline search with [[]] or (())*/

/* .bp3-text-overflow-ellipsis {
    text-overflow: unset;
    white-space: unset;
} */

/* ----------------------------------------- */

/*RR change: PAGE WIDTH - Un-comment the section below to maximize page width, line length, and images widths */

/* 
.roam-block-container {
  max-width: 100% !important; 
}
div.roam-center > div:first-child {
    padding-right: calc((100% - 950px) / 2) !important;
    padding-left: calc((100% - 1500px) / 2) !important;
}
.hoverparent[style^='position: relative; width: 500px;'] {
    width: 100% !important;
}
.hoverparent .react-resizable[style^='width: 500px;'] {
    width: 100% !important;
}
.react-resizable[style^='width: 580px;'], 
.react-resizable[style^='width: 720px;'] {
  width: 100% !important;
}
.hoverparent[style^="position: relative; width: 580px;"],
.hoverparent[style^="position: relative; width: 720px;"] {
  width: 100% !important;
}
*/ 

/* ----------------------------------------- */

/*RR change: SEARCH/TOOLBAR - Uncomment the following section to hide the tool bar when not in use. A great idea from @Devon. Source: https://gist.github.com/devonzuegel/f54de76cbf0c0355d93e721c89f45787;
 */

/* 
#roam-right-sidebar-content > div {
  border-bottom: none !important;
}
.check-container {
  padding-right: 4px;
}
.roam-body-main {
  height: 100% !important;
  top: 0 !important;
}
.roam-topbar {
  opacity: 0;
  transition: opacity 200ms;
  z-index: 1;
  background: none;
  width: calc(100% - 40px);
  padding: 0;
}
.roam-topbar:hover, .roam-topbar:focus-within {
  opacity: 1;
  transition: opacity 200ms;
}
#right-sidebar button {
  z-index: 100;
} 
*/

/* ----------------------------------------- */

/*RR change: SCROLLBARS - Comment/un-comment this section to toggle scrollbars on or off
inspired by @Malcolm Ocean*/

div::-webkit-scrollbar {
  width: 10px;
}
div::-webkit-scrollbar-track {
  background-color: var(--scrollbar-track) !important;
}
div::-webkit-scrollbar-thumb {
  background-color: var(--scrollbar-thumb) !important;
}

/* ----------------------------------------- */

/*RR change: BREADCRUMBS - */
/* .rm-reference-item div[style*="display: flex; flex-wrap: wrap; margin-left: 4px;"] {
    line-height: var(--breadcrumb-line-height);
    font-size: var(--breadcrumb-font-size);
    color: var(--breadcrumb-color) !important;  */
    /*RR change: Added variable for the breadcrumb navigation in reference blocks*/

/*RR change: decrease the line spacing in the breadcrumbs for referenced items*/
.zoom-mentions-view span {
padding-top: 0 !important;
padding-bottom: 0 !important;
}

/* RR change: Comment/un-comment to remove checkboxes in breadcrumb navigation */

.roam-reference-item > div:first-child:not(.roam-log-container) > div:first-child label.check-container,
.roam-article > div:first-child:not(.roam-log-container) > div:first-child label.check-container {
  display: none;
}

/* ----------------------------------------- */

/* ----------------------------------------- */
/* RR change: QUERIES - Query results options */

/* Show empty query message */
.rm-block-text .rm-reference-main .rm-mentions:empty:after {
  content: var(--no-query-results);
  color: var(--no-query-results-color);
  font-family: var(--main-font);
  padding: var(--s1);
}
.rm-query {
  /* border: 0.5px solid #38332e; */
  padding-bottom: var(--s1);
  /* border-top-left-radius: 7px;
  border-top-right-radius: 7px; */
  border-radius: 7px;
  border: 0.75px solid var(--query-results-border);
}
.rm-query .rm-query-title {
  /* color: #508bb5; */
  /* background-color: #38332e; */
  padding: var(--s1);
  font-size: .8em;
  border-top-left-radius: 7px;
  border-top-right-radius: 7px;
  background-color: var(--reference-item-bg);
  color: var(--breadcrumb-color);
}

/*RR change: HIDE QUERY SCRIPT - Comment/uncomment to hide the original query and revert back to legacy behavior */

/* 
.rm-query .rm-query-title {
  display: none;
}
 */

/* RR change: MINIMIZE QUERIES: add any one of the following tags before the beginning of your query (in the same block):

    #min-title = hides the page reference link / page title
    #min-con = hides the contextual reference information (breadcrumbs)
    #minimal = hides both the title and the context
    #min-q = hides the query string, similar to legacy behavior
    #min-all = hides everything — title, context, and query string

inspired by Matt Goldenberg */

[data-tag="minimal"], 
[data-tag="minimal"] + .rm-query .rm-title-arrow-wrapper,
[data-tag="minimal"] + .rm-query .zoom-mentions-view {
  display:none!important; /* hide page reference (title) and mention context (breadcrumbs) */
}
[data-tag="min-title"], [data-tag="min-title"] + .rm-query .rm-title-arrow-wrapper {
display:none!important; /* hide page reference (title) */
}
[data-tag="min-con"], [data-tag="min-con"] + .rm-query .zoom-mentions-view {
  display:none !important;  /* hide mention context (breadcrumbs) */
}
[data-tag="min-q"], 
[data-tag="min-q"] + .rm-query .rm-query-title {
  display:none !important;  /* hide the query string */
}
[data-tag="min-all"], 
[data-tag="min-all"] + .rm-query .zoom-mentions-view,
[data-tag="min-all"] + .rm-query .rm-title-arrow-wrapper,
[data-tag="min-all"] + .rm-query .rm-query-title {
  display:none !important;  /* hide everything */
}
[data-tag="minimal"] + .rm-query .rm-query-title::after,
[data-tag="min-title"] + .rm-query .rm-query-title::after,
[data-tag="min-con"] + .rm-query .rm-query-title::after{
  content: " #minimal" /* add a tag to the query string to indicate this query has been minimized */
}

/* ----------------------------------------- */

/*RR change: CUSTOM TAGS: Uncomment to use the section below to create custom styles for specific tags. Change "Meeting" to match some portion of the title of the tag you want to customize. Adjust the background-color value ("F00") and color value ("fff") to suite your preferences. Duplicate the section for each new tag to be customized */

/* 
span[data-tag*="Meeting"] {
  background-color: #F00;
  color: #fff;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;

}
 */


 /*RR change: CUSTOM LINKS: Uncomment to use the section below to create custom styles for specific links. Change "Theme" to match some portion of the title of the link you want to customize. Adjust the background-color value ("F00") and color value ("fff") to suite your preferences. Duplicate the section for each new link to be customized*/

/* 
span[data-link-title*="Theme"] .rm-page-ref-link-color {
  background-color: #F00;
  color: #fff;
  padding: 3px 7px;
  line-height: 2em;
  font-weight: 500;
}
 */


/* ----------------------------------------- */

/*RR change: ATTRIBUTE STYLES: Uncomment and customize this section to style all attributes */

/* .roam-block span strong[style*='cursor: pointer;'] {
    color: #f00 !important;
} */

/* ----------------------------------------- */

/*RR change: SIDEBAR IMAGE - comment/uncomment this section to add a backgound image to the sidebar - by Daniel van der Merwe*/

/* 
.roam-sidebar-container {
  overflow: hidden !important;
}
.roam-sidebar-container.noselect:before {
  background-image: url(https://images.unsplash.com/photo-1589809489704-71becdce06f0?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=634&q=80);
  width: 100%;
  height: 100%;
  content: "";
  position: absolute;
  background-repeat: no-repeat;
  background-position: 75% 40%;
  top: 0;
  bottom: 0;
  z-index: -1;
  opacity: 0.3;
  filter: blur(4px);
}
 */


/* ----------------------------------------- */

/*RR change: DEFAULT TEXT - a small addition to the placeholder text to Daily Notes or Pages to help get you started */
div#block-input-ghost span:before {
  content: "Cmd+enter or ";
}

/* ----------------------------------------- */

.roam-article div {
  font-family: var(--main-font);
}

/* ----------------------------------------- */

/*RR change: POMODORO - Comment/un-comment this section to apply custom styling to the the Pomodoro timer */
/* ------------- Red Pomodoro ------------- */
.rm-pomodoro {
  background: var(--reference-item-bg) !important;
  color: #FC5963 !important;
  padding: 2px 12px;
  line-height: 1.7em;
  font-weight: 600;
  border-radius: 2em;
  border: 1px solid #FC596370;
}

.rm-pomodoro::first-letter {
  margin-right: 4px;
}

/* ----------------------------------------- */

.rm-reference-container span[style*="color: red;"] {
    color: var(--main-font-color) !important;
}
/* ----------------------------------------- */

```

## Other great themes worth checking out
https://github.com/vandermerwed/Roam-Research-Dark

https://github.com/apg-dev/roam-theme-bear

https://www.roamtips.com/home/roam-research-css-styles
