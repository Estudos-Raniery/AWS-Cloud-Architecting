<!DOCTYPE html>
<!-- saved from url=(0089)https://labs.vocareum.com/web/1964919/3231443.0/ASNLIB/public/docs/lang/en_us/README.html -->
<html foxified=""><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta name="viewport" content="width=device-width initial-scale=1">

<link href="./Guided Lab Creating an Amazon RDS Database_files/all.css" rel="stylesheet" type="text/css"><style type="text/css">html {overflow-x: initial !important;}:root { --bg-color: #ffffff; --text-color: #333333; --select-text-bg-color: #B5D6FC; --select-text-font-color: auto; --monospace: "Lucida Console",Consolas,"Courier",monospace; --title-bar-height: 20px; }
.mac-os-11 { --title-bar-height: 28px; }
html { font-size: 14px; background-color: var(--bg-color); color: var(--text-color); font-family: "Helvetica Neue", Helvetica, Arial, sans-serif; -webkit-font-smoothing: antialiased; }
body { margin: 0px; padding: 0px; height: auto; inset: 0px; font-size: 1rem; line-height: 1.42857143; overflow-x: hidden; background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; tab-size: 4; background-position: inherit; background-repeat: inherit; }
iframe { margin: auto; }
a.url { word-break: break-all; }
a:active, a:hover { outline: 0px; }
.in-text-selection, ::selection { text-shadow: none; background: var(--select-text-bg-color); color: var(--select-text-font-color); }
#write { margin: 0px auto; height: auto; width: inherit; word-break: normal; word-wrap: break-word; position: relative; white-space: normal; overflow-x: visible; padding-top: 36px; }
#write.first-line-indent p { text-indent: 2em; }
#write.first-line-indent li p, #write.first-line-indent p * { text-indent: 0px; }
#write.first-line-indent li { margin-left: 2em; }
.for-image #write { padding-left: 8px; padding-right: 8px; }
body.typora-export { padding-left: 30px; padding-right: 30px; }
.typora-export .footnote-line, .typora-export li, .typora-export p { white-space: pre-wrap; }
.typora-export .task-list-item input { pointer-events: none; }
@media screen and (max-width: 500px) {
  body.typora-export { padding-left: 0px; padding-right: 0px; }
  #write { padding-left: 20px; padding-right: 20px; }
  .CodeMirror-sizer { margin-left: 0px !important; }
  .CodeMirror-gutters { display: none !important; }
}
#write li > figure:last-child { margin-bottom: 0.5rem; }
#write ol, #write ul { position: relative; }
img { max-width: 100%; vertical-align: middle; image-orientation: from-image; }
button, input, select, textarea { color: inherit; font-family: inherit; font-size: inherit; font-style: inherit; font-variant-caps: inherit; font-weight: inherit; font-stretch: inherit; line-height: inherit; }
input[type="checkbox"], input[type="radio"] { line-height: normal; padding: 0px; }
*, ::after, ::before { box-sizing: border-box; }
#write h1, #write h2, #write h3, #write h4, #write h5, #write h6, #write p, #write pre { width: inherit; }
#write h1, #write h2, #write h3, #write h4, #write h5, #write h6, #write p { position: relative; }
p { line-height: inherit; }
h1, h2, h3, h4, h5, h6 { break-after: avoid-page; break-inside: avoid; orphans: 4; }
p { orphans: 4; }
h1 { font-size: 2rem; }
h2 { font-size: 1.8rem; }
h3 { font-size: 1.6rem; }
h4 { font-size: 1.4rem; }
h5 { font-size: 1.2rem; }
h6 { font-size: 1rem; }
.md-math-block, .md-rawblock, h1, h2, h3, h4, h5, h6, p { margin-top: 1rem; margin-bottom: 1rem; }
.hidden { display: none; }
.md-blockmeta { color: rgb(204, 204, 204); font-weight: 700; font-style: italic; }
a { cursor: pointer; }
sup.md-footnote { padding: 2px 4px; background-color: rgba(238, 238, 238, 0.7); color: rgb(85, 85, 85); border-radius: 4px; cursor: pointer; }
sup.md-footnote a, sup.md-footnote a:hover { color: inherit; text-transform: inherit; text-decoration: inherit; }
#write input[type="checkbox"] { cursor: pointer; width: inherit; height: inherit; }
figure { overflow-x: auto; margin: 1.2em 0px; max-width: calc(100% + 16px); padding: 0px; }
figure > table { margin: 0px; }
tr { break-inside: avoid; break-after: auto; }
thead { display: table-header-group; }
table { border-collapse: collapse; border-spacing: 0px; width: 100%; overflow: auto; break-inside: auto; text-align: left; }
table.md-table td { min-width: 32px; }
.CodeMirror-gutters { border-right-width: 0px; background-color: inherit; }
.CodeMirror-linenumber { }
.CodeMirror { text-align: left; }
.CodeMirror-placeholder { opacity: 0.3; }
.CodeMirror pre { padding: 0px 4px; }
.CodeMirror-lines { padding: 0px; }
div.hr:focus { cursor: none; }
#write pre { white-space: pre-wrap; }
#write.fences-no-line-wrapping pre { white-space: pre; }
#write pre.ty-contain-cm { white-space: normal; }
.CodeMirror-gutters { margin-right: 4px; }
.md-fences { font-size: 0.9rem; display: block; break-inside: avoid; text-align: left; overflow: visible; white-space: pre; background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; position: relative !important; background-position: inherit; background-repeat: inherit; }
.md-fences-adv-panel { width: 100%; margin-top: 10px; text-align: center; padding-top: 0px; padding-bottom: 8px; overflow-x: auto; }
#write .md-fences.mock-cm { white-space: pre-wrap; }
.md-fences.md-fences-with-lineno { padding-left: 0px; }
#write.fences-no-line-wrapping .md-fences.mock-cm { white-space: pre; overflow-x: auto; }
.md-fences.mock-cm.md-fences-with-lineno { padding-left: 8px; }
.CodeMirror-line, twitterwidget { break-inside: avoid; }
.footnotes { opacity: 0.8; font-size: 0.9rem; margin-top: 1em; margin-bottom: 1em; }
.footnotes + .footnotes { margin-top: 0px; }
.md-reset { margin: 0px; padding: 0px; border: 0px; outline: 0px; vertical-align: top; text-decoration: none; text-shadow: none; float: none; position: static; width: auto; height: auto; white-space: nowrap; cursor: inherit; line-height: normal; font-weight: 400; text-align: left; box-sizing: content-box; direction: ltr; background-position: 0px 0px; }
li div { padding-top: 0px; }
blockquote { margin: 1rem 0px; }
li .mathjax-block, li p { margin: 0.5rem 0px; }
li blockquote { margin: 1rem 0px; }
li { margin: 0px; position: relative; }
blockquote > :last-child { margin-bottom: 0px; }
blockquote > :first-child, li > :first-child { margin-top: 0px; }
.footnotes-area { color: rgb(136, 136, 136); margin-top: 0.714rem; padding-bottom: 0.143rem; white-space: normal; }
#write .footnote-line { white-space: pre-wrap; }
@media print {
  body, html { border: 1px solid transparent; height: 99%; break-after: avoid; break-before: avoid; font-variant-ligatures: no-common-ligatures; }
  #write { margin-top: 0px; padding-top: 0px; border-color: transparent !important; }
  .typora-export * { print-color-adjust: exact; }
  .typora-export #write { break-after: avoid; }
  .typora-export #write::after { height: 0px; }
  .is-mac table { break-inside: avoid; }
  .typora-export-show-outline .typora-export-sidebar { display: none; }
}
.footnote-line { margin-top: 0.714em; font-size: 0.7em; }
a img, img a { cursor: pointer; }
pre.md-meta-block { font-size: 0.8rem; min-height: 0.8rem; white-space: pre-wrap; background-color: rgb(204, 204, 204); display: block; overflow-x: hidden; }
p > .md-image:only-child:not(.md-img-error) img, p > img:only-child { display: block; margin: auto; }
#write.first-line-indent p > .md-image:only-child:not(.md-img-error) img { left: -2em; position: relative; }
p > .md-image:only-child { display: inline-block; width: 100%; }
#write .MathJax_Display { margin: 0.8em 0px 0px; }
.md-math-block { width: 100%; }
.md-math-block:not(:empty)::after { display: none; }
.MathJax_ref { fill: currentcolor; }
[contenteditable="true"]:active, [contenteditable="true"]:focus, [contenteditable="false"]:active, [contenteditable="false"]:focus { outline: 0px; box-shadow: none; }
.md-task-list-item { position: relative; list-style-type: none; }
.task-list-item.md-task-list-item { padding-left: 0px; }
.md-task-list-item > input { position: absolute; top: 0px; left: 0px; margin-left: -1.2em; margin-top: calc(1em - 10px); border: none; }
.math { font-size: 1rem; }
.md-toc { min-height: 3.58rem; position: relative; font-size: 0.9rem; border-radius: 10px; }
.md-toc-content { position: relative; margin-left: 0px; }
.md-toc-content::after, .md-toc::after { display: none; }
.md-toc-item { display: block; color: rgb(65, 131, 196); }
.md-toc-item a { text-decoration: none; }
.md-toc-inner:hover { text-decoration: underline; }
.md-toc-inner { display: inline-block; cursor: pointer; }
.md-toc-h1 .md-toc-inner { margin-left: 0px; font-weight: 700; }
.md-toc-h2 .md-toc-inner { margin-left: 2em; }
.md-toc-h3 .md-toc-inner { margin-left: 4em; }
.md-toc-h4 .md-toc-inner { margin-left: 6em; }
.md-toc-h5 .md-toc-inner { margin-left: 8em; }
.md-toc-h6 .md-toc-inner { margin-left: 10em; }
@media screen and (max-width: 48em) {
  .md-toc-h3 .md-toc-inner { margin-left: 3.5em; }
  .md-toc-h4 .md-toc-inner { margin-left: 5em; }
  .md-toc-h5 .md-toc-inner { margin-left: 6.5em; }
  .md-toc-h6 .md-toc-inner { margin-left: 8em; }
}
a.md-toc-inner { font-size: inherit; font-style: inherit; font-weight: inherit; line-height: inherit; }
.footnote-line a:not(.reversefootnote) { color: inherit; }
.md-attr { display: none; }
.md-fn-count::after { content: "."; }
code, pre, samp, tt { font-family: var(--monospace); }
kbd { margin: 0px 0.1em; padding: 0.1em 0.6em; font-size: 0.8em; color: rgb(36, 39, 41); background-color: rgb(255, 255, 255); border: 1px solid rgb(173, 179, 185); border-radius: 3px; box-shadow: rgba(12, 13, 14, 0.2) 0px 1px 0px, rgb(255, 255, 255) 0px 0px 0px 2px inset; white-space: nowrap; vertical-align: middle; }
.md-comment { color: rgb(162, 127, 3); opacity: 0.6; font-family: var(--monospace); }
code { text-align: left; }
a.md-print-anchor { white-space: pre !important; border: none !important; display: inline-block !important; position: absolute !important; width: 1px !important; right: 0px !important; outline: 0px !important; text-shadow: initial !important; background-position: 0px 0px !important; }
.os-windows.monocolor-emoji .md-emoji { font-family: "Segoe UI Symbol", sans-serif; }
.md-diagram-panel > svg { max-width: 100%; }
[lang="flow"] svg, [lang="mermaid"] svg { max-width: 100%; height: auto; }
[lang="mermaid"] .node text { font-size: 1rem; }
table tr th { border-bottom-width: 0px; }
video { max-width: 100%; display: block; margin: 0px auto; }
iframe { max-width: 100%; width: 100%; border: none; }
.highlight td, .highlight tr { border: 0px; }
mark { background-color: rgb(255, 255, 0); color: rgb(0, 0, 0); }
.md-html-inline .md-plain, .md-html-inline strong, mark .md-inline-math, mark strong { color: inherit; }
.md-expand mark .md-meta { opacity: 0.3 !important; }
mark .md-meta { color: rgb(0, 0, 0); }
@media print {
  .typora-export h1, .typora-export h2, .typora-export h3, .typora-export h4, .typora-export h5, .typora-export h6 { break-inside: avoid; }
}
.md-diagram-panel .messageText { stroke: none !important; }
.md-diagram-panel .start-state { fill: var(--node-fill); }
.md-diagram-panel .edgeLabel rect { opacity: 1 !important; }
.md-fences.md-fences-math { font-size: 1em; }
.md-fences-advanced:not(.md-focus) { padding: 0px; white-space: nowrap; border: 0px; }
.md-fences-advanced:not(.md-focus) { background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; background-position: inherit; background-repeat: inherit; }
.typora-export-show-outline .typora-export-content { max-width: 1440px; margin: auto; display: flex; flex-direction: row; }
.typora-export-sidebar { width: 300px; font-size: 0.8rem; margin-top: 80px; margin-right: 18px; }
.typora-export-show-outline #write { --webkit-flex: 2; flex: 2 1 0%; }
.typora-export-sidebar .outline-content { position: fixed; top: 0px; max-height: 100%; overflow: hidden auto; padding-bottom: 30px; padding-top: 60px; width: 300px; }
@media screen and (max-width: 1024px) {
  .typora-export-sidebar, .typora-export-sidebar .outline-content { width: 240px; }
}
@media screen and (max-width: 800px) {
  .typora-export-sidebar { display: none; }
}
.outline-content li, .outline-content ul { margin-left: 0px; margin-right: 0px; padding-left: 0px; padding-right: 0px; list-style: none; }
.outline-content ul { margin-top: 0px; margin-bottom: 0px; }
.outline-content strong { font-weight: 400; }
.outline-expander { width: 1rem; height: 1.428571429rem; position: relative; display: table-cell; vertical-align: middle; cursor: pointer; padding-left: 4px; }
.outline-expander::before { content: ""; position: relative; font-family: Ionicons; display: inline-block; font-size: 8px; vertical-align: middle; }
.outline-item { padding-top: 3px; padding-bottom: 3px; cursor: pointer; }
.outline-expander:hover::before { content: ""; }
.outline-h1 > .outline-item { padding-left: 0px; }
.outline-h2 > .outline-item { padding-left: 1em; }
.outline-h3 > .outline-item { padding-left: 2em; }
.outline-h4 > .outline-item { padding-left: 3em; }
.outline-h5 > .outline-item { padding-left: 4em; }
.outline-h6 > .outline-item { padding-left: 5em; }
.outline-label { cursor: pointer; display: table-cell; vertical-align: middle; text-decoration: none; color: inherit; }
.outline-label:hover { text-decoration: underline; }
.outline-item:hover { border-color: rgb(245, 245, 245); background-color: var(--item-hover-bg-color); }
.outline-item:hover { margin-left: -28px; margin-right: -28px; border-left-width: 28px; border-left-style: solid; border-left-color: transparent; border-right-width: 28px; border-right-style: solid; border-right-color: transparent; }
.outline-item-single .outline-expander::before, .outline-item-single .outline-expander:hover::before { display: none; }
.outline-item-open > .outline-item > .outline-expander::before { content: ""; }
.outline-children { display: none; }
.info-panel-tab-wrapper { display: none; }
.outline-item-open > .outline-children { display: block; }
.typora-export .outline-item { padding-top: 1px; padding-bottom: 1px; }
.typora-export .outline-item:hover { margin-right: -8px; border-right-width: 8px; border-right-style: solid; border-right-color: transparent; }
.typora-export .outline-expander::before { content: "+"; font-family: inherit; top: -1px; }
.typora-export .outline-expander:hover::before, .typora-export .outline-item-open > .outline-item > .outline-expander::before { content: "−"; }
.typora-export-collapse-outline .outline-children { display: none; }
.typora-export-collapse-outline .outline-item-open > .outline-children, .typora-export-no-collapse-outline .outline-children { display: block; }
.typora-export-no-collapse-outline .outline-expander::before { content: "" !important; }
.typora-export-show-outline .outline-item-active > .outline-item .outline-label { font-weight: 700; }
.md-inline-math-container mjx-container { zoom: 0.95; }


/*
Version: v1.4
1. Updated colour to be more accessible.
2. Included FontAwesome link directly in the css.
3. Imported Buttons CSS.
4. Updated font to Amazon Ember.
*/

:root {
    --side-bar-bg-color: #fafafa;
    --control-text-color: #333333;
}

/* Importing Font Awesome */
@import url("file:///Users/davemohr/Library/Application%20Support/abnerworks.Typora/themes/");

/* @include-when-export url(https://fonts.loli.net/css?family=Open+Sans:400italic,700italic,700,400&subset=latin,latin-ext); /*


/* Adding button support */
#ssb_alexa_blue {
background-color: #3366ff;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #3366ff;
border-radius: 2px;
white-space: nowrap
}
#ssb_alexa_ocean {
background-color: #00a0d2;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #00a0d2;
white-space: nowrap
}
#ssb_alexa_sand {
background-color: #f2f2f2;
font-weight: bold;
font-size: 90%;
color: #00a0d2;
position: relative;
top: -1px;
border-color: #dcdcdc;
border-style: solid;
border-width: 2px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_alexa_white {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #00a0d2;
position: relative;
top: -1px;
border-color: #00a0d2;
border-style: solid;
border-width: 2px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_blue {
background-color: #257ACF;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
border-radius: 5px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_catalog_orange {
background-color: #E36000;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
border-radius: 1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_catalog_red {
background-color: #D90000;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
border-radius: 5px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_dark_blue {
color: white;
background-color: darkblue;
border-radius: 3px;
padding: 0px 6px;
white-space: nowrap
}
#ssb_grafana_blue {
background-color: #00678b;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #00678b;
border-radius: 2px;
white-space: nowrap
}
#ssb_grafana_green {
background-color: #629300;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #629300;
border-radius: 2px;
white-space: nowrap
}
#ssb_grafana_orange {
background-color: #ec8427;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #ec8427;
border-radius: 2px;
white-space: nowrap
}
#ssb_grey {
background-color: #DEDEDE;
font-weight: bold;
font-size: 90%;
color: #444;
position: relative;
top: -1px;
border-radius: 5px;
border-width: 1px;
border-style: solid;
border-color: #444;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_grey_square {
background-color: #DEDEDE;
font-weight: bold;
font-size: 90%;
color: #444;
position: relative;
top: -1px;
border-radius: 1px;
border-width: 1px;
border-style: solid;
border-color: #444;
padding-top: 2px;
padding-bottom: 2px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_iot_blue {
background-color: #00A1C9;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #00A1C9;
border-radius: 2px;
white-space: nowrap
}
#ssb_iot_grey {
background-color: white;
font-weight: bold;
font-size: 90%;
color: gray;
position: relative;
top: -1px;
border-color: gray;
border-radius: 2px;
border-style: solid;
border-width: 1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_iot_white {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #00A1C9;
position: relative;
top: -1px;
border-color: #00A1C9;
border-radius: 2px;
border-style: solid;
border-width: 1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_kibana_blue {
background-color: #0079a5;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #0079a5;
border-radius: 2px;
white-space: nowrap
}
#ssb_kibana_white {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #0079a5;
position: relative;
top: -1px;
border-color: #0079a5;
border-radius: 2px;
border-width: 1px;
border-style: solid;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_lambda_orange {
background-color: #ec7211;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_lambda_white {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #545b64;
position: relative;
top: -1px;
border-color: #545b64;
border-radius: 2px;
border-width: 1px;
border-style: solid;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_maroon {
color: white;
background-color: darkred;
border-radius: 3px;
padding: 0px 6px;
white-space: nowrap
}
#ssb_orange {
background-color: #ec7211;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssl_orange {
color: #ec7211;
font-weight: bold
}
#ssb_orange_oval {
background-color: #ec7211;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-radius: 20px;
white-space: nowrap
}
#ssb_oval {
background-color: #DEDEDE;
font-weight: bold;
font-size: 90%;
color: #444;
position: relative;
top: -1px;
border-radius: 20px;
border-width: 1px;
border-style: solid;
border-color: #444;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
}
#ssb_start_lab {
background-color: #34A853;
font-weight: bold;
font-size: 90%;
color: white;
border-radius: 2px;
padding-left: 10px;
padding-right: 10px;
padding-top: 3px;
padding-bottom: 3px
}
#ssb_open_console {
background-color: white;
font-family: Google Sans;
font-weight: bold;
font-size: 90%;
color: #1a73e8;
border-color: #dadce0;
border-radius: 4px;
border-width: 2px;
border-style: solid;
outline-color: #ffffff;
padding-top: 5px;
padding-bottom: 5px;
padding-left: 10px;
padding-right: 10px
}
#ssb_rds_white {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #545b64;
position: relative;
top: -1px;
border-color: #545b64;
border-radius: 2px;
border-width: 1px;
border-style: solid;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
}
#ssb_red {
background-color: #D93025;
font-weight: bold;
font-size: 90%;
color: white;
border-radius: 2px;
padding-left: 10px;
padding-right: 10px;
padding-top: 3px;
padding-bottom: 3px
}
#ssb_red_oval {
background-color: #D93025;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-radius: 20px;
white-space: nowrap
}
#ssb_s3_blue {
background-color: #329AD6;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
}
#ssb_s3_white {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #329AD6;
position: relative;
top: -1px;
border-color: #329AD6;
border-width: 1px;
border-style: solid;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
}
#ssb_services {
background-color: #232f3e;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
}
#ssb_square_lex {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #1166bb;
position: relative;
top: -1px;
border-color: #c4cbcd;
border-style: solid;
border-width: 2px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px
}
#ssb_ssm_white {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #545b64;
position: relative;
top: -1px;
border-color: #545b64;
border-radius: 2px;
border-width: 1px;
border-style: solid;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
}
#ssb_white {
background-color: white;
font-weight: bold;
font-size: 90%;
color: #545b64;
position: relative;
top: -1px;
border-color: #545b64;
border-radius: 2px;
border-width: 1px;
border-style: solid;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
}
#ssbox_cloudformation_blue {
font-weight: bold;
background-color: #f1faff;
font-size: 90%;
border-color: #00A1C9;
border-width: 1px;
border-style: solid;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
}
#ssl_alexa_ocean {
color: #00a0d2;
font-weight: bold
}
#ssl_blue {
color: #1166bb;
font-weight: bold
}
#ssl_catalog_orange {
color: #E16706;
font-weight: bold
}
#ssb_codestar_blue {
background-color: #329AD6;
font-weight: bold;
font-size: 80%;
color: white;
position: relative;
top: -1px;
border-radius: 1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
white-space: nowrap
}
#ssb_cognito_blue {
background-color: #2a7fd4;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #0055aa;
border-radius: 2px;
white-space: nowrap
}
#ssb_eb_blue {
background-color: #0f6dca;
font-weight: bold;
font-size: 90%;
color: white;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #0055aa;
border-width: 1px;
border-style: solid;
border-radius: 4px;
white-space: nowrap;
}
#ssb_eb_grey {
background-color: #e5e5e5;
font-weight: bold;
font-size: 90%;
color: 444444;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: #bbbbbb;
border-width: 1px;
border-style: solid;
border-radius: 4px;
white-space: nowrap
}
#ssb_voc_grey {
background-color: #F2F3F4;
font-size: 90%;
color: black;
position: relative;
top: -1px;
padding-top: 3px;
padding-bottom: 3px;
padding-left: 10px;
padding-right: 10px;
border-color: grey;
border-width: 1px;
border-style: solid;
white-space: nowrap
}


/* open-sans-regular - latin-ext_latin */
  /* open-sans-italic - latin-ext_latin */
    /* open-sans-700 - latin-ext_latin */
    /* open-sans-700italic - latin-ext_latin */
  html {
    font-size: 16px;
    -webkit-font-smoothing: antialiased;
}

body {
    font-family: "Amazon Ember", "Open Sans","Clear Sans", "Helvetica Neue", Helvetica, Arial, 'Segoe UI Emoji', sans-serif;
    color: rgb(51, 51, 51);
    line-height: 1.6;
}

#write {
    max-width: 860px;
  	margin: 0 auto;
  	padding: 30px;
    padding-bottom: 100px;
}

@media only screen and (min-width: 1400px) {
	#write {
		max-width: 1024px;
	}
}

@media only screen and (min-width: 1800px) {
	#write {
		max-width: 1200px;
	}
}

#write > ul:first-child,
#write > ol:first-child{
    margin-top: 30px;
}

a {
    color: #0071bc;
}
h1,
h2,
h3,
h4,
h5,
h6 {
    position: relative;
    margin-top: 1rem;
    margin-bottom: 1rem;
    font-weight: bold;
    line-height: 1.4;
    cursor: text;
}
h1:hover a.anchor,
h2:hover a.anchor,
h3:hover a.anchor,
h4:hover a.anchor,
h5:hover a.anchor,
h6:hover a.anchor {
    text-decoration: none;
}
h1 tt,
h1 code {
    font-size: inherit;
}
h2 tt,
h2 code {
    font-size: inherit;
}
h3 tt,
h3 code {
    font-size: inherit;
}
h4 tt,
h4 code {
    font-size: inherit;
}
h5 tt,
h5 code {
    font-size: inherit;
}
h6 tt,
h6 code {
    font-size: inherit;
}
h1 {
    font-size: 2.25em;
    line-height: 1.2;
    border-bottom: 1px solid #eee;
}
h2 {
    font-size: 1.75em;
    line-height: 1.225;
    border-bottom: 1px solid #eee;
}

h3 {
    font-size: 1.5em;
    line-height: 1.43;
}
h4 {
    font-size: 1.25em;
}
h5 {
    font-size: 1em;
}
h6 {
   font-size: 1em;
    color: #5b616b;
}
p,
blockquote,
ul,
ol,
dl,
table{
    margin: 0.8em 0;
}
li>ol,
li>ul {
    margin: 0 0;
}
hr {
    height: 2px;
    padding: 0;
    margin: 16px 0;
    background-color: #e7e7e7;
    border: 0 none;
    overflow: hidden;
    box-sizing: content-box;
}

li p.first {
    display: inline-block;
}
ul,
ol {
    padding-left: 30px;
}
ul:first-child,
ol:first-child {
    margin-top: 0;
}
ul:last-child,
ol:last-child {
    margin-bottom: 0;
}
blockquote {
    border-left: 4px solid #dfe2e5;
    padding: 0 15px;
    color: #5b616b; /*#777777*/
}
blockquote blockquote {
    padding-right: 0;
}
table {
    padding: 0;
    word-break: initial;
}
table tr {
    border: 1px solid #dfe2e5;
    margin: 0;
    padding: 0;
}
table tr:nth-child(2n),
thead {
    background-color: #f8f8f8;
}
table th {
    font-weight: bold;
    border: 1px solid #dfe2e5;
    border-bottom: 0;
    margin: 0;
    padding: 6px 13px;
}
table td {
    border: 1px solid #dfe2e5;
    margin: 0;
    padding: 6px 13px;
}
table th:first-child,
table td:first-child {
    margin-top: 0;
}
table th:last-child,
table td:last-child {
    margin-bottom: 0;
}

.CodeMirror-lines {
    padding-left: 4px;
}

.code-tooltip {
    box-shadow: 0 1px 1px 0 rgba(0,28,36,.3);
    border-top: 1px solid #eef2f2;
}

.md-fences,
code,
tt {
    border: 1px solid #e7eaed;
    background-color: #f8f8f8;
    border-radius: 3px;
    padding: 0;
    padding: 2px 4px 0px 4px;
    font-size: 0.9em;
}

code {
    background-color: #f3f4f4;
    padding: 0 2px 0 2px;
}

.md-fences {
    margin-bottom: 15px;
    margin-top: 15px;
    padding-top: 8px;
    padding-bottom: 6px;
}


.md-task-list-item > input {
  margin-left: -1.3em;
}

@media print {
    html {
        font-size: 13px;
    }
    table,
    pre {
        page-break-inside: avoid;
    }
    pre {
        word-wrap: break-word;
    }
}

.md-fences {
	background-color: #f8f8f8;
}
#write pre.md-meta-block {
	padding: 1rem;
    font-size: 85%;
    line-height: 1.45;
    background-color: #f7f7f7;
    border: 0;
    border-radius: 3px;
    color: #323a45;  /*#777777*/
    margin-top: 0 !important;
}

.mathjax-block>.code-tooltip {
	bottom: .375rem;
}

.md-mathjax-midline {
    background: #fafafa;
}

#write>h3.md-focus:before{
	left: -1.5625rem;
	top: .375rem;
}
#write>h4.md-focus:before{
	left: -1.5625rem;
	top: .285714286rem;
}
#write>h5.md-focus:before{
	left: -1.5625rem;
	top: .285714286rem;
}
#write>h6.md-focus:before{
	left: -1.5625rem;
	top: .285714286rem;
}
.md-image>.md-meta {
    /*border: 1px solid #ddd;*/
    border-radius: 3px;
    padding: 2px 0px 0px 4px;
    font-size: 0.9em;
    color: inherit;
}

.md-tag {
    color: #323a45; /*a7a7a7*/
    opacity: 1;
}

.md-toc {
    margin-top:20px;
    padding-bottom:20px;
}

.sidebar-tabs {
    border-bottom: none;
}

#typora-quick-open {
    border: 1px solid #ddd;
    background-color: #f8f8f8;
}

#typora-quick-open-item {
    background-color: #ffffff;
    border-color: #FEFEFE #e5e5e5 #e5e5e5 #eee;
    border-style: solid;
    border-width: 1px;
}

/** focus mode */
.on-focus-mode blockquote {
    border-left-color: rgba(85, 85, 85, 0.12);
}

header, .context-menu, .megamenu-content, footer{
    font-family: "Segoe UI", "Arial", sans-serif;
}

.file-node-content:hover .file-node-icon,
.file-node-content:hover .file-node-open-state{
    visibility: visible;
}

.mac-seamless-mode #typora-sidebar {
    background-color: #fafafa;
    background-color: var(--side-bar-bg-color);
}

.md-lang {
    color: #981b1e;
}

/*.html-for-mac {
    --item-hover-bg-color: #E6F0FE;
}*/

#md-notification .btn {
    border: 0;
}

.dropdown-menu .divider {
    border-color: #e5e5e5;
    opacity: 0.4;
}

.ty-preferences .window-content {
    background-color: #fafafa;
}

.ty-preferences .nav-group-item.active {
    color: white;
    background: #999;
}

.menu-item-container a.menu-style-btn {
    background-color: #f5f8fa;
    background-image: linear-gradient( 180deg , hsla(0, 0%, 100%, 0.8), hsla(0, 0%, 100%, 0));
}


 @media print { @page {margin: 0 0 0 0;} body.typora-export {padding-left: 0; padding-right: 0;} #write {padding:0;}}
</style><title>README</title>
<script type="text/javascript" src="./Guided Lab Creating an Amazon RDS Database_files/c7fa7451-6f95-4815-ac32-b8cc2537837a" data-awssuidacr="53831616-c450-4d58-b234-a61f3b697d56"></script></head>
<body class="typora-export vsc-initialized"><div class="typora-export-content">
<div id="write" class=""><h1 id="module-5---guided-lab-creating-an-amazon-rds-database"><span>Module 5 - Guided Lab: Creating an Amazon RDS Database</span></h1><!-- ILT-TF-200-ACACAD-2 Source Course: ILT-TF-100-ARCHIT-6 branch dev_65 --><h2 id="lab-overview-and-objectives"><span>Lab overview and objectives</span></h2><p><span>Traditionally, creating a database can be a complex process that requires either a database administrator or a systems administrator. In the cloud, you can simplify this process by using Amazon Relational Database Service (Amazon RDS).</span></p><p><span>After completing this lab, you should be able to:</span></p><ul><li><span>Launch a database using </span><strong><span>Amazon RDS</span></strong><span>  </span></li><li><span>Configure a web application to connect to the </span><strong><span>database instance</span></strong></li></ul><p><span>At the </span><strong><span>end</span></strong><span> of this lab, your architecture will look like the following example:</span></p><p><img src="./Guided Lab Creating an Amazon RDS Database_files/rds-guided-lab-arch.png" referrerpolicy="no-referrer" alt="Architecture"></p><h2 id="duration"><span>Duration</span></h2><p><span>This lab will require approximately </span><strong><span>20 minutes</span></strong><span> to complete.</span></p><p>&nbsp;</p><h2 id="aws-service-restrictions"><span>AWS service restrictions</span></h2><p><span>In this lab environment, access to AWS services and service actions might be restricted to the ones that are needed to complete the lab instructions. You might encounter errors if you attempt to access other services or perform actions beyond the ones that are described in this lab.</span></p><p>&nbsp;</p><h2 id="accessing-the-aws-management-console"><span>Accessing the AWS Management Console</span></h2><ol start=""><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> to launch your lab.</span></p><p><span>A </span><strong><span>Start Lab</span></strong><span> panel opens, and it displays the lab status.</span></p><p><i class="fas fa-info-circle"></i><span> </span><strong><span>Tip</span></strong><span>: If you need more time to complete the lab, restart the timer for the environment by choosing the </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> button again.</span></p><p>&nbsp;</p></li><li><p><span>Wait until the </span><strong><span>Start Lab</span></strong><span> panel displays the message </span><strong><span>Lab status: ready</span></strong><span>, then close the panel by choosing the </span><strong><span>X</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>AWS</span></span></p><p><span>This action opens the AWS Management Console in a new browser tab. The system automatically logs you in.</span></p><p><i class="fas fa-exclamation-triangle"></i><span> </span><strong><span>Tip</span></strong><span>: If a new browser tab does not open, a banner or icon is usually at the top of your browser with the message that your browser is preventing the site from opening pop-up windows. Choose the banner or icon, and then choose </span><strong><span>Allow pop-ups</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Arrange the </span><strong><span>AWS Management Console</span></strong><span> tab so that it displays alongside these instructions. Ideally, you will have both browser tabs open at the same time so that you can follow the lab steps more easily.</span></p><p><i class="fas fa-exclamation-triangle"></i><span> </span><strong><span>Do not change the Region unless specifically instructed to do so</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><h2 id="task-1-creating-an-amazon-rds-database"><span>Task 1: Creating an Amazon RDS database</span></h2><p><span>In this task, you will create a MySQL database in your virtual private cloud (VPC). MySQL is a popular open source relational database management system (RDBMS), so there are no software licensing fees.</span></p><p><span style="color:red"><i class="fas fa-exclamation-triangle"></i><span> </span><strong><span>Windows Users:</span></strong></span><span> Use Chrome or Firefox as your web browser for this lab. The lab instructions are </span><strong><span>not compatible with </span><em><span>Internet Explorer</span></em></strong><span> because of a difference in the Amazon RDS console.</span></p><p>&nbsp;</p><ol start="5"><li><p><span>In the search box to the right of </span><i class="fas fa-th"></i><span> </span><strong><span>Services</span></strong><span>, search for and choose </span><strong><span>RDS</span></strong><span> to open the RDS console.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create database</span></span></p><p>&nbsp;</p></li><li><p><span>Under </span><strong><span>Engine options</span></strong><span>, select </span><i class="far fa-dot-circle"></i><strong><span>MySQL</span></strong><span>.</span></p><p><span>The options include several use cases, ranging from enterprise-class databases to Dev/Test systems. In the options, you might notice </span><strong><span>Amazon Aurora</span></strong><span>. Aurora is a MySQL-compatible system that was re-architected for the cloud. If your company uses large-scale MySQL or PostgreSQL databases, Aurora can provide enhanced performance.</span></p><p>&nbsp;</p></li><li><p><span>Set the templates and availability and durability options:</span></p><ul><li><p><span>Under the </span><strong><span>Templates</span></strong><span> section, select </span><i class="far fa-dot-circle"></i><span> </span><strong><span>Dev/Test</span></strong><span>.</span></p></li><li><p><span>Under the </span><strong><span>Availability and durability</span></strong><span> section, select </span><i class="far fa-dot-circle"></i><span>  </span><strong><span>Single DB instance</span></strong><span> </span></p><p><strong><span>Note</span></strong><span>: the default </span><em><span>Multi-AZ deployment</span></em><span> option automatically creates a replica of the database in a second Availability Zone for High Availability, however in this lab that is not needed.</span></p></li></ul><p>&nbsp;</p></li><li><p><span>Under the </span><strong><span>Settings</span></strong><span> section, configure these options:</span></p><ul><li><p><strong><span>DB instance identifier:</span></strong><span> </span><code>inventory-db</code></p></li><li><p><strong><span>Username:</span></strong><span> </span><code>admin</code></p></li><li><p><strong><span>Password:</span></strong><span> </span><code>lab-password</code></p></li><li><p><strong><span>Confirm password:</span></strong><span> </span><code>lab-password</code></p><p>&nbsp;</p></li></ul></li><li><p><span>Under the </span><strong><span>DB instance class</span></strong><span> section, configure these options:</span></p><ul><li><p><span>Select </span><i class="far fa-dot-circle"></i><strong><span>Burstable classes (includes t classes)</span></strong><span>.</span></p></li><li><p><span>Select </span><strong><span>db.t3.micro</span></strong></p><p>&nbsp;</p></li></ul></li><li><p><span>Under the </span><strong><span>Connectivity</span></strong><span> section, configure these options: </span></p><ul><li><p><strong><span>Virtual Private Cloud (VPC):</span></strong><span> </span><em><span>Lab VPC</span></em></p></li><li><p><strong><span>Existing VPC security groups:</span></strong><span> </span></p><ul><li><span>Choose </span><em><span>DB-SG</span></em><span>. It will be highlighted. </span></li><li><span>Remove the </span><em><span>default</span></em><span> security group.</span></li></ul><p>&nbsp;</p></li></ul></li><li><p><span>Expand the </span><i class="fas fa-caret-right"></i><strong><span>Additional configuration</span></strong><span> panel, then configure these settings:</span></p><ul><li><p><strong><span>Initial database name:</span></strong><span> </span><code>inventory</code></p><p><span>Note: This is the logical name of the database that will be used by the application.</span></p></li><li><p><span>Clear (turn off) the </span><strong><span>Enable Enhanced monitoring</span></strong><span> option</span></p></li></ul><p>&nbsp;</p><p><i class="fas fa-comment"></i><span> Feel free to review the many other options displayed on the page, but leave them set to their default values. Options include automatic backups, the ability to export log files, and automatic version upgrades. The ability to activate these features through check boxes demonstrates the power of using a </span><em><span>fully managed database solution</span></em><span> instead of installing, backing up, and maintaining the database yourself.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create database</span></span><span> (at the bottom of the page).</span></p><p><span>You should receive a message indicating that your database is being created.</span></p><p><i class="fas fa-exclamation-triangle"></i><span> If you receive an error message that mentions </span><em><span>rds-monitoring-role</span></em><span>, confirm that you have cleared (turned off) the </span><strong><span>Enhanced Monitoring</span></strong><span> option in the previous step, then try again.</span></p><p><span>Before you continue to the next task, the database instance status must be </span><em><span>Available</span></em><span>. This process might take several minutes.</span></p></li></ol><p>&nbsp;</p><h2 id="task-2-configuring-web-application-communication-with-a-database-instance"><span>Task 2: Configuring web application communication with a database instance</span></h2><p><span>This lab automatically deployed an Amazon Elastic Compute Cloud (Amazon EC2) instance with a running web application. You must use the IP address of the instance to connect to the application.</span></p><p>&nbsp;</p><ol start="14"><li><p><span>In the search box to the right of </span><i class="fas fa-th"></i><span> </span><strong><span>Services</span></strong><span>, search for and choose </span><strong><span>EC2</span></strong><span> to open the EC2 console.</span></p><p>&nbsp;</p></li><li><p><span>In the left navigation pane, choose </span><strong><span>Instances</span></strong><span>.</span></p><p><span>In the center pane, there should be a running instance that is named </span><strong><span>App Server</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Select the </span><strong><span>App Server</span></strong><span> instance.</span></p><p>&nbsp;</p></li><li><p><span>In the </span><strong><span>Details</span></strong><span> tab, copy the </span><strong><span>Public IPv4 address</span></strong><span> to your clipboard.</span></p><p><strong><span>Tip:</span></strong><span> If you hover over the IP address, a copy </span><i class="far fa-copy"></i><span> icon appears. To copy the displayed value, choose the icon.</span></p><p>&nbsp;</p></li><li><p><span>Open a new web browser tab, paste the IP address into the address bar, and then press ENTER.</span></p><p><span>The web application should appear. It does not display much information because the application is not yet connected to the database.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><i class="fas fa-cog" aria-hidden="true"></i><strong><span>Settings</span></strong><span>.</span></p><p><span>You can now configure the application to use the RDS DB instance you created earlier. You will first retrieve the </span><strong><span>Database Endpoint</span></strong><span> so that the application knows how to connect to a database.</span></p><p>&nbsp;</p></li><li><p><span>Return to the </span><strong><span>AWS Management Console</span></strong><span>, but do not close the application tab. (You will return to it soon.</span></p><p>&nbsp;</p></li><li><p><span>In the </span><i class="fas fa-th"></i><span> </span><strong><span>Services</span></strong><span> search box, search for and choose </span><strong><span>RDS</span></strong><span> to open the RDS console.</span></p><p>&nbsp;</p></li><li><p><span>In the left navigation pane, choose </span><strong><span>Databases</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span style="color:blue;"><span>inventory-db</span></span><span>.</span></p><p>&nbsp;</p></li><li><p><span>Scroll to the </span><strong><span>Connectivity &amp; Security</span></strong><span> section and copy the </span><strong><span>Endpoint</span></strong><span> to your clipboard.</span></p><p><span>It should look similar to this example: </span><em><span>inventory-db.crwxbgqad61a.rds.amazonaws.com</span></em></p><p>&nbsp;</p></li><li><p><span>Return to the browser tab with the Inventory application, and enter these values:</span></p><ul><li><strong><span>Endpoint:</span></strong><span> Paste the endpoint you copied earlier</span></li><li><strong><span>Database:</span></strong><span> </span><code>inventory</code></li><li><strong><span>Username:</span></strong><span> </span><code>admin</code></li><li><strong><span>Password:</span></strong><span> </span><code>lab-password</code></li><li><span>Choose </span><strong><span>Save</span></strong></li></ul><p><span>The application will now connect to the database, load some initial data, and display information.</span></p><p>&nbsp;</p></li><li><p><i class="fas fa-plus"></i><span>  Add inventory, </span><i class="fas fa-edit" style="color:#257ACF;"></i><span> edit, and </span><i class="fas fa-trash-alt" style="color:#d82323;"></i><span>delete inventory information by using the web application.</span></p><p><span>The inventory information is stored in the Amazon RDS MySQL database that you created earlier in the lab. This means that any failure in the application server will </span><em><span>not</span></em><span> lose any data. It also means that multiple application servers can access the same data.</span></p><p>&nbsp;</p></li><li><p><span>Insert new records into the table. Ensure that the table has 5 or more inventory records before submitting your work.</span></p><p><i class="fas fa-thumbs-up" style="color:green;"></i><span> You have now successfully launched the application and connected it to the database!</span></p><p><strong><span>Optional:</span></strong><span> You can access the saved parameters in the </span><strong><span>Systems Manager</span></strong><span> console, under </span><strong><span>Parameter Store</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><h2 id="submitting-your-work"><span>Submitting your work</span></h2><ol start="28"><li><p><span>At the top of these instructions, choose </span><span id="ssb_blue"><span>Submit</span></span><span> to record your progress and when prompted, choose </span><strong><span>Yes</span></strong><span>. </span></p><p>&nbsp;</p></li><li><p><span>If the results don't display after a couple of minutes, return to the top of these instructions and choose </span><span id="ssb_voc_grey"><span>Grades</span></span></p><p><strong><span>Tip</span></strong><span>: You can submit your work multiple times. After you change your work, choose </span><strong><span>Submit</span></strong><span> again. Your last submission is what will be recorded for this lab.</span></p><p>&nbsp;</p></li><li><p><span>To find detailed feedback on your work, choose </span><span id="ssb_voc_grey"><span>Details</span></span><span> followed by </span><i class="fas fa-caret-right"></i><span> </span><strong><span>View Submission Report</span></strong><span>.</span></p></li></ol><br><h2 id="lab-complete-i-classfas-fa-graduation-capi"><span>Lab complete </span><i class="fas fa-graduation-cap"></i></h2><p><i class="fas fa-flag-checkered"></i><span> Congratulations! You have completed the lab.</span></p><p>&nbsp;</p><ol start="31"><li><p><span>Choose </span><span id="ssb_voc_grey"><span>End Lab</span></span><span> at the top of this page, and then select </span><span id="ssb_blue"><span>Yes</span></span><span> to confirm that you want to end the lab.</span></p><p><span>A panel should appear with this message: </span><em><span>DELETE has been initiated... You may close this message box now.</span></em><span>   </span></p><p>&nbsp;</p></li><li><p><span>Select the </span><strong><span>X</span></strong><span> in the top right corner to close the panel.</span></p></li></ol><p>&nbsp;</p><p><em><span>©2021 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.</span></em></p><p>&nbsp;</p></div></div>
<script defer="" src="./Guided Lab Creating an Amazon RDS Database_files/vcd15cbe7772f49c399c6a5babf22c1241717689176015" integrity="sha512-ZpsOmlRQV6y907TI0dKBHq9Md29nnaEIPlkf84rnaERnq6zvWvPUqr2ft8M1aS28oN72PdrCzSjY4U6VaAw1EQ==" data-cf-beacon="{&quot;rayId&quot;:&quot;8bae30a2ec3d77f4&quot;,&quot;serverTiming&quot;:{&quot;name&quot;:{&quot;cfL4&quot;:true}},&quot;version&quot;:&quot;2024.8.0&quot;,&quot;token&quot;:&quot;a73834a4a1444e9ab89e8da06da41720&quot;}" crossorigin="anonymous"></script>

<script>(() => {
        window.addoncropExtensions = window.addoncropExtensions || [];
        window.addoncropExtensions.push({
            mode: 'emulator',
            emulator: 'Foxified',
            extension: {
                id: 44,
                name: 'YouTube Downloader by Addoncrop',
                version: '17.3.2',
                date: 'May 24, 2024',
            },
            flixmateConnected: false,
        });
    })();</script></body></html>