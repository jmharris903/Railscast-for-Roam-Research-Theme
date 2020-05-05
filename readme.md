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
  /* Primary fonts */
  --main-font: 'Inter', sans-serif;
  --main-font-color:#999;
  --main-font-size: 1.0em;
  --code-font: 'Source Code Pro', 'Courier New', Courier, monospace;
  --code-font-color: #6d9cbe;
  
  /* font colors */
  --page-link-color: #eb9854;
  --external-link-color: #8DBB40;
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
  --block-ref-border: #FECF2B;
  --block-ref-hover: #e98924;
  --block-ref-hover-bg:#111;
  --block-ref-font-size: 1.0em;
  --new-page-color: #8DBB40;
  --highlight-font-color: #222;
  --highlight-background-color: #fef09f;
  --highlight-link-color: #ff6000;
  --search-font-color: #e98924;
  --ref-count-font-size: 12px;
  --breadcrumb-color: #5c7080;
  --breadcrumb-font-size: 13px;
  --breadcrumb-line-height: 0.85em;
  
  /* backgrounds and outlines */
  --body-bg: #232323;
  --left-sidebar-bg: #2b2b2b;
  --right-sidebar-bg: #2b2b2b;
  --icon-color: #e78924;
  --icon-bg-hover: rgba(167,182,194,0.3);
  --icon-color-hover: #e78924;
  --h1-bg: #2f2d2a;
  --hr: rgba(225, 117, 28, 0.50);
  --code-bg: #2b2b2b;
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
  --current-block-highlight: rgba(255, 255, 255, 0.07);
  --search-outline: #e9892475;
  --search-bg: #252525;
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

  /* JH overrides */
  /* --main-font: 'Calendas Plus', serif;
  --main-font-size: 1.2rem; 
  */
  
}
.check-container {
  top: -6px; /*RR change: adjust this value to move the checkbox up or down to better align with the font selected above - the default font Inter uses -6px*/
  padding-right: 4px;
}

/* JH overrides for Calendas font*/
/* 
.check-container {
  top: -10px;
}
rm-reference-item div.rm-block-text{
  font-size: 16px;
}
#right-sidebar .rm-reference-item div[style*="display: flex;"] {
  font-size: .90em;
}
*/

/* ----------------------------------------- */

/*RR change: Wraps text when performing an inline search with [[]] or (())*/

/* .bp3-text-overflow-ellipsis {
    text-overflow: unset;
    white-space: unset;
} */

/* ----------------------------------------- */

/*RR change: Un-comment the section below to maximize page width, line length, and images */

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
.react-resizable[style^='width: 580px;'] {
  width: 100% !important;
}
.hoverparent[style^="position: relative; width: 580px;"] {
  width: 100% !important;
}
*/ 

/* ----------------------------------------- */

/*RR change: Uncomment the following section to hide the tool bar when not in use. A great idea from @Devon. Source: https://gist.github.com/devonzuegel/f54de76cbf0c0355d93e721c89f45787;
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

```

## Other great themes worth checking out
https://github.com/vandermerwed/Roam-Research-Dark

https://github.com/apg-dev/roam-theme-bear
