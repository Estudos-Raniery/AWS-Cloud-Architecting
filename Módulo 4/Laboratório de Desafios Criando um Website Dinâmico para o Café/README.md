<!DOCTYPE html>
<!-- saved from url=(0089)https://labs.vocareum.com/web/1964919/3231441.0/ASNLIB/public/docs/lang/en_us/README.html -->
<html foxified=""><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta name="viewport" content="width=device-width initial-scale=1">

<link href="./Challenge Lab Creating a Dynamic Website for the Café_files/css" rel="stylesheet" type="text/css"><style type="text/css">html {overflow-x: initial !important;}:root { --bg-color: #ffffff; --text-color: #333333; --select-text-bg-color: #B5D6FC; --select-text-font-color: auto; --monospace: "Lucida Console",Consolas,"Courier",monospace; --title-bar-height: 20px; }
.mac-os-11 { --title-bar-height: 28px; }
html { font-size: 14px; background-color: var(--bg-color); color: var(--text-color); font-family: "Helvetica Neue", Helvetica, Arial, sans-serif; -webkit-font-smoothing: antialiased; }
h1, h2, h3, h4, h5 { white-space: pre-wrap; }
body { margin: 0px; padding: 0px; height: auto; inset: 0px; font-size: 1rem; line-height: 1.428571; overflow-x: hidden; background: inherit; }
iframe { margin: auto; }
a.url { word-break: break-all; }
a:active, a:hover { outline: 0px; }
.in-text-selection, ::selection { text-shadow: none; background: var(--select-text-bg-color); color: var(--select-text-font-color); }
#write { margin: 0px auto; height: auto; width: inherit; word-break: normal; overflow-wrap: break-word; position: relative; white-space: normal; overflow-x: visible; padding-top: 36px; }
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
}
#write li > figure:last-child { margin-bottom: 0.5rem; }
#write ol, #write ul { position: relative; }
img { max-width: 100%; vertical-align: middle; image-orientation: from-image; }
button, input, select, textarea { color: inherit; font-style: inherit; font-variant-caps: inherit; font-weight: inherit; font-stretch: inherit; font-size: inherit; line-height: inherit; font-family: inherit; font-size-adjust: inherit; font-kerning: inherit; font-variant-alternates: inherit; font-variant-ligatures: inherit; font-variant-numeric: inherit; font-variant-east-asian: inherit; font-variant-position: inherit; font-variant-emoji: inherit; font-feature-settings: inherit; font-optical-sizing: inherit; font-variation-settings: inherit; }
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
thead, tr { break-inside: avoid; break-after: auto; }
thead { display: table-header-group; }
table { border-collapse: collapse; border-spacing: 0px; width: 100%; overflow: auto; break-inside: auto; text-align: left; }
table.md-table td { min-width: 32px; }
.CodeMirror-gutters { border-right-width: 0px; border-right-style: none; border-right-color: currentcolor; background-color: inherit; }
.CodeMirror-linenumber { -webkit-user-select: none; }
.CodeMirror { text-align: left; }
.CodeMirror-placeholder { opacity: 0.3; }
.CodeMirror pre { padding: 0px 4px; }
.CodeMirror-lines { padding: 0px; }
div.hr:focus { cursor: none; }
#write pre { white-space: pre-wrap; }
#write.fences-no-line-wrapping pre { white-space: pre; }
#write pre.ty-contain-cm { white-space: normal; }
.CodeMirror-gutters { margin-right: 4px; }
.md-fences { font-size: 0.9rem; display: block; break-inside: avoid; text-align: left; overflow: visible; white-space: pre; background: inherit; position: relative !important; }
.md-fences-adv-panel { width: 100%; margin-top: 10px; text-align: center; padding-top: 0px; padding-bottom: 8px; overflow-x: auto; }
#write .md-fences.mock-cm { white-space: pre-wrap; }
.md-fences.md-fences-with-lineno { padding-left: 0px; }
#write.fences-no-line-wrapping .md-fences.mock-cm { white-space: pre; overflow-x: auto; }
.md-fences.mock-cm.md-fences-with-lineno { padding-left: 8px; }
.CodeMirror-line, twitterwidget { break-inside: avoid; }
svg { break-inside: avoid; }
.footnotes { opacity: 0.8; font-size: 0.9rem; margin-top: 1em; margin-bottom: 1em; }
.footnotes + .footnotes { margin-top: 0px; }
.md-reset { margin: 0px; padding: 0px; border: 0px; outline: 0px; vertical-align: top; background: 0px 0px; text-decoration: none; text-shadow: none; float: none; position: static; width: auto; height: auto; white-space: nowrap; cursor: inherit; line-height: normal; font-weight: 400; text-align: left; box-sizing: content-box; direction: ltr; }
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
  #write { margin-top: 0px; border-color: transparent !important; padding-top: 0px !important; padding-bottom: 0px !important; }
  .typora-export * { print-color-adjust: exact; }
  .typora-export #write { break-after: avoid; }
  .typora-export #write::after { height: 0px; }
  .is-mac table { break-inside: avoid; }
  #write > p:nth-child(1) { margin-top: 0px; }
  .typora-export-show-outline .typora-export-sidebar { display: none; }
  figure { overflow-x: visible; }
}
.footnote-line { margin-top: 0.714em; font-size: 0.7em; }
a img, img a { cursor: pointer; }
pre.md-meta-block { font-size: 0.8rem; min-height: 0.8rem; white-space: pre-wrap; background: rgb(204, 204, 204); display: block; overflow-x: hidden; }
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
.md-task-list-item > input { position: absolute; top: 0px; left: 0px; margin-left: -1.2em; margin-top: calc(1em - 10px); border: medium; }
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
.reversefootnote { font-family: ui-monospace, sans-serif; }
.md-attr { display: none; }
.md-fn-count::after { content: "."; }
code, pre, samp, tt { font-family: var(--monospace); }
kbd { margin: 0px 0.1em; padding: 0.1em 0.6em; font-size: 0.8em; color: rgb(36, 39, 41); background: rgb(255, 255, 255); border: 1px solid rgb(173, 179, 185); border-radius: 3px; box-shadow: rgba(12, 13, 14, 0.2) 0px 1px 0px, rgb(255, 255, 255) 0px 0px 0px 2px inset; white-space: nowrap; vertical-align: middle; }
.md-comment { color: rgb(162, 127, 3); opacity: 0.6; font-family: var(--monospace); }
code { text-align: left; vertical-align: initial; }
a.md-print-anchor { white-space: pre !important; border-width: medium !important; border-style: none !important; border-color: currentcolor !important; display: inline-block !important; position: absolute !important; width: 1px !important; right: 0px !important; outline: 0px !important; background: 0px 0px !important; text-decoration: initial !important; text-shadow: initial !important; }
.os-windows.monocolor-emoji .md-emoji { font-family: "Segoe UI Symbol", sans-serif; }
.md-diagram-panel > svg { max-width: 100%; }
[lang="flow"] svg, [lang="mermaid"] svg { max-width: 100%; height: auto; }
[lang="mermaid"] .node text { font-size: 1rem; }
table tr th { border-bottom-width: 0px; border-bottom-style: none; border-bottom-color: currentcolor; }
video { max-width: 100%; display: block; margin: 0px auto; }
iframe { max-width: 100%; width: 100%; border: medium; }
.highlight td, .highlight tr { border: 0px; }
mark { background: rgb(255, 255, 0); color: rgb(0, 0, 0); }
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
.md-fences-advanced:not(.md-focus) { background: inherit; }
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
.outline-content li, .outline-content ul { margin-left: 0px; margin-right: 0px; padding-left: 0px; padding-right: 0px; list-style: none; overflow-wrap: anywhere; }
.outline-content ul { margin-top: 0px; margin-bottom: 0px; }
.outline-content strong { font-weight: 400; }
.outline-expander { width: 1rem; height: 1.428571rem; position: relative; display: table-cell; vertical-align: middle; cursor: pointer; padding-left: 4px; }
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
mjx-container { break-inside: avoid; }
.md-alert.md-alert-note { border-left-color: rgb(9, 105, 218); }
.md-alert.md-alert-important { border-left-color: rgb(130, 80, 223); }
.md-alert.md-alert-warning { border-left-color: rgb(154, 103, 0); }
.md-alert.md-alert-tip { border-left-color: rgb(31, 136, 61); }
.md-alert.md-alert-caution { border-left-color: rgb(207, 34, 46); }
.md-alert { padding: 0px 1em; margin-bottom: 16px; color: inherit; border-left-width: 0.25em; border-left-style: solid; border-left-color: rgb(0, 0, 0); }
.md-alert-text-note { color: rgb(9, 105, 218); }
.md-alert-text-important { color: rgb(130, 80, 223); }
.md-alert-text-warning { color: rgb(154, 103, 0); }
.md-alert-text-tip { color: rgb(31, 136, 61); }
.md-alert-text-caution { color: rgb(207, 34, 46); }
.md-alert-text { font-size: 0.9rem; font-weight: 700; }
.md-alert-text svg { fill: currentcolor; position: relative; top: 0.125em; margin-right: 1ch; overflow: visible; }
.md-alert-text-container::after { content: attr(data-text); text-transform: capitalize; pointer-events: none; margin-right: 1ch; }


.CodeMirror { height: auto; }
.CodeMirror.cm-s-inner { background: inherit; }
.CodeMirror-scroll { overflow: auto hidden; z-index: 3; }
.CodeMirror-gutter-filler, .CodeMirror-scrollbar-filler { background-color: rgb(255, 255, 255); }
.CodeMirror-gutters { border-right-width: 1px; border-right-style: solid; border-right-color: rgb(221, 221, 221); background: inherit; white-space: nowrap; }
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
.cm-s-inner .CodeMirror-activeline-background { background: inherit; }
.CodeMirror { position: relative; overflow: hidden; }
.CodeMirror-scroll { height: 100%; outline: 0px; position: relative; box-sizing: content-box; background: inherit; }
.CodeMirror-sizer { position: relative; }
.CodeMirror-gutter-filler, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-filler, .CodeMirror-vscrollbar { position: absolute; z-index: 6; display: none; outline: 0px; }
.CodeMirror-vscrollbar { right: 0px; top: 0px; overflow: hidden; }
.CodeMirror-hscrollbar { bottom: 0px; left: 0px; overflow: auto hidden; }
.CodeMirror-scrollbar-filler { right: 0px; bottom: 0px; }
.CodeMirror-gutter-filler { left: 0px; bottom: 0px; }
.CodeMirror-gutters { position: absolute; left: 0px; top: 0px; padding-bottom: 10px; z-index: 3; overflow-y: hidden; }
.CodeMirror-gutter { white-space: normal; height: 100%; box-sizing: content-box; padding-bottom: 30px; margin-bottom: -32px; display: inline-block; }
.CodeMirror-gutter-wrapper { position: absolute; z-index: 4; background: 0px 0px !important; border: medium !important; }
.CodeMirror-gutter-background { position: absolute; top: 0px; bottom: 0px; z-index: 4; }
.CodeMirror-gutter-elt { position: absolute; cursor: default; z-index: 4; }
.CodeMirror-lines { cursor: text; }
.CodeMirror pre { border-radius: 0px; border-width: 0px; background: 0px 0px; font-family: inherit; font-size: inherit; margin: 0px; white-space: pre; overflow-wrap: normal; color: inherit; z-index: 2; position: relative; overflow: visible; }
.CodeMirror-wrap pre { overflow-wrap: break-word; white-space: pre-wrap; word-break: normal; }
.CodeMirror-code pre { border-right-width: 30px; border-right-style: solid; border-right-color: transparent; width: fit-content; }
.CodeMirror-wrap .CodeMirror-code pre { border-right-width: medium; border-right-style: none; border-right-color: currentcolor; width: auto; }
.CodeMirror-linebackground { position: absolute; inset: 0px; z-index: 0; }
.CodeMirror-linewidget { position: relative; z-index: 2; overflow: auto; }
.CodeMirror-wrap .CodeMirror-scroll { overflow-x: hidden; }
.CodeMirror-measure { position: absolute; width: 100%; height: 0px; overflow: hidden; visibility: hidden; }
.CodeMirror-measure pre { position: static; }
.CodeMirror div.CodeMirror-cursor { position: absolute; visibility: hidden; border-right-width: medium; border-right-style: none; border-right-color: currentcolor; width: 0px; }
.CodeMirror div.CodeMirror-cursor { visibility: hidden; }
.CodeMirror-focused div.CodeMirror-cursor { visibility: inherit; }
.cm-searching { background: rgba(255, 255, 0, 0.4); }
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


:root {
    --side-bar-bg-color: #fafafa;
    --control-text-color: #777;
}

@include-when-export url(https://fonts.googleapis.com/css?family=Open+Sans:400italic,700italic,700,400&subset=latin,latin-ext);

/* open-sans-regular - latin-ext_latin */
  /* open-sans-italic - latin-ext_latin */
    /* open-sans-700 - latin-ext_latin */
    /* open-sans-700italic - latin-ext_latin */
  html {
    font-size: 16px;
    -webkit-font-smoothing: antialiased;
}

body {
    font-family: "Open Sans","Clear Sans", "Helvetica Neue", Helvetica, Arial, 'Segoe UI Emoji', sans-serif;
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
    color: #4183C4;
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

/*@media print {
    .typora-export h1,
    .typora-export h2 {
        border-bottom: none;
        padding-bottom: initial;
    }

    .typora-export h1::after,
    .typora-export h2::after {
        content: "";
        display: block;
        height: 100px;
        margin-top: -96px;
        border-top: 1px solid #eee;
    }
}*/

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
    color: #777;
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
    color: #777777;
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
    pre {
        page-break-inside: avoid;
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
    color: #777777;
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
    color: #a7a7a7;
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
    background-color: #FAFAFA;
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

.mac-os #write{
    caret-color: AccentColor;
}

.md-lang {
    color: #b4654d;
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
<script type="text/javascript" src="./Challenge Lab Creating a Dynamic Website for the Café_files/c7fa7451-6f95-4815-ac32-b8cc2537837a" data-awssuidacr="53831616-c450-4d58-b234-a61f3b697d56"></script></head>
<body class="typora-export vsc-initialized"><div class="typora-export-content">
<div id="write" class=""><link rel="stylesheet" href="./Challenge Lab Creating a Dynamic Website for the Café_files/all.css"><style type="text/css"><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="" style="break-inside: unset;"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang=""><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation" style=""><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_blue {</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #257ACF;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 5px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_services {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>background-color:#232f3e; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>font-weight:bold; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>font-size:90%; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>color:white; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>position:relative; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>top:-1px; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>padding-top:3px; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>padding-bottom:3px; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>padding-left:10px; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>padding-right:10px; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>margin-right:5px; </span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tab" role="presentation" cm-text="	">  </span>white-space:nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_catalog_orange {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #E36000;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_catalog_red {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #D90000;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 5px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_dark_blue {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: darkblue;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding: 0px 6px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_grafana_blue {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #00678b;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: #00678b;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 2px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_grafana_green {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #629300;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: #629300;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 2px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_grafana_orange {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #ec8427;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: #ec8427;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 2px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_grey {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #DEDEDE;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: #444;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 5px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-width: 1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-style: solid;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: #444;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_grey_square {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #DEDEDE;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: #444;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-width: 1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-style: solid;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: #444;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 2px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 2px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span cm-text="" cm-zwsp="">
</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_lambda_orange {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #ec7211;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_lambda_white {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: #545b64;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: #545b64;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 2px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-width: 1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-style: solid;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_maroon {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: darkred;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding: 0px 6px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_orange {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #ec7211;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: black;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssl_orange {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: #ec7211;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_orange_oval {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #ec7211;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 20px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_oval {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #DEDEDE;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: #444;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 20px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-width: 1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-style: solid;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: #444;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_start_lab {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #34A853;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 2px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_open_console {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: white;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-family: Google Sans;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-weight: bold;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: #1a73e8;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: #dadce0;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-radius: 4px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-width: 2px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-style: solid;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  outline-color: #ffffff;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 5px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 5px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">#ssb_voc_grey {</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  background-color: #F2F3F4;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  font-size: 90%;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  color: black;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  position: relative;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  top: -1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-top: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-bottom: 3px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-left: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  padding-right: 10px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-color: grey;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-width: 1px;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  border-style: solid;</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"> &nbsp;  white-space: nowrap</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">}</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 6187px;"></div><div class="CodeMirror-gutters" style="display: none; height: 6187px;"></div></div></div></pre></style><h1 id="module-4---challenge-lab-creating-a-dynamic-website-for-the-café"><span>Module 4 - Challenge Lab: Creating a Dynamic Website for the Café</span></h1><!--Note: the step-by-step solutions to the challenge sections of this lab can be found in the instructor guide (source document at https://awsu-coursebuild.s3-us-west-2.amazonaws.com/sourcefiles/CUR-TF-200-ACACAD-20-EN/IG/AcademyCloudArchitecting-IG-Module-04.docx)--><h2 id="scenario"><span>Scenario</span></h2><p><span>After the café launched the first version of their website, customers told the café staff how nice the website looks. However, in addition to the praise, customers often asked whether they could place online orders.</span></p><p><span>Sofía, Nikhil, Frank, and Martha discussed the situation. They agreed that their business strategy and decisions should focus on delighting their customers and providing them with the best possible café experience.</span></p><p>&nbsp;</p><h2 id="lab-overview-and-objectives"><span>Lab overview and objectives</span></h2><p><span>In this lab, you will deploy an application on an Amazon Elastic Compute Cloud (Amazon EC2) instance. The application enables the café to accept online orders. After testing that the application works as intended in the first AWS Region (the </span><em><span>development</span></em><span> environment), you will then create an Amazon Machine Image (AMI) from the EC2 instance. You will also deploy a second instance of the same application as the </span><em><span>production</span></em><span> environment in another AWS Region.</span></p><p><span>After completing this lab, you should be able to:</span></p><ul><li><p><span>Connect to the AWS Cloud9 IDE on an existing EC2 instance</span></p></li><li><p><span>Analyze the EC2 instance environment and confirm web server accessibility</span></p></li><li><p><span>Install a web application on an EC2 instance that also uses AWS Systems Manager Parameter Store</span></p></li><li><p><span>Test the web application</span></p></li><li><p><span>Create an AMI</span></p></li><li><p><span>Deploy a second copy of the web application to another AWS Region</span></p></li></ul><p>&nbsp;</p><p><span>When you </span><em><span>start</span></em><span> the lab, some resources are already created for you in the AWS account:</span></p><p><img src="./Challenge Lab Creating a Dynamic Website for the Café_files/m4ch-lab-start-arch.png" referrerpolicy="no-referrer" alt="start architecture"></p><p><span>At the </span><em><span>end</span></em><span> of this lab, your architecture should look like the following example:</span></p><p><img src="./Challenge Lab Creating a Dynamic Website for the Café_files/m4ch-lab-end-arch.png" referrerpolicy="no-referrer" alt="final architecture"></p><p>&nbsp;</p><h2 id="duration"><span>Duration</span></h2><p><span>This lab will require approximately </span><strong><span>60 minutes</span></strong><span> to complete.</span></p><p>&nbsp;</p><h2 id="aws-service-restrictions"><span>AWS service restrictions</span></h2><p><span>In this lab environment, access to AWS services and service actions might be restricted to the ones that are needed to complete the lab instructions. You might encounter errors if you attempt to access other services or perform actions beyond the ones that are described in this lab.</span></p><p>&nbsp;</p><h2 id="accessing-the-aws-management-console"><span>Accessing the AWS Management Console</span></h2><ol start=""><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> to launch your lab.</span></p><p><span>A </span><strong><span>Start Lab</span></strong><span> panel opens, and it displays the lab status.</span></p><p><strong><span>Tip</span></strong><span>: If you ever need more time to complete the lab that is displayed on the timer, choose the </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> button again to restart the timer for the environment. Doing so will not delete resources you have created.</span></p></li></ol><p>&nbsp;</p><ol start="2"><li><p><span>Wait until you see the message </span><em><span>Lab status: ready</span></em><span>, then close the </span><strong><span>Start Lab</span></strong><span> panel by choosing the </span><strong><span>X</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><ol start="3"><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>AWS</span></span><span>.</span></p><p><span>This opens the AWS Management Console in a new browser tab. The system will automatically log you in.</span></p><p><strong><span>Tip</span></strong><span>: If a new browser tab does not open, a banner or icon is usually at the top of your browser with the message that your browser is preventing the site from opening pop-up windows. Choose the banner or icon, and then choose </span><strong><span>Allow pop-ups</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><ol start="4"><li><p><span>Arrange the AWS Management Console tab so that it displays alongside these instructions. Ideally, you will have both browser tabs open at the same time so that you can follow the lab steps more easily.</span></p></li></ol><p>&nbsp;</p><h2 id="a-business-request-for-the-café-preparing-an-ec2-instance-to-host-a-website-challenge-1"><span>A business request for the café: Preparing an EC2 instance to host a website (Challenge #1)</span></h2><p><span>The café wants to introduce online ordering for customers, and enable café staff to view submitted orders. Their current website architecture, where the website is hosted on Amazon S3, does not support the new business requirements.</span></p><p><span>In the first part of this lab, you will take on the role of Sofía. You will configure an Amazon EC2 instance so that it is ready to host a website for the café.</span></p><p>&nbsp;</p><h3 id="task-1-analyzing-the-existing-ec2-instance"><span>Task 1: Analyzing the existing EC2 instance</span></h3><p><span>In this task, you will note details about an existing EC2 instance that was created for you in the AWS account.</span></p><ol start="5"><li><p><span>In the search box next to </span><i class="fas fa-th"></i><span> Services, search for and select </span><strong><span>EC2</span></strong><span>, to go to the EC2 console. Then choose </span><strong><span>Instances</span></strong><span>.</span></p><p><span>Notice the running instance named </span><em><span>aws-cloud9-CafeWebServer-...</span></em><span>. This EC2 instance was created when you started the lab.  </span></p><p><img src="./Challenge Lab Creating a Dynamic Website for the Café_files/ec2.png" referrerpolicy="no-referrer" alt="EC2 console"></p></li></ol><p>&nbsp;</p><h4 id="answering-questions-about-the-instance"><span>Answering questions about the instance</span></h4><p><span>Answers will be evaluated when you choose the blue </span><strong><span>Submit</span></strong><span> button at the end of the lab.</span></p><ol start="6"><li><p><span>Access the questions in this lab.</span></p><ul><li><p><span>Choose the </span><strong><span>Details</span></strong><span> menu, and choose </span><strong><span>Show</span></strong><span>.</span></p></li><li><p><span>Choose the </span><strong><span>Access the multiple choice questions</span></strong><span> link that appears at the bottom of the page.</span></p></li></ul></li></ol><p>&nbsp;</p><ol start="7"><li><p><span>In the page that you loaded, answer the first four questions:</span></p><ul><li><p><strong><span>Question 1</span></strong><span>: Is the instance in a public subnet?</span></p></li><li><p><strong><span>Question 2</span></strong><span>: Does the EC2 instance have an IPv4 public IP address assigned to it?</span></p></li><li><p><strong><span>Question 3</span></strong><span>: What inbound TCP port numbers are open for this instance?</span></p></li><li><p><strong><span>Question 4</span></strong><span>: Does the EC2 instance have an AWS Identity and Access Management (IAM) role associated with it?</span></p></li></ul><p><strong><span>Note</span></strong><span>: Leave the questions webpage open in your browser tab. You will return to it later in this lab.</span></p></li></ol><p>&nbsp;</p><h3 id="task-2-connecting-to-the-ide-on-the-ec2-instance"><span>Task 2: Connecting to the IDE on the EC2 instance</span></h3><p><span>AWS Cloud9 is service that can run on an EC2 instance. It provides an integrated development environment (IDE) that includes features such as a code editor, debugger, and terminal.</span></p><p><span>By using the AWS Cloud9 environment, you don't need to download a key pair and connect to the EC2 instance by using PuTTY or similar Secure Shell (SSH) software. By using AWS Cloud9, you also don't need to use command line text-editing tools (like vi or nano) to edit files on the Linux instance.</span></p><ol start="8"><li><p><span>In the search box next to </span><i class="fas fa-th"></i><span> Services, search for and select </span><strong><span>Cloud9</span></strong><span>, to go to the AWS Cloud9 console. </span></p><p><span>In the Environments page, notice the </span><em><span>CafeWebServer</span></em><span> environment. It indicates that it is of type </span><em><span>EC2 instance</span></em><span>.</span></p></li></ol><p>&nbsp;</p><ol start="9"><li><p><span>Choose </span><strong><span>Open</span></strong><span>.</span></p><p><span>You are now connected to the AWS Cloud9 IDE that is running on the EC2 instance that you observed earlier.</span></p><p><span>The IDE includes:</span></p><ul><li><p><span>A </span><em><span>Bash terminal</span></em><span> in the bottom-right panel.</span></p></li><li><p><span>A </span><em><span>file browser</span></em><span> in the left panel that shows files in the </span><code>/home/ec2-user/environment</code><span> directory on the instance.</span></p></li><li><p><span>A </span><em><span>file editor</span></em><span> in the upper-right panel. If you double-click a file in the file browser—such as the README.md file—it will display in the editor.</span></p></li></ul></li></ol><p><span>  </span><img src="./Challenge Lab Creating a Dynamic Website for the Café_files/cloud9.png" referrerpolicy="no-referrer" alt="AWS Cloud9"></p><p>&nbsp;</p><h3 id="task-3-analyzing-the-lamp-stack-environment-and-confirming-that-the-web-server-is-accessible"><span>Task 3: Analyzing the LAMP stack environment and confirming that the web server is accessible</span></h3><p><span>Recall that the objective of this challenge lab is configure an EC2 instance to host the new dynamic website for the café. In this task, you will analyze what is already installed.</span></p><ol start="10"><li><p><span>Observe the OS version.</span></p><p><span>In the AWS Cloud9 bash terminal, run this command:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">cat</span> /proc/version</span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre><p><span>Notice how the output indicates it is an Amazon Linux instance, roughly analogous to Red Hat 7.</span></p></li></ol><p>&nbsp;</p><ol start="11"><li><p><span>Observe the web server, database, and PHP details and server state.</span></p><p><span>In the terminal, run these commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> httpd <span class="cm-attribute">-v</span></span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> yum <span class="cm-attribute">-y</span> install httpd php-mbstring</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">service</span> httpd status</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">php <span class="cm-attribute">--version</span></span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 92px;"></div><div class="CodeMirror-gutters" style="display: none; height: 92px;"></div></div></div></pre><p><span>The output should show the versions of the web server and the database, and also show that they are not currently running.</span></p></li></ol><p>&nbsp;</p><ol start="12"><li><p><span>Start the web server and the database, and also set them to start automatically after any future EC2 instance restart.</span></p><p><span>In the terminal, run these commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation" style=""><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> chkconfig httpd on</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">service</span> httpd <span class="cm-builtin">start</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">service</span> httpd status</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-comment">#install database</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> yum install <span class="cm-attribute">-y</span> mariadb-server</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> mariadb <span class="cm-attribute">--version</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> systemctl enable mariadb</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-comment">#</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> chkconfig mariadb on</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">service</span> mariadb <span class="cm-builtin">start</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">service</span> mariadb status</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 253px;"></div><div class="CodeMirror-gutters" style="display: none; height: 253px;"></div></div></div></pre></li></ol><p>&nbsp;</p><ol start="13"><li><p><span>Configure the EC2 instance so that you can use the AWS Cloud9 editor to edit web server files.</span></p><p><span>Notice that the AWS Cloud9 file browser currently does not display the Apache web server default web directory.</span></p><p><span>In the terminal, run these two commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">ln</span> <span class="cm-attribute">-s</span> /var/www/ /home/ec2-user/environment</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">chown</span> ec2-user:ec2-user /var/www/html</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 46px;"></div><div class="CodeMirror-gutters" style="display: none; height: 46px;"></div></div></div></pre><p><span>The first command you ran created a symlink from the default AWS Cloud9 editor workspace to the </span><code>/var/www</code><span> directory that contains your web server files.</span></p><p><span>The second command changed ownership of the </span><strong><span>html</span></strong><span> subdirectory so that the </span><em><span>ec2-user</span></em><span> (which you are logged in as) can edit and create new files in it.</span></p></li></ol><p>&nbsp;</p><ol start="14"><li><p><span>Creating a simple test webpage.</span></p><ul><li><p><span>In the </span><em><span>file browser</span></em><span>, expand the </span><strong><span>CafeWebServer &gt; www</span></strong><span> directory, and highlight the </span><strong><span>html</span></strong><span> directory.</span></p></li><li><p><span>Choose </span><strong><span>File</span></strong><span> &gt; </span><strong><span>New File</span></strong><span>.</span></p></li><li><p><span>In the text editor tab, paste the following line:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="html"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="html"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-tag cm-bracket">&lt;</span><span class="cm-tag">html</span><span class="cm-tag cm-bracket">&gt;</span>Hello from the café web server!<span class="cm-tag cm-bracket">&lt;/</span><span class="cm-tag">html</span><span class="cm-tag cm-bracket">&gt;</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li><li><p><span>Choose </span><strong><span>File</span></strong><span> &gt; </span><strong><span>Save</span></strong><span>, and save the file in the </span><strong><span>html</span></strong><span> directory as </span><em><span>index.html</span></em><span>.</span></p></li></ul></li></ol><p>&nbsp;</p><ol start="15"><li><p><span>Make the website accessible from the internet.</span></p><p><span>In this step, you will need to verify and update the configurations that make the webpages (which are hosted on the web server) accessible from the internet.</span></p><p><span>Here are some tips to help you get started:</span></p></li></ol><details>
<summary>
<b>Tip #1</b> (click to expand)
</summary>
Discover the IPv4 public IP address of the EC2 instance, and try to load `http://&lt;public-ip&gt;` in a new browser tab. Does the message that you entered into index.html load in the browser?
</details><p>&nbsp;</p><details>
<summary>
<b>Tip #2</b> (click to expand)
</summary>To allow inbound HTTP traffic on TCP port 80 from anywhere, update the security group of the EC2 instance, as needed.
</details><p>&nbsp;</p><h2 id="new-business-requirement-installing-a-dynamic-website-application-on-the-ec2-instance-challenge-2"><span>New business requirement: Installing a dynamic website application on the EC2 instance (Challenge #2)</span></h2><p><span>In the previous challenge, you configured the EC2 instance. You now know that PHP is installed, and that the application environment has a running relational database. Also, the environment has a running web server that can be accessed from the internet. You now have the basic setup for hosting a dynamic website for the café.</span></p><p><span>In the second part of this lab, you will take on the role of Sofía, and install the café application on the EC2 instance.</span></p><p>&nbsp;</p><h3 id="task-4-installing-the-café-application"><span>Task 4: Installing the café application</span></h3><ol start="16"><li><p><span>Download and extract the web server application files.</span></p><p><span>In the Bash terminal, run these commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation" style=""><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">cd</span> ~/environment</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">wget</span> https://aws-tc-largeobjects.s3.us-west-2.amazonaws.com/CUR-TF-200-ACACAD-2-91555/04-lab-mod4-challenge-EC2/s3/setup.zip</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">unzip setup.zip</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">wget</span> https://aws-tc-largeobjects.s3.us-west-2.amazonaws.com/CUR-TF-200-ACACAD-2-91555/04-lab-mod4-challenge-EC2/s3/db.zip</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">unzip db.zip</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">wget</span> https://aws-tc-largeobjects.s3.us-west-2.amazonaws.com/CUR-TF-200-ACACAD-2-91555/04-lab-mod4-challenge-EC2/s3/cafe.zip</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 138px;"></div><div class="CodeMirror-gutters" style="display: none; height: 138px;"></div></div></div></pre></li></ol><p><span>Notice how the file browser now shows the three .tar.gz files that you downloaded.</span>
<span>  </span><br><span>You also extracted these archive files, which created the </span><code>cafe</code><span>, </span><code>db</code><span>, and </span><code>setup</code><span> directories in your work environment.</span></p><p>&nbsp;</p><ol start="17"><li><p><span>Copy the café files over to the web server document root.</span></p><p><span>In the Bash terminal, run this command:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">unzip cafe.zip <span class="cm-attribute">-d</span> /var/www/html/</span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li></ol><p>&nbsp;</p><ol start="18"><li><p><span>Observe how the application is designed to work.</span></p><ul><li><p><span>Open the </span><code>html/cafe/index.php</code><span> source code in the AWS Cloud9 editor by double-clicking it.</span></p></li><li><p><span>Notice that this file has HTML code in it, but it also contains sections that are enclosed in </span><em><!--?php ... ?--></em><span> elements. These elements make calls to other systems and resources.</span></p></li><li><p><span>For example, on </span><strong><span>line 18</span></strong><span>, you see that the PHP code references a file named </span><em><span>getAppParameters.php</span></em><span>.</span></p></li><li><p><span>Open the </span><strong><span>getAppParameters.php</span></strong><span> file in the code editor.</span></p></li><li><p><span>Notice on </span><strong><span>line 3</span></strong><span> of this file that the </span><em><span>AWSSDK</span></em><span> is invoked.</span></p></li><li><p><span>Also, on </span><strong><span>lines 10–33</span></strong><span>, the web application creates a client that connects to the </span><em><span>ssm</span></em><span> service, which is AWS Systems Manager. The application then retrieves seven parameters from Systems Manager. Those parameters have not been created in AWS Systems Manager yet, but you will do that next.</span></p></li></ul></li></ol><p>&nbsp;</p><ol start="19"><li><p><span>In the AWS Systems Manager Parameter Store, configure the application parameters.</span></p><p><span>In the Bash terminal, run these commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">cd</span> setup</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">./set-app-parameters.sh</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 46px;"></div><div class="CodeMirror-gutters" style="display: none; height: 46px;"></div></div></div></pre><p><span>The shell script that you just ran issued AWS Command Line Interface (AWS CLI) commands. These commands added the parameters that the application will use to the Parameter Store.</span></p></li></ol><p>&nbsp;</p><ol start="20"><li><p><span>In the AWS Management Console, from the </span><strong><span>Services</span></strong><span> menu, choose </span><strong><span>Systems Manager</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><ol start="21"><li><p><span>From the panel on the left, choose </span><strong><span>Parameter Store</span></strong><span>.</span></p><p><span>Notice how there are now seven parameters stored here.</span></p><p><span>The café application's PHP code references these values (for example, so that it can retrieve the connection information for the MySQL database).</span></p><p><span>Choose the </span><code>/cafe/dbPassword</code><span> parameter, and copy the </span><em><span>Value</span></em><span> to your clipboard. You will use this value in a moment.</span></p></li></ol><p>&nbsp;</p><ol start="22"><li><p><span>Configure the MySQL database to support the café application.</span></p><p><span>Back in the AWS Cloud9 bash terminal, run the following commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">cd</span> ../db/</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">./set-root-password.sh</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">./create-db.sh</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 69px;"></div><div class="CodeMirror-gutters" style="display: none; height: 69px;"></div></div></div></pre></li></ol><p>&nbsp;</p><ol start="23"><li><p><span>Observe the database tables that were created.</span></p><p><span>In the Bash terminal, run this command to connect the terminal-based MySQL client to the database:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">mysql <span class="cm-attribute">-u</span> admin <span class="cm-attribute">-p</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre><p><span>When you are prompted for the database password, paste the </span><em><span>dbPassword</span></em><span> parameter value that you copied.</span></p><p><span>You should now see a  </span><code>mysql&gt;</code><span> prompt, which indicates that you are now connected to the MySQL database that runs on this EC2 instance.</span></p></li></ol><p><span>  </span><img src="./Challenge Lab Creating a Dynamic Website for the Café_files/db-client.png" referrerpolicy="no-referrer" alt="database-client"></p><p>&nbsp;</p><p><span>To observe the contents of the database (specifically, the tables that support the café web application), enter the following commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="sql"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="sql"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation" style=""><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">show</span> <span class="cm-keyword">databases</span><span class="cm-punctuation">;</span></span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">use</span> cafe_db<span class="cm-punctuation">;</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">show</span> <span class="cm-keyword">tables</span><span class="cm-punctuation">;</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">select</span> <span class="cm-operator">*</span> <span class="cm-keyword">from</span> product<span class="cm-punctuation">;</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">exit</span><span class="cm-punctuation">;</span></span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 115px;"></div><div class="CodeMirror-gutters" style="display: none; height: 115px;"></div></div></div></pre><p>&nbsp;</p><ol start="24"><li><p><span>Update the </span><em><span>timezone</span></em><span> configuration in PHP.</span></p><p><span>In the Bash terminal, run the following commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">sed</span> <span class="cm-attribute">-i</span> <span class="cm-string">"2i date.timezone = \"America/New_York\" "</span> /etc/php.ini</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">service</span> httpd <span class="cm-builtin">restart</span></span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 46px;"></div><div class="CodeMirror-gutters" style="display: none; height: 46px;"></div></div></div></pre><p><span>The first command that you ran configured the time zone in the PHP software.</span></p><p><span>The second command that you ran restarted the web server so that the web server notices the configuration update.</span></p></li></ol><p>&nbsp;</p><ol start="25"><li><p><span>Test whether the café website is working and can be accessed from the internet.</span></p><p><span>In a new browser tab, try to load the application at </span><code>http://&lt;public-ip&gt;/cafe</code><span> where &lt;</span><em><span>public-ip</span></em><span>&gt; is the IPv4 public IP address of the EC2 instance.</span></p><p><span>You will see that </span><em><span>only the title banner</span></em><span> of the website loads. The rest of the webpage is not loading correctly.</span></p></li></ol><p>&nbsp;</p><ol start="26"><li><p><span>Resolve an issue with the website.</span></p><p><span>In this step, you will need to figure out how to make the café website function correctly.</span></p><p><span>Here's a list of what </span><em><span>does</span></em><span> work:</span></p><ul><li><p><span>The test page at </span><em><a href="http://&amp;lt;public-ip/" target="_blank" class="url" rel="noopener noreferrer">http://&lt;public-ip</a><span>&gt;/</span></em><span> loads, so you know that the web server works, and is accessible from the internet</span></p></li><li><p><span>You also know that the MySQL database is running, and contains tables and data to support the application</span></p></li></ul></li></ol><p><span>What could be the issue?</span></p><details>
<summary>
<b>Tip #1</b> (click to expand)
</summary>
There is nothing wrong with the PHP code as written. The issue is related to permissions.
</details><details>
<summary>
<b>Tip #2</b> (click to expand)
</summary>
Does the web application rely on any other services or resources in addition to the web server and the database? For example, does it require access to another AWS service?
</details><details>
<summary>
<b>Tip #3</b> (click to expand)
</summary>
Go to the IAM service and search for the IAM role that is named <b>CafeRole</b>. Observe the permissions that this role grants. Would it be helpful to have these rights granted to the EC2 instance? How could you grant these permissions to the café web application?
</details><details>
<summary>
<b>Tip #4</b> (click to expand)
</summary>
 Select the EC2 instance in the Amazon EC2 console, and review the options on the <b>Actions</b> menu. Would any of the actions help solve the issue?
</details><p>&nbsp;</p><p><span>When you think you have fixed the issue, load the </span><code>http://&lt;public-ip&gt;/cafe</code><span> page again. Does it load completely so that you can see the café menu items? If so, congratulations!</span></p><p><strong><span>Note</span></strong><span>: If you still can't solve the issue, you might find it helpful to run the grading script as documented in the </span><strong><span>Submitting your work</span></strong><span> section at the end of these lab instructions. The Submission Report that is generated can provide additional tips for parts of the lab that you didn't complete successfully. You can submit your work as many times as you like—only the score that you achieve on the last submission will be retained.</span></p><p>&nbsp;</p><h3 id="task-5-testing-the-web-application"><span>Task 5: Testing the web application</span></h3><ol start="27"><li><p><span>Test by placing an order.</span></p><ul><li><p><span>In the browser tab where you have the </span><code>http://&lt;public-ip&gt;/cafe</code><span> page open, choose </span><strong><span>Menu</span></strong><span>.</span></p></li><li><p><span>Submit an order for at least one of the menu items displayed.</span></p><ul><li><p><span>Note: you may need to scroll down to find the </span><strong><span>Submit Order</span></strong><span> button.</span></p></li></ul></li><li><p><span>Return to the menu page and place another order, then go to the </span><strong><span>Order History</span></strong><span> page to see the order details for all the orders that you placed.</span></p></li></ul></li></ol><p>&nbsp;</p><h2 id="new-business-requirement-creating-development-and-production-websites-in-different-aws-regions-challenge-3"><span>New business requirement: Creating development and production websites in different AWS Regions (Challenge #3)</span></h2><p><img src="./Challenge Lab Creating a Dynamic Website for the Café_files/sofie.png" referrerpolicy="no-referrer" alt="Sofía"></p><p>&nbsp;</p><p><span>Everyone at the café is impressed with the new dynamic website that Sofía created! Customers are delighted that they can now place online orders and schedule dessert items for pickup. Customer satisfaction has increased because of the reduced customer wait times.  </span></p><p><span>However, another business requirement emerges, along with the praise. Martha and Frank would like to have </span><em><span>two</span></em><span> café websites:</span></p><ul><li><p><span>One website that can be used as a </span><em><span>development environment</span></em><span> to mock up new features and web designs before they are released to customers</span></p></li><li><p><span>A separate website that will host the </span><em><span>production environment</span></em><span> that customers use</span></p></li></ul><p><span>Sofía discussed the new requirement with Mateo when he came into the café one morning for his coffee. He suggested that, ideally, the two environments would exist in </span><em><span>different AWS Regions</span></em><span>. Such a design would have the added benefit of providing more robust disaster recovery (DR) in the unlikely scenario when an AWS Region becomes temporarily unavailable.</span></p><p><span>Sofía is now very busy! As she accomplishes more impressive work, her skills become more in-demand.</span></p><p>&nbsp;</p><h3 id="task-6-creating-an-ami-and-launching-another-ec2-instance"><span>Task 6: Creating an AMI and launching another EC2 instance</span></h3><p><span>Because the café website already runs well on an existing EC2 instance, Sofía decides to duplicate it by creating an AMI from it. She will then launch a new instance from the new AMI.</span></p><p><span>You will continue to take on the role of Sofía for this task. Before you create an AMI out of this instance, you should create a new key pair, which might be important to have later in this lab.</span></p><ol start="28"><li><p><span>Set a static internal hostname and create a new key pair on the EC2 instance.</span></p><p><span>In the bash terminal, run the following commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> hostname cafeserver</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">ssh-keygen <span class="cm-attribute">-t</span> rsa <span class="cm-attribute">-f</span> ~/.ssh/id_rsa</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 46px;"></div><div class="CodeMirror-gutters" style="display: none; height: 46px;"></div></div></div></pre><p><span>For the two times that you are prompted for a passphrase, press the ENTER key.</span></p><p><span>To make the new key available to the SSH utilities, in the Bash terminal, run the following command:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">cat</span> ~/.ssh/id_rsa.pub &gt;&gt; ~/.ssh/authorized_keys</span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li></ol><p>&nbsp;</p><ol start="29"><li><p><span>In the AWS Management Console, browse to the </span><strong><span>EC2</span></strong><span> service area and select the instance.</span></p></li></ol><p>&nbsp;</p><ol start="30"><li><p><span>Choose </span><strong><span>Actions &gt; Images and templates &gt; Create Image</span></strong><span>.</span></p><p><strong><span>Tip</span></strong><span>: Leave the </span><strong><span>Create Image</span></strong><span> dialog open in the browser tab while you answer some questions about AMIs.</span></p></li></ol><p>&nbsp;</p><h4 id="answering-questions-about-amis"><span>Answering questions about AMIs</span></h4><p><span>Answers will be recorded when you choose the blue </span><strong><span>Submit</span></strong><span> button at the end of the lab.</span></p><ol start="31"><li><p><span>Return to the browser tab that has the questions for this lab. You accessed this tab earlier.</span></p><p><span>If you need to find the page again:</span></p><ul><li><p><span>Choose the </span><strong><span>Details</span></strong><span> menu, and choose </span><strong><span>Show</span></strong><span>.</span></p></li><li><p><span>Choose the </span><strong><span>Access the multiple choice questions</span></strong><span> link that appears at the bottom of the page.</span></p></li></ul></li></ol><p>&nbsp;</p><ol start="32"><li><p><span>In the page, submit answers to the following questions:</span></p><ul><li><p><strong><span>Question 5</span></strong><span>: When you create an AMI from an instance, will the instance be rebooted?</span></p></li><li><p><strong><span>Question 6</span></strong><span>: In what ways can you modify the root volume properties when you create an AMI from an instance?</span></p></li><li><p><strong><span>Question 7</span></strong><span>: Can you add more volumes to an AMI that you create from an instance that only has one volume?</span></p></li></ul></li></ol><p>&nbsp;</p><ol start="33"><li><p><span>Back in the AWS Management Console, in the </span><strong><span>Create Image</span></strong><span> screen, create the new AMI:</span></p><ul><li><p><strong><span>Image name</span></strong><span>: </span><code>CafeServer</code></p></li><li><p><span>Choose </span><strong><span>Create Image</span></strong></p></li></ul></li></ol><p>&nbsp;</p><ol start="34"><li><p><span>From the navigation menu,  choose </span><strong><span>AMIs</span></strong><span> and wait until the image status becomes </span><em><span>Available</span></em><span>. The process typically takes about 2 minutes. You may need to expand </span><strong><span>Images</span></strong><span> to find </span><strong><span>AMIs</span></strong><span>.</span></p><p>&nbsp;</p></li><li><p><span>Create an AMI in another AWS Region</span></p><p><span>In this step, your objective is to create a new EC2 instance from the AMI that you just captured. However, you must create the new instance in the Oregon (us-west-2) AWS Region.</span></p></li></ol><details>
<summary>
<b>Tip #1</b> (click to expand)
</summary>
Copy the AMI ID of the image that you just created. Then, try to find it in the us-west-2 Region.
</details><details>
<summary>
<b>Tip #2</b> (click to expand)
</summary>
Do AMIs exist at the account level?
</details><details>
<summary>
<b>Tip #3</b> (click to expand)
</summary>
Select the AMI you that you created in the AWS Region where you created it. Next, choose the <b>Actions</b> menu. Do any actions seem like they could help you make the AMI available in the US West (Oregon) Region? Go ahead and choose the appropriate action. After you initiate it, the action might take up to 5 minutes to complete. Choose the refresh icon occasionally to know more quickly when it has completed.
</details><p>&nbsp;</p><ol start="36"><li><p><span>Create the new café instance from your AMI. The new instance that you create must match the following criteria.</span></p><ul><li><p><strong><span>Region</span></strong><span>: </span><code>Oregon</code></p></li><li><p><strong><span>Instance Size</span></strong><span>: </span><code>t2.small</code></p></li><li><p><strong><span>Network</span></strong><span>: </span><code>Lab VPC Region 2</code><span>, </span><code>Public Subnet</code></p></li><li><p><strong><span>IAM Role</span></strong><span>: </span><code>CafeRole</code></p></li><li><p><span>Tag:</span></p><ul><li><p><strong><span>Key</span></strong><span>: </span><code>Name</code></p></li><li><p><strong><span>Value</span></strong><span>: </span><code>ProdCafeServer</code></p></li></ul></li><li><p><span>Security Group:</span></p><ul><li><p><span>Create a new one named </span><strong><span>cafeSG</span></strong><span>, with TCP port </span><strong><span>22</span></strong><span> open to anywhere</span></p></li><li><p><span>Set TCP port </span><strong><span>80</span></strong><span> so that it's open to anywhere as well</span></p></li></ul></li><li><p><strong><span>Proceed without a key pair</span></strong><span> (the key pair that you created earlier in this lab should work to connect to it, if necessary)</span></p></li></ul></li></ol><p>&nbsp;</p><ol start="37"><li><p><span>Wait for the new instance to have a </span><em><span>Public DNS</span></em><span> value assigned to it, even if the status of the instance is still not </span><em><span>Available</span></em><span>.</span></p></li></ol><p>&nbsp;</p><ol start="38"><li><p><span>Copy the </span><strong><span>Public DNS</span></strong><span> value. You will use it soon.</span></p></li></ol><p>&nbsp;</p><ol start="39"><li><p><span>To create the needed </span><em><span>AWS Systems Manager parameters</span></em><span> in the new AWS Region, complete these steps.</span></p><ul><li><p><span>Return to the AWS Cloud9 IDE in the </span><strong><span>N. Virginia (us-east-1)</span></strong><span> Region.</span></p></li><li><p><span>Open the CafeWebServer/setup/</span><strong><span>set-app-parameters.sh</span></strong><span> file in the text editor.</span></p></li><li><p><span>Edit </span><strong><span>line 12</span></strong><span> of the file to match this setting:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-def">region</span><span class="cm-operator">=</span><span class="cm-string">"us-west-2"</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li><li><p><span>Edit </span><strong><span>line 18</span></strong><span> to match this setting (where &lt;</span><em><span>public-dns-of-ProdCafeServer-instance</span></em><span>&gt; is the actual DNS of the ProdCafeServer instance):</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-def">publicDNS</span><span class="cm-operator">=</span><span class="cm-string">"&lt;public-dns-of-ProdCafeServer-instance&gt;"</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li></ul><p><strong><span>Note</span></strong><span>: The line should still contain the quotation marks, but it should </span><em><span>not</span></em><span> contain the angle brackets (&lt; &gt;).</span></p></li></ol><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang=""><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang=""><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">This example shows what line 12 should look like and how line 18 should be formatted. However, the value of your public DNS will be different.</span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 46px;"></div><div class="CodeMirror-gutters" style="display: none; height: 46px;"></div></div></div></pre><p><img src="./Challenge Lab Creating a Dynamic Website for the Café_files/php-file.png" referrerpolicy="no-referrer" alt="php-file"></p><ul><li><p><strong><span>File &gt; Save</span></strong><span> the change.</span></p></li><li><p><span>To run this script, go to the top of the IDE and choose the </span><strong><span>Run</span></strong><span> button.</span></p></li></ul><p><span>In the Bash terminal below the text editor, you should see output that's formatted in JavaScript Object Notation (JSON). This output indicates that the parameters script ran successfully.</span></p><details>
<summary>If the script encountered an issue, click here to view troubleshooting tips.</summary>
If the output of the command indicates that the credentials are expired, try running these commands in the Bash terminal (and then run the set-app-parameters.sh again):
<br><code>wget https://aws-tc-largeobjects.s3-us-west-2.amazonaws.com/ILT-TF-200-ACACAD-20-EN/mod4-challenge/cred-update.sh</code><br>
<code>chmod +x cred-update.sh</code><br>
<code>./cred-update.sh</code>
</details><p><strong><span>Note</span></strong><span>: By changing the AWS Region details and running this script again, you created the same parameters that you created earlier in the us-east-1 Region of the AWS Systems Manager Parameter Store. However, this time, you created these parameters in the Oregon Region.</span></p><p>&nbsp;</p><h3 id="task-7-verifying-the-new-café-instance"><span>Task 7: Verifying the new café instance  </span></h3><ol start="40"><li><p><span>Return to the EC2 Console in the </span><strong><span>Oregon</span></strong><span> Region, and verify that the new </span><strong><span>ProdCafeServer</span></strong><span> instance is running.</span></p></li></ol><p>&nbsp;</p><ol start="41"><li><p><span>Copy the IPv4 public IP address, and load it in a web browser.</span></p><p><span>The </span><em><span>Hello from the cafe web server!</span></em><span> message should display.</span></p></li></ol><p>&nbsp;</p><ol start="42"><li><p><span>Load the </span><code>http://&lt;public-ip&gt;/cafe/</code><span> URL in a browser tab.</span></p><p><span>The entire café website should display.</span></p></li></ol><p>&nbsp;</p><ol start="43"><li><p><span>Load the </span><strong><span>Menu</span></strong><span> page.</span></p><p><span>The full </span><em><span>Menu</span></em><span> page should load, and the order-placing functionality should work.</span></p></li></ol><p>&nbsp;</p><ol start="44"><li><p><span>Place an order to verify that the website is working as intended.</span></p></li></ol><p>&nbsp;</p><ol start="45"><li><p><span>Troubleshooting tips (skip this one step if you didn't encounter any issues with loading the </span><em><span>Menu</span></em><span> page).</span></p><p><span>The grading script can provide additional tips for parts of the lab that you didn't complete successfully. You can submit your work as many times as you like—only the score that you achieve on the last submission will be retained.</span></p><p><span>Also, if you want to connect to the new EC2 instance in Oregon (us-west-2) to do some troubleshooting, run this command from the AWS Cloud9 IDE in us-east-1:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">ssh</span> <span class="cm-attribute">-i</span> ~/.ssh/id_rsa ec2-user@&lt;public-ip-of-ProdCafeServer&gt;</span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre><p><span>Note that &lt;</span><em><span>public-ip-of-ProdCafeServer</span></em><span>&gt; is the actual public IP address of the ProdCafeServer instance.</span></p></li></ol><p>&nbsp;</p><h2 id="update-from-the-café"><span>Update from the café</span></h2><p><img src="./Challenge Lab Creating a Dynamic Website for the Café_files/cafe-team.png" referrerpolicy="no-referrer" alt="cafe team"></p><p><span>Sofía is now a hero at the cafe! She created a dynamic website, </span><em><span>and</span></em><span> she also created a duplicate version of the same website that runs in a second AWS Region.</span></p><p><span>Sofía decided to designate the first EC2 instance that she created—the one in the us-east-1 Region—as the </span><em><span>development</span></em><span> instance. The second instance she created—the one in Oregon (the us-west-2 Region)—will be the </span><em><span>production</span></em><span> instance.</span></p><p><span>This way, Sofía and any other application developers can test application enhancements on the </span><em><span>development</span></em><span> site without affecting the </span><em><span>production</span></em><span> site. Then, when the developers decide that the enhancements look good and they have fully tested them, they can migrate the code to the production site.</span></p><p><span>Sofía explained to her parents, Frank and Martha, what she had done. Though they didn't fully understand all the technical terms that Sofía used, they were pleased to know that the website can now take online orders. They were also glad to hear that they can now test new enhancements to the website without immediately exposing those changes to customers.</span></p><p>&nbsp;</p><h2 id="submitting-your-work"><span>Submitting your work</span></h2><ol start="46"><li><p><span>At the top of these instructions, </span><span id="ssb_blue"><span>Submit</span></span><span> to record your progress and when prompted, choose </span><strong><span>Yes</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><ol start="47"><li><p><span>If the results don't display after a couple of minutes, return to the top of these instructions and choose </span><span id="ssb_voc_grey"><span>Grades</span></span></p><p><span> </span><strong><span>Tip</span></strong><span>: You can submit your work multiple times. After you change your work, choose </span><strong><span>Submit</span></strong><span> again. Your last submission is what will be recorded for this lab.</span></p></li></ol><p>&nbsp;</p><ol start="48"><li><p><span>To find detailed feedback on your work, choose </span><span id="ssb_voc_grey"><span>Details</span></span><span> followed by </span><i class="fas fa-caret-right"></i><span> </span><strong><span>View Submission Report</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><h2 id="lab-complete"><span>Lab complete</span></h2><p><i class="icon-flag-checkered"></i><span> Congratulations! You have completed the lab.</span></p><ol start="49"><li><p><span>To confirm that you want to end the lab, at the top of this page, choose </span><strong><span id="ssb_voc_grey"><span>End Lab</span></span></strong><span>, and then choose </span><strong><span id="ssb_blue"><span>Yes</span></span></strong><span>.  </span></p><p><span>A panel should appear with this message: </span><em><span>DELETE has been initiated... You may close this message box now.</span></em></p></li></ol><p>&nbsp;</p><ol start="50"><li><p><span>To close the panel, choose the </span><strong><span>X</span></strong><span> in the top-right corner.</span></p></li></ol><p>&nbsp;</p><p><em><span>©2020 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.</span></em></p></div></div>
<script defer="" src="./Challenge Lab Creating a Dynamic Website for the Café_files/vcd15cbe7772f49c399c6a5babf22c1241717689176015" integrity="sha512-ZpsOmlRQV6y907TI0dKBHq9Md29nnaEIPlkf84rnaERnq6zvWvPUqr2ft8M1aS28oN72PdrCzSjY4U6VaAw1EQ==" data-cf-beacon="{&quot;rayId&quot;:&quot;8ba7aefa1f6c0304&quot;,&quot;serverTiming&quot;:{&quot;name&quot;:{&quot;cfL4&quot;:true}},&quot;version&quot;:&quot;2024.8.0&quot;,&quot;token&quot;:&quot;a73834a4a1444e9ab89e8da06da41720&quot;}" crossorigin="anonymous"></script>

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