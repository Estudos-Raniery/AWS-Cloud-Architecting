<!DOCTYPE html>
<!-- saved from url=(0089)https://labs.vocareum.com/web/1964919/3231447.0/ASNLIB/public/docs/lang/en_us/README.html -->
<html foxified=""><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta name="viewport" content="width=device-width initial-scale=1">

<link href="./Guided Lab Creating a Virtual Private Cloud_files/all.css" rel="stylesheet" type="text/css"><style type="text/css">html {overflow-x: initial !important;}:root { --bg-color: #ffffff; --text-color: #333333; --select-text-bg-color: #B5D6FC; --select-text-font-color: auto; --monospace: "Lucida Console",Consolas,"Courier",monospace; --title-bar-height: 20px; }
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


.CodeMirror { height: auto; }
.CodeMirror.cm-s-inner { background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; background-position: inherit; background-repeat: inherit; }
.CodeMirror-scroll { overflow: auto hidden; z-index: 3; }
.CodeMirror-gutter-filler, .CodeMirror-scrollbar-filler { background-color: rgb(255, 255, 255); }
.CodeMirror-gutters { border-right-width: 1px; border-right-style: solid; border-right-color: rgb(221, 221, 221); background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; white-space: nowrap; background-position: inherit; background-repeat: inherit; }
.CodeMirror-linenumber { padding: 0px 3px 0px 5px; text-align: right; color: rgb(153, 153, 153); }
.cm-s-inner .cm-keyword { color: rgb(119, 0, 136); }
.cm-s-inner .cm-atom, .cm-s-inner.cm-atom { color: rgb(34, 17, 153); }
.cm-s-inner .cm-number { color: rgb(17, 102, 68); }
.cm-s-inner .cm-def { color: rgb(0, 0, 255); }
.cm-s-inner .cm-variable { color: rgb(0, 0, 0); }
.cm-s-inner .cm-variable-2 { color: rgb(0, 85, 170); }
.cm-s-inner .cm-variable-3 { color: rgb(0, 136, 85); }
.cm-s-inner .cm-string { color: rgb(170, 17, 17); }
.cm-s-inner .cm-property { color: rgb(0, 0, 0); }
.cm-s-inner .cm-operator { color: rgb(152, 26, 26); }
.cm-s-inner .cm-comment, .cm-s-inner.cm-comment { color: rgb(170, 85, 0); }
.cm-s-inner .cm-string-2 { color: rgb(255, 85, 0); }
.cm-s-inner .cm-meta { color: rgb(85, 85, 85); }
.cm-s-inner .cm-qualifier { color: rgb(85, 85, 85); }
.cm-s-inner .cm-builtin { color: rgb(51, 0, 170); }
.cm-s-inner .cm-bracket { color: rgb(153, 153, 119); }
.cm-s-inner .cm-tag { color: rgb(17, 119, 0); }
.cm-s-inner .cm-attribute { color: rgb(0, 0, 204); }
.cm-s-inner .cm-header, .cm-s-inner.cm-header { color: rgb(0, 0, 255); }
.cm-s-inner .cm-quote, .cm-s-inner.cm-quote { color: rgb(0, 153, 0); }
.cm-s-inner .cm-hr, .cm-s-inner.cm-hr { color: rgb(153, 153, 153); }
.cm-s-inner .cm-link, .cm-s-inner.cm-link { color: rgb(0, 0, 204); }
.cm-negative { color: rgb(221, 68, 68); }
.cm-positive { color: rgb(34, 153, 34); }
.cm-header, .cm-strong { font-weight: 700; }
.cm-del { text-decoration: line-through; }
.cm-em { font-style: italic; }
.cm-link { text-decoration: underline; }
.cm-error { color: red; }
.cm-invalidchar { color: red; }
.cm-constant { color: rgb(38, 139, 210); }
.cm-defined { color: rgb(181, 137, 0); }
div.CodeMirror span.CodeMirror-matchingbracket { color: rgb(0, 255, 0); }
div.CodeMirror span.CodeMirror-nonmatchingbracket { color: rgb(255, 34, 34); }
.cm-s-inner .CodeMirror-activeline-background { background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; background-position: inherit; background-repeat: inherit; }
.CodeMirror { position: relative; overflow: hidden; }
.CodeMirror-scroll { height: 100%; outline: 0px; position: relative; box-sizing: content-box; background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; background-position: inherit; background-repeat: inherit; }
.CodeMirror-sizer { position: relative; }
.CodeMirror-gutter-filler, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-filler, .CodeMirror-vscrollbar { position: absolute; z-index: 6; display: none; outline: 0px; }
.CodeMirror-vscrollbar { right: 0px; top: 0px; overflow: hidden; }
.CodeMirror-hscrollbar { bottom: 0px; left: 0px; overflow: auto hidden; }
.CodeMirror-scrollbar-filler { right: 0px; bottom: 0px; }
.CodeMirror-gutter-filler { left: 0px; bottom: 0px; }
.CodeMirror-gutters { position: absolute; left: 0px; top: 0px; padding-bottom: 10px; z-index: 3; overflow-y: hidden; }
.CodeMirror-gutter { white-space: normal; height: 100%; box-sizing: content-box; padding-bottom: 30px; margin-bottom: -32px; display: inline-block; }
.CodeMirror-gutter-wrapper { position: absolute; z-index: 4; border: none !important; background-position: 0px 0px !important; }
.CodeMirror-gutter-background { position: absolute; top: 0px; bottom: 0px; z-index: 4; }
.CodeMirror-gutter-elt { position: absolute; cursor: default; z-index: 4; }
.CodeMirror-lines { cursor: text; }
.CodeMirror pre { border-radius: 0px; border-width: 0px; font-family: inherit; font-size: inherit; margin: 0px; white-space: pre; word-wrap: normal; color: inherit; z-index: 2; position: relative; overflow: visible; background-position: 0px 0px; }
.CodeMirror-wrap pre { word-wrap: break-word; white-space: pre-wrap; word-break: normal; }
.CodeMirror-code pre { border-right-width: 30px; border-right-style: solid; border-right-color: transparent; width: fit-content; }
.CodeMirror-wrap .CodeMirror-code pre { border-right-style: none; width: auto; }
.CodeMirror-linebackground { position: absolute; inset: 0px; z-index: 0; }
.CodeMirror-linewidget { position: relative; z-index: 2; overflow: auto; }
.CodeMirror-wrap .CodeMirror-scroll { overflow-x: hidden; }
.CodeMirror-measure { position: absolute; width: 100%; height: 0px; overflow: hidden; visibility: hidden; }
.CodeMirror-measure pre { position: static; }
.CodeMirror div.CodeMirror-cursor { position: absolute; visibility: hidden; border-right-style: none; width: 0px; }
.CodeMirror div.CodeMirror-cursor { visibility: hidden; }
.CodeMirror-focused div.CodeMirror-cursor { visibility: inherit; }
.cm-searching { background-color: rgba(255, 255, 0, 0.4); }
span.cm-underlined { text-decoration: underline; }
span.cm-strikethrough { text-decoration: line-through; }
.cm-tw-syntaxerror { color: rgb(255, 255, 255); background-color: rgb(153, 0, 0); }
.cm-tw-deleted { text-decoration: line-through; }
.cm-tw-header5 { font-weight: 700; }
.cm-tw-listitem:first-child { padding-left: 10px; }
.cm-tw-box { border-style: solid; border-right-width: 1px; border-bottom-width: 1px; border-left-width: 1px; border-color: inherit; border-top-width: 0px !important; }
.cm-tw-underline { text-decoration: underline; }
@media print {
  .CodeMirror div.CodeMirror-cursor { visibility: hidden; }
}


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
</style><script type="text/javascript" src="./Guided Lab Creating a Virtual Private Cloud_files/c7fa7451-6f95-4815-ac32-b8cc2537837a" data-awssuidacr="53831616-c450-4d58-b234-a61f3b697d56"></script><title>README</title>
</head>
<body class="typora-export vsc-initialized"><div class="typora-export-content">
<div id="write" class=""><h1 id="module-6---guided-lab-creating-a-virtual-private-cloud"><span>Module 6 - Guided Lab: Creating a Virtual Private Cloud</span></h1><!-- ILT-TF-200-ACACAD-2 orig source: ILT-TF-100-ARCHIT-6 branch dev_65 --><h2 id="lab-overview-and-objectives"><span>Lab overview and objectives</span></h2><p><span>Traditional networking is difficult. It involves equipment, cabling, complex configurations, and specialist skills. Amazon Virtual Private Cloud (Amazon VPC) hides the complexity, and simplifies the deployment of secure private networks.</span></p><p><span>This lab shows you how to build your own virtual private cloud (VPC), deploy resources, and create private peering connections between VPCs.</span></p><p><span>After completing this lab, you should be able to:</span></p><ul><li><p><span>Deploy a VPC</span></p></li><li><p><span>Create an internet gateway and attach it to the VPC</span></p></li><li><p><span>Create a public subnet</span></p></li><li><p><span>Create private subnet</span></p></li><li><p><span>Create an application server to test the VPC</span></p><p>&nbsp;</p></li></ul><h2 id="duration"><span>Duration</span></h2><p><span>This lab will require approximately </span><strong><span>30 minutes</span></strong><span> to complete.</span></p><p>&nbsp;</p><h2 id="aws-service-restrictions"><span>AWS service restrictions</span></h2><p><span>In this lab environment, access to AWS services and service actions might be restricted to the ones that are needed to complete the lab instructions. You might encounter errors if you attempt to access other services or perform actions beyond the ones that are described in this lab.</span></p><p>&nbsp;</p><p><span>At the </span><strong><span>end</span></strong><span> of this lab, your architecture will look like the following example:</span></p><p><img src="./Guided Lab Creating a Virtual Private Cloud_files/module-6-guided-lab-architecture.png" referrerpolicy="no-referrer" alt="Architecture"></p><p>&nbsp;</p><h2 id="accessing-the-aws-management-console"><span>Accessing the AWS Management Console</span></h2><p>&nbsp;</p><ol start=""><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> to launch your lab.</span></p><p><span>A </span><strong><span>Start Lab</span></strong><span> panel opens, and it displays the lab status.</span></p><p><i class="fas fa-info-circle"></i><span> </span><strong><span>Tip</span></strong><span>: If you need more time to complete the lab, restart the timer for the environment by choosing the </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> button again.</span></p><p>&nbsp;</p></li><li><p><span>Wait until the </span><strong><span>Start Lab</span></strong><span> panel displays the message </span><em><span>Lab status: ready</span></em><span>, then close the panel by choosing the </span><strong><span>X</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>AWS</span></span><span>.</span></p><p><span>This action opens the AWS Management Console in a new browser tab. The system automatically logs you in.</span></p><p><i class="fas fa-exclamation-triangle"></i><span> </span><strong><span>Tip</span></strong><span>: If a new browser tab does not open, a banner or icon is usually at the top of your browser with the message that your browser is preventing the site from opening pop-up windows. Choose the banner or icon, and then choose </span><strong><span>Allow pop-ups</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Arrange the </span><strong><span>AWS Management Console</span></strong><span> tab so that it displays alongside these instructions. Ideally, you will have both browser tabs open at the same time so that you can follow the lab steps more easily.</span></p><p><i class="fas fa-exclamation-triangle"></i><span> </span><strong><span>Do not change the Region unless specifically instructed to do so</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><h2 id="task-1-creating-a-vpc"><span>Task 1: Creating a VPC</span></h2><p><span>You will begin by using Amazon VPC to create a new </span><strong><span>virtual private cloud, or VPC</span></strong><span>.</span></p><p><span>A VPC is a virtual network that is dedicated to your Amazon Web Services (AWS) account. It is logically isolated from other virtual networks in the AWS Cloud. You can launch AWS resources, such as Amazon Elastic Compute Cloud (Amazon EC2) instances, into the VPC. You can configure the VPC by modifying its IP address range, and create subnets. You can also configure route tables, network gateways, and security settings.</span></p><p>&nbsp;</p><ol start="5"><li><p><span>In the search box to the right of </span><i class="fas fa-th"></i><span> </span><strong><span>Services</span></strong><span>, search for and choose </span><strong><span>VPC</span></strong><span> to open the VPC console.</span></p><p><span>The VPC console provides a wizard that can automatically create several VPC architectures. However, in this lab, you will create the VPC components manually.</span></p><p>&nbsp;</p></li><li><p><span>In the left navigation pane, choose </span><strong><span>Your VPCs</span></strong><span>.</span></p><p><span>A default VPC is provided so that you can launch resources as soon as you start using AWS. There is also a </span><strong><span>Shared VPC</span></strong><span> that you will use later in the lab. However, you will now create your own </span><em><span>Lab VPC</span></em><span>.</span></p><p><span>The VPC will have a Classless Inter-Domain Routing (CIDR) range of </span><strong><span>10.0.0.0/16</span></strong><span>, which includes all IP address that start with </span><strong><span>10.0.x.x</span></strong><span>. It contains over 65,000 addresses. You will later divide the addresses into separate </span><em><span>subnets</span></em><span>.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create VPC</span></span><span> and configure these settings:</span></p><ul><li><p><strong><span>Name tag:</span></strong><span> </span><code>Lab VPC</code></p></li><li><p><strong><span>IPv4 CIDR block:</span></strong><span> </span><code>10.0.0.0/16</code></p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create VPC</span></span></p><p><span>A message that you successfully created the VPC appears.</span></p></li></ul><p><span> </span></p></li><li><p><span>In the lower half of the page, choose the </span><strong><span>Tags</span></strong><span> tab.</span></p><p><span>Tags are useful for identifying resources. For example, you can use a tag to identify cost centers or different environments (such as development, test, or production).</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_white"><span>Actions</span><i class="fas fa-angle-down"></i></span><span> and select </span><strong><span>Edit VPC settings</span></strong><span>.</span></p><p><span>This option assigns a </span><em><span>friendly</span></em><span> Domain Name System (DNS) name to EC2 instances in the VPC, such as:</span></p><p><em><span>ec2-52-42-133-255.us-west-2.compute.amazonaws.com</span></em></p><p>&nbsp;</p></li><li><p><span>Select </span><i class="far fa-check-square"></i><strong><span>Enable DNS hostname</span></strong><span> and then choose </span><span id="ssb_orange"><span>Save</span></span><span> </span></p><p><span>Any EC2 instances that are launched into the VPC will now automatically receive a DNS hostname. You can also add a more meaningful DNS name (such as </span><em><span>app.example.com</span></em><span>) later by using Amazon Route 53.</span></p></li></ol><p>&nbsp;</p><h2 id="task-2-creating-subnets"><span>Task 2: Creating subnets</span></h2><p><span>A subnet is a subrange of IP addresses in the VPC. AWS resources can be launched into a specified subnet. Use a </span><em><span>public subnet</span></em><span> for resources that must be connected to the internet, and use a </span><em><span>private subnet</span></em><span> for resources that must remain isolated from the internet.</span></p><p><span>In this task, you will create a public subnet and a private subnet:</span></p><p><img src="./Guided Lab Creating a Virtual Private Cloud_files/module-6-guided-lab-task-2.png" referrerpolicy="no-referrer" alt="Subnets"></p><h3 id="creating-a-public-subnet"><span>Creating a public subnet</span></h3><p><span>The public subnet will be used for internet-facing resources.</span></p><p>&nbsp;</p><ol start="11"><li><p><span>In the left navigation pane, choose </span><strong><span>Subnets</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create subnet</span></span><span> and configure these settings:</span></p><ul><li><p><strong><span>VPC ID:</span></strong><span> </span><em><span>Lab VPC</span></em></p></li><li><p><strong><span>Subnet name:</span></strong><span> </span><code>Public Subnet</code></p></li><li><p><strong><span>Availability Zone:</span></strong><span> Select the </span><em><span>first</span></em><span> Availability Zone in the list (do </span><em><span>not</span></em><span> keep the No Preference default)</span></p></li><li><p><strong><span>IPv4 CIDR block:</span></strong><span> </span><code>10.0.0.0/24</code></p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create subnet</span></span></p><p><i class="fas fa-comment"></i><span> The VPC has a CIDR block of </span><em><span>10.0.0.0/16</span></em><span>, which includes all </span><em><span>10.0.x.x</span></em><span> IP addresses. The subnet you just created has a CIDR block of </span><em><span>10.0.0.0/24</span></em><span>, which includes all </span><em><span>10.0.0.x</span></em><span> IP addresses. They might look similar, but the subnet is smaller than the VPC because of the </span><em><span>/24</span></em><span> in the CIDR range.</span></p><p><span>You will now configure the subnet to automatically assign a public IP address for all instances that are launched in it.</span></p></li></ul><p>&nbsp;</p></li><li><p><span>Select </span><i class="far fa-check-square"></i><span> </span><strong><span>Public Subnet</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_white"><span>Actions</span><i class="fas fa-angle-down"></i></span><span> and select </span><strong><span>Edit subnet settings</span></strong><span>, then:</span></p><ul><li><p><span>Select </span><i class="far fa-check-square"></i><strong><span>Enable auto-assign public IPv4 address</span></strong></p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Save</span></span></p><p><i class="fas fa-comment"></i><span>Though this subnet is named </span><em><span>Public Subnet</span></em><span>, it is not yet public. A public subnet must have an internet gateway, which you attach in the next task.</span></p></li></ul></li></ol><p>&nbsp;</p><h3 id="creating-a-private-subnet"><span>Creating a private subnet</span></h3><p><span>The private subnet will be used for resources that must remain isolated from the internet.</span></p><p>&nbsp;</p><ol start="15"><li><p><span>Use what you just learned to create another subnet with these settings:</span></p><ul><li><p><strong><span>VPC ID:</span></strong><span> </span><em><span>Lab VPC</span></em></p></li><li><p><strong><span>Subnet name:</span></strong><span> </span><code>Private Subnet</code></p></li><li><p><strong><span>Availability Zone:</span></strong><span> Select the </span><em><span>first</span></em><span> Availability Zone in the list (do </span><em><span>not</span></em><span> keep the No Preference default)</span></p></li><li><p><strong><span>IPv4 CIDR block:</span></strong><span> </span><code>10.0.2.0/23</code></p><p><span>The CIDR block of </span><em><span>10.0.2.0/23</span></em><span> includes all IP addresses that start with </span><em><span>10.0.2.x</span></em><span> and </span><em><span>10.0.3.x</span></em><span>. This is twice as large as the public subnet because most resources should be kept private, unless they specifically must be accessible from the internet.</span></p><p><span>Your VPC now has two subnets. However, the public subnet is totally isolated and cannot communicate with resources outside the VPC. You will next configure the public subnet to connect to the internet via an internet gateway.</span></p></li></ul></li></ol><p>&nbsp;</p><h2 id="task-3-creating-an-internet-gateway"><span>Task 3: Creating an internet gateway</span></h2><p><span>An </span><em><span>internet gateway</span></em><span> is a horizontally scaled, redundant, and highly available VPC component. It allows communication between the instances in a VPC and the internet. It imposes no availability risks or bandwidth constraints on network traffic.</span></p><p><span>An internet gateway serves two purposes:</span></p><ul><li><span>To provide a target in route tables that connects to the internet</span></li><li><span>To perform network address translation (NAT) for instances that were assigned public IPv4 addresses</span></li></ul><p><span>In this task, you will create an internet gateway so that internet traffic can access the public subnet.</span></p><p>&nbsp;</p><ol start="16"><li><p><span>In the left navigation pane, choose </span><strong><span>Internet Gateways</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create internet gateway</span></span><span> and configure these settings:</span></p><ul><li><strong><span>Name tag:</span></strong><span> </span><code>Lab IGW</code></li><li><span>Choose </span><span id="ssb_orange"><span>Create internet gateway</span></span></li></ul><p><span>You can now attach the internet gateway to your </span><em><span>Lab VPC</span></em><span>.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_white"><span>Actions</span><i class="fas fa-angle-down"></i></span><span> then </span><strong><span>Attach to VPC</span></strong><span>, and configure these settings:</span></p><ul><li><p><strong><span>Available VPCs:</span></strong><span> Place you cursor in the search box, then select </span><em><span>Lab VPC</span></em><span> </span></p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Attach internet gateway</span></span></p><p><span>This action will attach the internet gateway to your </span><em><span>Lab VPC</span></em><span>. Though you created an internet gateway and attached it to your VPC, you must also configure the public subnet </span><em><span>route table</span></em><span> so it uses the internet gateway.</span></p><p>&nbsp;</p></li></ul></li></ol><h2 id="task-4-configuring-route-tables"><span>Task 4: Configuring route tables</span></h2><p><span>A </span><em><span>route table</span></em><span> contains a set of rules, called </span><em><span>routes</span></em><span>, that are used to determine where network traffic is directed. Each subnet in a VPC must be associated with a route table because the table controls the routing for the subnet. A subnet can only be associated with one route table at a time, but you can associate multiple subnets with the same route table.</span></p><p><span>To use an internet gateway, a subnet's route table must contain a route that directs internet-bound traffic to the internet gateway. If a subnet is associated with a route table that has a route to an internet gateway, it is known as a </span><em><span>public subnet</span></em><span>.</span></p><p><span>In this task, you will:</span></p><ul><li><p><span>Create a </span><em><span>public route table</span></em><span> for internet-bound traffic</span></p></li><li><p><span>Add a </span><em><span>route</span></em><span> to the route table to direct internet-bound traffic to the internet gateway</span></p></li><li><p><span>Associate the public subnet with the new route table</span></p><p>&nbsp;</p></li></ul><ol start="19"><li><p><span>In the left navigation pane, choose </span><strong><span>Route Tables</span></strong><span>.</span></p><p><span>Several route tables are displayed, but there is only one route table associated with </span><em><span>Lab VPC</span></em><span>. This route table routes traffic locally, so it is called a </span><em><span>private route table</span></em><span>.</span></p><p>&nbsp;</p></li><li><p><span>Scroll to the right so that you can see the </span><strong><span>VPC </span></strong><span> column, then expand the width of the column so that you can see which one is used by </span><strong><span>Lab VPC</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Scroll back to the left and select </span><i class="far fa-check-square"></i><span> the route table that shows </span><strong><span>Lab VPC</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>In the </span><strong><span>Name</span></strong><span> column, choose </span><i class="fas fa-pencil-alt"></i><span> then enter the name  </span><code>Private Route Table</code><span> and choose </span><i class="fas fa-check-circle"></i><span>.</span></p><p>&nbsp;</p></li><li><p><span>In the lower half of the page, choose the </span><strong><span>Routes</span></strong><span> tab.</span></p><p><span>There is only one route. It shows that all traffic that is destined for </span><em><span>10.0.0.0/16</span></em><span> (which is the range of the </span><em><span>Lab VPC</span></em><span>) will be routed </span><em><span>locally</span></em><span>. This route allows all subnets in a VPC to communicate with each other.</span></p><p><span>You will now create a new public route table to send public traffic to the internet gateway.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create route table</span></span><span> and configure these settings:</span></p><ul><li><strong><span>Name:</span></strong><span> </span><code>Public Route Table</code></li><li><strong><span>VPC:</span></strong><span> </span><em><span>Lab VPC</span></em></li><li><span>Choose </span><span id="ssb_orange"><span>Create route table</span></span></li></ul></li></ol><p><span>   </span></p><ol start="25"><li><p><span>In the </span><strong><span>Routes</span></strong><span> tab, choose </span><span id="ssb_white"><span>Edit routes</span></span></p><p><span>You will now add a route to direct internet-bound traffic (</span><em><span>0.0.0.0/0</span></em><span>) to the internet gateway.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_white"><span>Add route</span></span><span> then configure these settings:</span></p><ul><li><strong><span>Destination:</span></strong><span> </span><code>0.0.0.0/0</code></li><li><strong><span>Target:</span></strong><span> Select </span><em><span>Internet Gateway</span></em><span> and then, from the list, select </span><em><span>Lab IGW</span></em></li><li><span>Choose </span><span id="ssb_orange"><span>Save changes</span></span></li></ul><p><span>The last step is to </span><em><span>associate</span></em><span> this new route table with the public subnet.</span></p><p>&nbsp;</p></li><li><p><span>Choose the </span><strong><span>Subnet associations</span></strong><span> tab.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_white"><span>Edit subnet associations</span></span></p><p>&nbsp;</p></li><li><p><span>Select </span><i class="far fa-check-square"></i><span> the row with </span><strong><span>Public Subnet</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Save associations</span></span></p><p><span>The public subnet is now </span><em><span>public</span></em><span> because it has a route table entry that sends traffic to the internet via the internet gateway.</span></p><p><span>To summarize, you can create a public subnet by following these steps:</span></p><ul><li><span>Create an </span><em><span>internet gateway</span></em></li><li><span>Create a </span><em><span>route table</span></em></li><li><span>Add a </span><em><span>route</span></em><span> to the route table that directs </span><em><span>0.0.0.0/0</span></em><span> traffic to the internet gateway</span></li><li><span>Associate the route table with a </span><em><span>subnet</span></em><span>, which thus becomes a </span><em><span>public subnet</span></em></li></ul></li></ol><p>&nbsp;</p><h2 id="task-5-creating-a-security-group-for-the-application-server"><span>Task 5: Creating a security group for the application server</span></h2><p><span>A </span><em><span>security group</span></em><span> acts as a virtual firewall for instances to control inbound and outbound traffic. Security groups operate at the level of the </span><em><span>elastic network interface for the instance</span></em><span>. Security groups do not operate at the </span><em><span>subnet</span></em><span> level. Thus, each instance can have its own firewall that controls traffic. If you do not specify a particular security group at launch time, the instance is automatically assigned to the </span><em><span>default security group</span></em><span> for the VPC.</span></p><p><span>In this task, you will create a security group that allows users to access your application server via HTTP.</span></p><p>&nbsp;</p><ol start="31"><li><p><span>In the left navigation pane, choose </span><strong><span>Security Groups</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_orange"><span>Create security group</span></span><span> and configure these settings:</span></p><ul><li><strong><span>Security group name:</span></strong><span> </span><code>App-SG</code></li><li><strong><span>Description:</span></strong><span> </span><code>Allow HTTP traffic</code></li><li><strong><span>VPC:</span></strong><span> select the X to clear the default selection, then choose </span><em><span>Lab VPC</span></em></li><li><span>Scroll to the bottom and choose </span><span id="ssb_orange"><span>Create security group</span></span></li></ul></li></ol><p><span>    </span></p><ol start="33"><li><p><span>Verify the </span><strong><span>Inbound rules</span></strong><span> tab is selected below.</span></p><p><span>The settings for </span><strong><span>Inbound Rules</span></strong><span> determine what traffic is permitted to reach the instance. You will configure it to permit HTTP (port 80) traffic that comes from anywhere on the internet (</span><em><span>0.0.0.0/0</span></em><span>).</span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_white"><span>Edit inbound rules</span></span></p><p>&nbsp;</p></li><li><p><span>Choose </span><span id="ssb_white"><span>Add rule</span></span><span> and then configure these settings:</span></p><ul><li><strong><span>Type:</span></strong><span>  </span><em><span>HTTP</span></em></li><li><strong><span>Source type:</span></strong><span> </span><em><span>Anywhere-IPv4</span></em></li><li><strong><span>Description:</span></strong><span> </span><code>Allow web access</code></li><li><span>Choose </span><span id="ssb_orange"><span>Save rules</span></span></li></ul><p><span>You use this </span><em><span>App-SG</span></em><span> in the next task.</span></p><p>&nbsp;</p></li></ol><h2 id="task-6-launching-an-application-server-in-the-public-subnet"><span>Task 6: Launching an application server in the public subnet</span></h2><p><span>To test that your VPC is correctly configured, you will now launch an EC2 instance into the public subnet. You will also confirm that you can access the EC2 instance from the internet.</span></p><p>&nbsp;</p><ol start="36"><li><p><span>In the search box to the right of </span><i class="fas fa-th"></i><span> </span><strong><span>Services</span></strong><span>, search for and choose </span><strong><span>EC2</span></strong><span> to open the EC2 console.</span></p><p>&nbsp;</p></li><li><p><span>From the </span><span id="ssb_orange"><span>Launch instance</span></span><span> menu, choose </span><strong><span>Launch Instance</span></strong><span>. Configure these options:</span></p><ul><li><p><strong><span>Name</span></strong><span>: </span><code>App Server</code></p></li><li><p><span>In the list of available </span><em><span>Quick Start</span></em><span> AMIs, keep the default </span><strong><span>Amazon Linux</span></strong><span> selected. Also keep the specific default </span><strong><span>Amazon Linux 2023 AMI</span></strong><span> selected.</span></p></li><li><p><span>In the </span><em><span>Instance type</span></em><span> panel, keep the default </span><strong><span>t2.micro</span></strong><span> selected.</span></p></li><li><p><span>From the </span><strong><span>Key pair name</span></strong><span> menu, select </span><strong><span>vockey</span></strong><span>.</span></p></li><li><p><span>Next to Network settings, choose </span><span id="ssb_white"><span>Edit</span></span><span>, then configure: </span></p><ul><li><strong><span>Network:</span></strong><span> </span><em><span>Lab VPC</span></em></li><li><strong><span>Subnet:</span></strong><span> </span><em><span>Public Subnet</span></em></li></ul></li><li><p><span>Under Firewall (security groups), choose </span><i class="far fa-dot-circle"></i><span> </span><strong><span>Select an existing security group</span></strong><span>.</span></p><ul><li><span>For </span><strong><span>Common security groups</span></strong><span>, select </span><strong><span>App-SG</span></strong><span>.</span></li></ul></li><li><p><span>In the </span><em><span>Configure storage</span></em><span> section, keep the default settings.</span></p></li><li><p><span>Expand the </span><strong><span>Advanced details</span></strong><span> panel.</span></p></li><li><p><strong><span>IAM instance profile:</span></strong><span> </span><em><span>Inventory-App-Role</span></em><span> </span></p></li><li><p><span>For the </span><strong><span>Metadata version</span></strong><span> set to </span><strong><span>V1 and V2 (token optional)</span></strong><span>.</span></p></li><li><p><span>Scroll to the bottom of the page and then copy and paste the code shown below into the </span><strong><span>User data</span></strong><span> box:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash" style="break-inside: unset;"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 10.3375px; left: 4px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: none;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: none;"><div class="CodeMirror-measure"></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation" style=""><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-meta">#!/bin/bash</span></span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-comment"># Install Apache Web Server and PHP</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">dnf install <span class="cm-attribute">-y</span> httpd <span class="cm-builtin">wget</span> php-fpm php-mysqli php-json php php-devel</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">dnf install <span class="cm-attribute">-y</span> mariadb105-server</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-comment"># Download Lab files</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">wget</span> https://aws-tc-largeobjects.s3-us-west-2.amazonaws.com/ILT-TF-200-ACACAD-20-EN/mod6-guided/scripts/inventory-app.zip</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">unzip inventory-app.zip <span class="cm-attribute">-d</span> /var/www/html/</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-comment"># Download and install the AWS SDK for PHP</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">wget</span> https://github.com/aws/aws-sdk-php/releases/download/3.298.5/aws.zip</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">unzip <span class="cm-attribute">-o</span> aws.zip </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">unzip <span class="cm-attribute">-o</span> aws.zip <span class="cm-attribute">-d</span> /var/www/html/</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-comment"># Turn on web server</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">systemctl enable httpd</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">systemctl <span class="cm-builtin">start</span> httpd</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom: 0px solid transparent; top: 444px;"></div><div class="CodeMirror-gutters" style="display: none; height: 444px;"></div></div></div></pre></li><li><p><span>At the bottom of the </span><strong><span>Summary</span></strong><span> panel on the right side of the screen choose </span><span id="ssb_orange"><span>Launch instance</span></span></p><p><span>You will see a Success message.</span></p><p>&nbsp;</p></li></ul></li><li><p><span>Choose </span><span id="ssb_orange"><span>View all instances</span></span></p><p>&nbsp;</p></li><li><p><span>Wait until the App Server instance shows </span><em><span>2/2 checks passed</span></em><span> in the </span><strong><span>Status check</span></strong><span> column.</span></p><p><i class="fas fa-comment"></i><span> This may take a few minutes. Choose the refresh </span><i class="fas fa-sync"></i><span> icon at the top of the page every 30 seconds or so to more quickly become aware of the latest status of the instance.</span></p><p>&nbsp;</p></li><li><p><span>Select </span><i class="far fa-check-square"></i><span> </span><strong><span>App Server</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Copy the </span><strong><span>Public IPv4 DNS</span></strong><span> value shown in the </span><strong><span>Details</span></strong><span> tab at the bottom of the page.</span></p><p>&nbsp;</p></li><li><p><span>Open a new web browser tab with that IP address.</span></p><p><span>If you configured the VPC correctly, the Inventory application and this message should appear: </span><em><span>Please configure Settings to connect to database</span></em><span>. You have not configured any database settings yet, but the appearance of the Inventory application demonstrates that the public subnet was correctly configured.</span></p><p><span style="color:red"><i class="fas fa-exclamation-triangle"></i></span><span> If the Inventory application does not appear, wait 60 seconds and refresh </span><i class="fas fa-sync"></i><span> the page to try again. It can take a couple of minutes for the EC2 instance to boot and run the script that installs the software.</span></p></li></ol><p>&nbsp;</p><h2 id="submitting-your-work"><span>Submitting your work</span></h2><ol start="43"><li><p><span>At the top of these instructions, choose </span><span id="ssb_blue"><span>Submit</span></span><span> to record your progress and when prompted, choose </span><span id="ssb_blue"><span>Yes</span></span><span>.</span></p><p>&nbsp;</p></li><li><p><span>If the results don't display after a minute, return to the top of these instructions and choose </span><span id="ssb_voc_grey"><span>Grades</span></span></p><p><strong><span>Tip</span></strong><span>: You can submit your work multiple times. After you change your work, choose </span><strong><span>Submit</span></strong><span> again. Your last submission is what will be recorded for this lab.</span></p><p>&nbsp;</p></li><li><p><span>To find detailed feedback on your work, choose </span><span id="ssb_voc_grey"><span>Details</span></span><span> followed by </span><i class="fas fa-caret-right"></i><span> </span><strong><span>View Submission Report</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><h2 id="lab-complete-i-classfas-fa-graduation-capi"><span>Lab complete </span><i class="fas fa-graduation-cap"></i></h2><p><i class="fas fa-flag-checkered"></i><span> Congratulations! You have completed the lab.</span></p><p>&nbsp;</p><ol start="46"><li><p><span>Choose </span><span id="ssb_voc_grey"><span>End Lab</span></span><span> at the top of this page, and then select </span><span id="ssb_orange"><span>Yes</span></span><span> to confirm that you want to end the lab.</span></p><p><span>A panel indicates that </span><em><span>DELETE has been initiated... You may close this message box now.</span></em></p><p>&nbsp;</p></li><li><p><span>Select the </span><strong><span>X</span></strong><span> in the top right corner to close the panel.</span></p></li></ol><p>&nbsp;</p><p><span>© 2022, Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.</span></p></div></div>
<script defer="" src="./Guided Lab Creating a Virtual Private Cloud_files/vcd15cbe7772f49c399c6a5babf22c1241717689176015" integrity="sha512-ZpsOmlRQV6y907TI0dKBHq9Md29nnaEIPlkf84rnaERnq6zvWvPUqr2ft8M1aS28oN72PdrCzSjY4U6VaAw1EQ==" data-cf-beacon="{&quot;rayId&quot;:&quot;8bafec9bec36010f&quot;,&quot;serverTiming&quot;:{&quot;name&quot;:{&quot;cfL4&quot;:true}},&quot;version&quot;:&quot;2024.8.0&quot;,&quot;token&quot;:&quot;a73834a4a1444e9ab89e8da06da41720&quot;}" crossorigin="anonymous"></script>

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