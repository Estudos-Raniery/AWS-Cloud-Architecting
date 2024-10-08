<!DOCTYPE html>
<!-- saved from url=(0089)https://labs.vocareum.com/web/1964919/3231445.0/ASNLIB/public/docs/lang/en_us/README.html -->
<html foxified=""><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta name="viewport" content="width=device-width initial-scale=1">

<link href="./Challenge Lab Migrating a Database to Amazon RDS_files/css" rel="stylesheet" type="text/css"><style type="text/css">html {overflow-x: initial !important;}:root { --bg-color: #ffffff; --text-color: #333333; --select-text-bg-color: #B5D6FC; --select-text-font-color: auto; --monospace: "Lucida Console",Consolas,"Courier",monospace; --title-bar-height: 20px; }
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
<script type="text/javascript" src="./Challenge Lab Migrating a Database to Amazon RDS_files/c7fa7451-6f95-4815-ac32-b8cc2537837a" data-awssuidacr="53831616-c450-4d58-b234-a61f3b697d56"></script></head>
<body class="typora-export vsc-initialized"><div class="typora-export-content">
<div id="write" class=""><h1 id="module-5----challenge-lab-migrating-a-database-to-amazon-rds"><span>Module 5 – Challenge Lab: Migrating a Database to Amazon RDS</span></h1><!--Lab borrows from ACOv1 activity 6, but is significantly modified and extended--><h2 id="scenario"><span>Scenario</span></h2><p><span>The café currently uses a single EC2 instance to host their web server, database, and application code.</span></p><p><span>Meanwhile, café business has grown. The order history that's stored in the database provides valuable business information that the café staff doesn't want to lose. Martha uses the data for accounting, and Frank looks at it occasionally to plan how many of each dessert type he should bake.</span></p><p><span>Sofía has additional concerns. The database must be consistently upgraded and patched, and she doesn’t always have time to do these tasks. Also, administering the database is a specialized skill. Training others to do database administration isn’t something that she wants to spend time on. Meanwhile, Sofía is also concerned that the café isn’t doing data backups as often as they should.</span></p><p><span>Finally, Martha also wants to reduce labor costs that are associated with the technical learning investment that's needed to manage the database.</span></p><p>&nbsp;</p><h2 id="lab-overview-and-objectives"><span>Lab overview and objectives</span></h2><p><span>In this lab, you will migrate data from a database on an Amazon Elastic Compute Cloud (Amazon EC2) instance to Amazon Relational Database Service (Amazon RDS). Specifically, you will migrate a MariaDB database that runs on an EC2 instance to a MariaDB database that runs on Amazon RDS. You will also update the café web application to use the new database to store data for all future orders.</span></p><p><span>After completing this lab, you should be able to:</span></p><ul><li><p><span>Create an RDS database instance</span></p></li><li><p><span>Export data from MariaDB database by using mysqldump</span></p></li><li><p><span>Connect a SQL client to an RDS database.</span></p></li><li><p><span>Migrate data from a MariaDB database that runs on an EC2 instance to an RDS database instance</span></p></li><li><p><span>Configure a web application to use the new RDS database instance for data storage</span></p></li></ul><p>&nbsp;</p><p><span>When you </span><em><span>start</span></em><span> the lab, the following resources are already created for you in the AWS account:</span></p><p><img src="./Challenge Lab Migrating a Database to Amazon RDS_files/m5ch-lab-start-arch.png" referrerpolicy="no-referrer" alt="start architecture"></p><p><span>At the </span><em><span>end</span></em><span> of this lab, your architecture will look like the following example:</span></p><p><img src="./Challenge Lab Migrating a Database to Amazon RDS_files/m5ch-lab-end-arch.png" referrerpolicy="no-referrer" alt="final architecture"></p><p>&nbsp;</p><h2 id="duration"><span>Duration</span></h2><p><span>This lab will require approximately </span><strong><span>80 minutes</span></strong><span> to complete.</span></p><p>&nbsp;</p><h2 id="aws-service-restrictions"><span>AWS service restrictions</span></h2><p><span>In this lab environment, access to AWS services and service actions might be restricted to the ones that are needed to complete the lab instructions. You might encounter errors if you attempt to access other services or perform actions beyond the ones that are described in this lab.</span></p><p>&nbsp;</p><h2 id="accessing-the-aws-management-console"><span>Accessing the AWS Management Console</span></h2><ol start=""><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> to launch your lab.</span></p><p><span>A </span><strong><span>Start Lab</span></strong><span> panel opens, and it displays the lab status.</span></p><p><i class="fas fa-info-circle"></i><span> </span><strong><span>Tip</span></strong><span>: If you need more time to complete the lab, restart the timer for the environment by choosing the </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> button again.</span></p></li><li><p><span>Wait until the </span><strong><span>Start Lab</span></strong><span> panel displays the message </span><em><span>Lab status: ready</span></em><span>, then close the panel by choosing the </span><strong><span>X</span></strong><span>.</span></p></li><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>AWS</span></span><span>.</span></p><p><span>This action opens the AWS Management Console in a new browser tab. The system automatically logs you in.</span></p><p><i class="fas fa-exclamation-triangle"></i><span> </span><strong><span>Tip</span></strong><span>: If a new browser tab does not open, a banner or icon is usually at the top of your browser with the message that your browser is preventing the site from opening pop-up windows. Choose the banner or icon, and then choose </span><strong><span>Allow pop-ups</span></strong><span>.</span></p></li><li><p><span>Arrange the </span><strong><span>AWS Management Console</span></strong><span> tab so that it displays alongside these instructions. Ideally, you will have both browser tabs open at the same time so that you can follow the lab steps more easily.</span></p><p><i class="fas fa-exclamation-triangle"></i><span> </span><strong><span>Do not change the Region unless specifically instructed to do so</span></strong><span>.</span></p><p><span> </span><strong><span>Tip</span></strong><span>: To hide the terminal, you can clear the </span><strong><span>Terminal</span></strong><span> check box at the top of the screen.</span></p></li></ol><p>&nbsp;</p><h2 id="a-business-request-creating-an-rds-instance-for-the-café-application-challenge-1"><span>A business request: Creating an RDS instance for the café application (Challenge #1)</span></h2><p><span>After a conversation with Olivia—the AWS solutions architect who often comes in for a coffee—Sofía decided that the café needs a database solution that is easier to maintain. In addition, the database should provide essential features such as durability, scalability, and high performance.</span></p><p><img src="./Challenge Lab Migrating a Database to Amazon RDS_files/olivia.png" alt="Olivia" width="300" class="centered_image"></p><p><span>In the first part of this lab, you will take on the role of Sofía. You will create an RDS instance that the café can use as the data storage layer for the café website. You will also connect to the EC2 instance and analyze the details of the cafe web application.</span></p><p>&nbsp;</p><h3 id="task-1-creating-an-rds-instance"><span>Task 1: Creating an RDS instance</span></h3><p><span>Your first challenge in this lab is to create an RDS instance.</span></p><ol start="5"><li><p><span>Create an RDS instance that complies with these specifications. (When you submit your work at the end of this lab, it will check for many of these settings. To get full credit, follow these guidelines.)</span></p><ul><li><p><strong><span>Engine type</span></strong><span>: </span><em><span>MariaDB</span></em></p></li><li><p><strong><span>Templates</span></strong><span>: </span><em><span>Dev/Test</span></em></p></li><li><p><strong><span>DB instance identifier</span></strong><span>: </span><code>CafeDatabase</code></p></li><li><p><strong><span>Username</span></strong><span>: </span><code>admin</code></p></li><li><p><strong><span>Password</span></strong><span>: </span><code>Caf3DbPassw0rd!</code></p><ul><li><p><i class="fas fa-exclamation-triangle"></i><span>You must use this precise password.</span></p></li><li><p><strong><span>Tip</span></strong><span>: Copy and paste the password to set it.</span></p></li></ul></li><li><p><strong><span>DB Instance Class</span></strong><span>: </span><em><span>db.t3.micro</span></em></p></li><li><p><strong><span>Storage type</span></strong><span>: </span><em><span>General Purpose (SSD)</span></em></p></li><li><p><strong><span>Allocated storage</span></strong><span>: </span><code>20</code><span> GiB</span></p></li><li><p><span>Do </span><em><span>not</span></em><span> create a standby instance</span></p></li><li><p><span>Place it in the </span><strong><span>Lab VPC</span></strong></p></li><li><p><strong><span>Subnet Group</span></strong><span>: </span><code>lab-db-subnet-group</code><span>, where the database is </span><em><span>not</span></em><span> publicly accessible.</span></p></li><li><p><span>Choose existing </span><strong><span>VPC security group</span></strong><span> named </span><code>dbSG</code><span>, and </span><em><span>unselect</span></em><span> the </span><code>default</code><span> security group.</span></p></li><li><p><strong><span>Availability Zone</span></strong><span>: Choose the first Availability Zone in the list, which ends in </span><code>a</code><span>. For example, if the Region is </span><em><span>us-east-1</span></em><span>, choose </span><strong><span>us-east-1a</span></strong><span>.</span></p></li><li><p><strong><span>Database port</span></strong><span>: Keep the default TCP port of </span><em><span>3306</span></em><span>.</span></p></li><li><p><span>Enhanced monitoring is </span><em><span>not</span></em><span> supported in the lab environment. Clear the default setting.</span></p></li></ul></li></ol><p><span> </span><img src="./Challenge Lab Migrating a Database to Amazon RDS_files/db-creating.png" referrerpolicy="no-referrer" alt="DB creating"></p><p>&nbsp;</p><p><strong><span>Important</span></strong><span>: Don't wait for the database to finish the creation process. Instead, after you have successfully started the database creation process, continue to the next step.</span></p><p>&nbsp;</p><h3 id="task-2-analyzing-the-existing-café-application-deployment"><span>Task 2: Analyzing the existing café application deployment</span></h3><p><span>In this task, you will connect to the existing EC2 instance that runs the current café application.</span></p><ol start="6"><li><p><span>Browse to the EC2 Console and choose </span><strong><span>Running instances</span></strong><span>.</span></p><p><span>Notice the running instance named </span><strong><span>CafeServer</span></strong><span>. This EC2 instance was created when you started the lab.  </span></p></li><li><p><span>Test the café application.</span></p><ul><li><p><span>Open a new browser tab and load the café application at </span><code>http://&lt;public-ip-address&gt;/cafe</code><span>.</span></p><p><strong><span>Note</span></strong><span>: Replace &lt;</span><em><span>public-ip-address</span></em><span>&gt; with the actual IPv4 public IP address of the </span><em><span>CafeServer</span></em><span> instance.</span></p></li><li><p><span>Browse to the </span><strong><span>Menu</span></strong><span> page and test placing an order.</span></p><p><span>To do this, change the quantity for at least one menu item to at least </span><em><span>1</span></em><span> and choose </span><strong><span>Submit Order</span></strong><span>.</span></p><p><span>An </span><strong><span>Order Confirmation</span></strong><span> page should display, which indicates that the café website is working as intended.</span></p></li><li><p><span>Choose </span><strong><span>Order History</span></strong><span>.</span></p><p><span>The page shows that many orders were placed. The current database contains past customer orders that you will migrate to a database that's hosted on Amazon RDS.</span></p></li></ul></li></ol><ol start="8"><li><p><span>Connect to the EC2 instance by using AWS Systems Manager to access a terminal session in the browser.</span></p><ul><li><p><span>Back in the AWS Management Console, navigate to the </span><strong><span>Systems Manager</span></strong><span> Console and choose </span><strong><span>Session Manager</span></strong><span>.</span></p></li><li><p><span>Start a session and connect to the </span><strong><span>CafeServer</span></strong><span>.</span></p><p><span>You should now have a new browser tab open, with a terminal session that's connected to the EC2 instance.</span></p></li><li><p><span>At the prompt, enter the following commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation" style=""><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">bash</span></span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">su</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">su</span> ec2-user</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">whoami</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">cd</span> /home/ec2-user/</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 115px;"></div><div class="CodeMirror-gutters" style="display: none; height: 115px;"></div></div></div></pre><p><strong><span>Analysis</span></strong><span>: The first command gave you a Bash shell. The second command switched your session to use the root user account on the EC2 instance. The third command switched you to use the </span><em><span>ec2-user</span></em><span> account. The fourth command should have returned output that confirms that you are connected as the ec2-user. The last command switches your terminal to the home directory of the ec2-user.</span></p></li></ul></li></ol><p><img src="./Challenge Lab Migrating a Database to Amazon RDS_files/sess-mgr.png" alt="session manager screenshot" width="400"></p><p><strong><span>Note</span></strong><span>: The Systems Manager agent (</span><em><span>ssm agent</span></em><span>) is installed by default on all Amazon Linux 2 instances (and some other OS types). When you started the lab and the EC2 instance was created, the user data specified that the ssm agent service should be started on the instance. Also, an AWS Identity and Access Management (IAM) role that includes an IAM policy named </span><em><span>AmazonSSMManagedInstanceCore</span></em><span> was attached to the EC2 instance. These two actions made the instance accessible through the Systems Manager session manager.</span></p><p>&nbsp;</p><h2 id="new-business-requirement-exporting-data-from-the-old-database-and-establishing-a-connection-to-the-new-database-challenge-2"><span>New business requirement: Exporting data from the old database and establishing a connection to the new database (Challenge #2)</span></h2><p><span>Now that you created a new RDS instance, you can move on to the next step in the café's database migration plan. Next, you will export the data from the database that the café application currently uses. You will also establish a network connection from the EC2 instance (where the application runs) to the new RDS database instance.</span></p><p><span>In this challenge, you continue as Sofía to complete these tasks.</span></p><h3 id="task-3-working-with-the-database-on-the-ec2-instance"><span>Task 3: Working with the database on the EC2 instance</span></h3><p><span>In this task, you will observe details about the MariaDB database that runs on the EC2 instance. You will then export existing order history data from the database by using the </span><em><span>mysqldump</span></em><span> utility.</span></p><ol start="9"><li><p><span>Observe details of the database that runs on the EC2 instance.</span></p><p><span>In the terminal, run these commands:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">service</span> mariadb status</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">mysql <span class="cm-attribute">--version</span></span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 46px;"></div><div class="CodeMirror-gutters" style="display: none; height: 46px;"></div></div></div></pre><p><span>The output should show that the locally installed MariaDB database on this EC2 instance is running. It should also show the version number of the database.</span></p><p><span>Leave this browser tab open. You will use it throughout this lab.</span></p></li></ol><ol start="10"><li><p><span>Return to the browser tab with the </span><strong><span>AWS Systems Manager</span></strong><span> console open in it.</span></p></li></ol><ol start="11"><li><p><span>From the panel on the left, under </span><strong><span>Application Management</span></strong><span>, choose </span><strong><span>Parameter Store</span></strong><span>.</span></p><p><span>Notice that seven parameters are stored here. The café application PHP code references these values—for example, to retrieve the connection information for the database.</span></p><ul><li><p><span>Choose the </span><code>/cafe/dbPassword</code><span> parameter, and copy the </span><strong><span>Value</span></strong><span> to your clipboard. You will use this value in a moment.</span></p></li></ul></li></ol><ol start="12"><li><p><span>Connect to the database that is running on the EC2 instance.</span></p><p><span>In the browser tab with the Bash terminal, connect the terminal-based MySQL client to the database by running this command:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">mysql <span class="cm-attribute">-u</span> root <span class="cm-attribute">-p</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre><p><span>When prompted for the database password, paste the </span><em><span>dbPassword</span></em><span> parameter value that you copied a moment ago.</span></p><p><span>You should now see a  </span><code>mariadb&gt;</code><span> prompt. This prompt indicates that you are now connected to the MariaDB database that runs on this EC2 instance.</span></p></li></ol><p><img src="./Challenge Lab Migrating a Database to Amazon RDS_files/db-client.png" referrerpolicy="no-referrer" alt="database-client"></p><ol start="13"><li><p><span>Observe the data in the existing database.</span></p><p><span>To observe the contents of the database, enter the following commands. In particular, you will review the tables that support the café web application.</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="sql"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="sql"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">show</span> <span class="cm-keyword">databases</span><span class="cm-punctuation">;</span></span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">use</span> cafe_db<span class="cm-punctuation">;</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">show</span> <span class="cm-keyword">tables</span><span class="cm-punctuation">;</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">select</span> <span class="cm-operator">*</span> <span class="cm-keyword">from</span> <span class="cm-variable-2">`order`</span><span class="cm-punctuation">;</span></span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 92px;"></div><div class="CodeMirror-gutters" style="display: none; height: 92px;"></div></div></div></pre><p><span>These commands show all the orders that were placed, including the order that you placed a moment ago.</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="sql"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="sql"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">select</span> <span class="cm-operator">*</span> <span class="cm-keyword">from</span> <span class="cm-variable-2">`order_item`</span><span class="cm-punctuation">;</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre><p><span>This command shows the order line items. Each order number has a row for each type of item that was ordered, with details about the quantity of each item and the price.</span></p><p><span>All this data must be migrated to the new database.</span></p></li><li><p><span>Exit the SQL client.</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="sql"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="sql"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">exit</span><span class="cm-punctuation">;</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li></ol><ol start="15"><li><p><span>Capture existing data in a file by using the </span><em><span>mysqldump</span></em><span> utility.</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">mysqldump <span class="cm-attribute">--databases</span> cafe_db <span class="cm-attribute">-u</span> root <span class="cm-attribute">-p</span> &gt; CafeDbDump.sql</span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre><p><span>When prompted for the database password, paste the </span><em><span>dbPassword</span></em><span> value from the Systems Manager Parameter Store.</span></p></li></ol><ol start="16"><li><p><span>Confirm that </span><em><span>mysqldump</span></em><span> succeeded.</span></p><ul><li><p><span>Run the </span><code>ls</code><span> command in the terminal. The output should show that the </span><code>CafeDbDump.sql</code><span> file was created.</span></p></li><li><p><span>Run the </span><code>cat CafeDbDump.sql</code><span> command to see the contents of the file.</span></p><p><span>In the next section of the lab, you will import this data to the new RDS database.</span></p></li></ul></li></ol><p>&nbsp;</p><h3 id="task-4-working-with-the-rds-database"><span>Task 4: Working with the RDS database</span></h3><p><span>In this task, you will first answer a few questions about the RDS instance that you created. Then, you will confirm that you can connect to the RDS instance.</span></p><ol start="17"><li><p><span>In the AWS Management Console, return to the </span><strong><span>RDS</span></strong><span> service console and confirm that the </span><em><span>cafedatabase</span></em><span> RDS instance you created is now available.</span></p></li></ol><p>&nbsp;</p><h4 id="answering-questions-about-the-rds-instance"><span>Answering questions about the RDS instance</span></h4><p><span>Your answers will be recorded when you click the blue </span><strong><span>Submit</span></strong><span> button at the end of the lab.</span></p><ol start="18"><li><p><span>Access the questions in this lab.</span></p><ul><li><p><span>Above these instructions, choose </span><strong><span>Details &gt; Show</span></strong><span>.</span></p></li><li><p><span>Choose the </span><strong><span>Access the multiple choice questions</span></strong><span> link.</span></p></li></ul></li><li><p><span>In the page you loaded, answer the first four questions:</span></p><ul><li><p><span>Question 1: Where is the RDS instance running?</span></p></li><li><p><span>Question 2: Does the RDS instance have an IPv4 public IP address assigned to it?</span></p></li><li><p><span>Question 3: What is the </span><strong><span>Name</span></strong><span> tag applied to the subnet in which the RDS instance is running?</span></p></li><li><p><span>Question 4: How many security group rules are defined for the RDS instance?</span></p></li></ul></li></ol><p>&nbsp;</p><ol start="20"><li><p><span>Establish a network connection from the terminal running on the EC2 instance to the new RDS instance.</span></p></li></ol><p><span>Here are some tips to help you get started:</span></p><details>
  <summary>
  <b>Tip #1</b> (click to expand)
  </summary>
	Here is the syntax that you can use to connect:
	<code> mysql -u admin -p --host &lt;rds-endpoint&gt;</code>
<br>Replace &lt;rds-endpoint&gt; with the actual RDS endpoint for your RDS instance.<br>After you run the command, it will prompt you to enter the password for the RDS instance. You defined this password when you created the RDS instance.
</details><br><details>
  <summary>
  <b>Tip #2</b> (click to expand)
  </summary>
	Even if you enter the RDS endpoint and database password correctly, you still won't be able to connect. You must update the inbound rules of the security group that the RDS instance runs in. The MySQL client software tries to connect to the database on TCP port 3306.
</details><br><details>
  <summary>
  <b>Tip #3</b> (click to expand)
  </summary>
  Avoid opening port 3306 to <i>all</i> source IP addresses. That would not be secure. Instead, open it only to servers in the security group that is used by the EC2 instance that you're connecting from (try typing <code>sg-</code> into the source field to see options).
</details><br><details>
  <summary>
  <b>Tip #4</b> (click to expand)
  </summary>   
  You can confirm that the security group settings allow traffic on TCP port 3306 from the EC2 instance to the database. Try running these commands in the Systems Manager session manager terminal (replace <rds-endpoint> with the actual RDS endpoint):<br><code>nmap -Pn &lt;rds-endpoint&gt;</code><br>If the output of the command shows that port 3306 is open for the *mysql* service, then it confirms that the security group settings allow the traffic. <br>If <i>nmap</i> shows that the port is <i>open</i>, then the  <code>mysql -u admin -p --host &lt;rds-endpoint&gt;</code> command should also work. (However, you must enter the database password correctly. This password is the one that you set when you created the instance).
</rds-endpoint></details>  <br><p><strong><span>Note</span></strong><span>: If you still can't solve the issue, you might find it helpful to submit your work, as documented in the </span><strong><span>Submitting your work</span></strong><span> section at the end of these lab instructions. The </span><strong><span>submission report</span></strong><span> that is generated can provide additional tips for parts of the lab that you didn't complete successfully. You can submit your work as many times as you like. Only the score you achieve on the last submission is retained.</span></p><p><span>It's important to confirm that you can connect to the RDS MariaDB before you go to the next step. If you already managed to connect, congratulations!</span></p><ol start="21"><li><p><span>Run the </span><code>show databases;</code><span> command. It should show this output:</span></p><p><img src="./Challenge Lab Migrating a Database to Amazon RDS_files/rds-client.png" referrerpolicy="no-referrer" alt="rds-client"></p><ul><li><p><span>Notice that </span><em><span>cafe_db</span></em><span> database is not in the list yet. This situation is expected, because you haven't imported any data.  </span></p></li><li><p><span>To disconnect, run the </span><code>exit;</code><span> command.</span></p></li></ul></li></ol><p>&nbsp;</p><h2 id="new-business-requirement-importing-data-and-connecting-the-application-to-the-new-database-challenge-3"><span>New business requirement: Importing data and connecting the application to the new database (Challenge #3)</span></h2><p><span>In the previous challenge, you exported the data from the database that the café application currently uses. you also established a network connection from the EC2 instance to the RDS instance. You can now work on the next business requirement.</span></p><p><span>In this challenge, you will continue to take on the role of Sofía to import the cafe data into the RDS database instance. After you complete the import, you will configure the application to use the new database.</span></p><p>&nbsp;</p><h3 id="task-5-importing-the-data-into-the-rds-database-instance"><span>Task 5: Importing the data into the RDS database instance</span></h3><ol start="22"><li><p><span>Import the data that you exported in task 3 to the RDS database instance.</span></p><ul><li><p><span>To import the data, in the terminal, run the following command (where </span><code>&lt;rds-endpoint&gt;</code><span> is the actual endpoint):</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">mysql <span class="cm-attribute">-u</span> admin <span class="cm-attribute">-p</span> <span class="cm-attribute">--host</span> &lt;rds-endpoint&gt; &lt; CafeDbDump.sql</span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li><li><p><span>At the password prompt, enter the password for the RDS instance.</span></p><p><span>If you don't see any errors, the command likely succeeded.</span></p></li></ul></li></ol><ol start="23"><li><p><span>Confirm that the data was imported.</span></p><ul><li><p><span>To connect to the RDS database, run this command:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang=""><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang=""><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;">mysql -u admin -p --host &lt;rds-endpoint&gt;</span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li><li><p><span>At the password prompt, enter the password for the RDS instance.</span></p></li><li><p><span>To confirm that the data was imported, run the following command:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="sql"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="sql"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">show</span> <span class="cm-keyword">databases</span><span class="cm-punctuation">;</span></span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">use</span> cafe_db<span class="cm-punctuation">;</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">show</span> <span class="cm-keyword">tables</span><span class="cm-punctuation">;</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">select</span> <span class="cm-operator">*</span> <span class="cm-keyword">from</span> <span class="cm-variable-2">`order`</span><span class="cm-punctuation">;</span></span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 92px;"></div><div class="CodeMirror-gutters" style="display: none; height: 92px;"></div></div></div></pre></li></ul><p><span>The output of the </span><em><span>select</span></em><span> statement should show at least 24 orders in the database.</span></p><ul><li><p><span>Exit the SQL client:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="sql"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="sql"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-keyword">exit</span><span class="cm-punctuation">;</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li></ul></li></ol><p>&nbsp;</p><h3 id="task-6-connecting-the-café-application-to-the-new-database"><span>Task 6: Connecting the café application to the new database</span></h3><p><span>In this last task in the lab, you will be challenged to connect the café application to the new database. You will also stop the database that runs locally on the EC2 instance.</span></p><ol start="24"><li><p><span>Return to the </span><strong><span>AWS Systems Manager</span></strong><span> console browser tab.</span></p></li></ol><ol start="25"><li><p><span>From the panel on the left, choose </span><strong><span>Parameter Store</span></strong><span>.</span></p><p><span>Recall from an earlier challenge lab that the café application's PHP code references these values. For example, it uses the values to retrieve the connection information for the database.</span></p></li></ol><ol start="26"><li><p><span>Connect the café application to the RDS instance.</span></p><p><span>Because the database connection information has changed, you must update these values to connect the application to the new RDS database instance instead of to the database running on the EC2 instance.</span></p></li></ol><details>
  <summary>
  <b>Tip #1</b> (click to expand)
  </summary>
After you update which database the application is connected to, use the <code>http://&lt;public-ip&gt;/cafe/menu.php</code> page to test whether you have successfully updated the connection.
</details><br><details>
  <summary>
  <b>Tip #2</b> (click to expand)
  </summary>
The PHP code doesn't need any updates. Also, the network configuration doesn't need additional changes, assuming that you successfully completed the previous challenge in this lab. The only updates that you must make will be to some values in the Systems Manager Parameter Store.
</details><br><details>
  <summary>
  <b>Tip #3</b> (click to expand)
  </summary>
The <i>currency</i>, <i>dbName</i>, <i>timeZone</i>, and <i>showServerInfo</i> values don't need to be updated.
</details><br><details>
  <summary>
  <b>Tip #4</b> (click to expand)
  </summary>
The <i>dbUrl</i> should be the RDS endpoint value.
</details><br><ol start="27"><li><p><span>Confirm that your web application now uses the new database.</span></p><ul><li><p><span>Stop the database that's still running on the EC2 instance. In the terminal, use this command:</span></p><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="bash"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="bash"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9.5px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: currentcolor;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: currentcolor;"><div class="CodeMirror-measure"><pre><span>xxxxxxxxxx</span></pre></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation"><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-builtin">sudo</span> <span class="cm-builtin">service</span> mariadb <span class="cm-builtin">stop</span></span></pre></div></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 23px;"></div><div class="CodeMirror-gutters" style="display: none; height: 23px;"></div></div></div></pre></li><li><p><span>Load the </span><code>http://&lt;public-ip&gt;/cafe/menu.php</code><span> page and confirm that the application still works by placing an order.</span></p></li><li><p><span>Choose </span><strong><span>Order History</span></strong><span>. Your latest order—and all the other previous orders—should be there. These orders are the data that you migrated to the new database.</span></p></li></ul></li></ol><p>&nbsp;</p><h2 id="update-from-the-café"><span>Update from the café</span></h2><p><img src="./Challenge Lab Migrating a Database to Amazon RDS_files/cafe-team.png" alt="cafe team" width="500" class="centered_image"></p><p><span>Everyone at the café is happy with the results of the database migration. Sofía and Nikhil now have more free time on weekends, which means that Frank and Martha are saving money on labor costs.</span></p><p><span>Sofía takes a minute to relax with her friends. However, she's already thinking about improvements. A good next step would be to reduce the size of the EBS volume that the EC2 instance uses. They could also save on expenses by changing the EC2 instance type to a smaller size. Because the database no longer runs on the EC2 instance, the instance now has extra hard drive space—and it might also not need as many CPU and memory resources.</span></p><p>&nbsp;</p><h2 id="submitting-your-work"><span>Submitting your work</span></h2><ol start="28"><li><p><span>At the top of these instructions, choose </span><span id="ssb_blue"><span>Submit</span></span><span> to record your progress and when prompted, choose </span><strong><span>Yes</span></strong><span>.</span></p></li><li><p><span>If the results don't display after a couple of minutes, return to the top of these instructions and choose </span><span id="ssb_voc_grey"><span>Grades</span></span></p><p><span> </span><strong><span>Tip</span></strong><span>: You can submit your work multiple times. After you change your work, choose </span><strong><span>Submit</span></strong><span> again. Your last submission is what will be recorded for this lab.</span></p></li><li><p><span>To find detailed feedback on your work, choose </span><span id="ssb_voc_grey"><span>Details</span></span><span> followed by </span><i class="fas fa-caret-right"></i><span> </span><strong><span>View Submission Report</span></strong><span>.</span></p></li></ol><p>&nbsp;</p><h2 id="lab-complete"><span>Lab complete</span></h2><p><i class="icon-flag-checkered"></i><span> Congratulations! You have completed the lab.</span></p><ol start="31"><li><p><span>To confirm that you want to end the lab, at the top of this page, choose </span><strong><span id="ssb_voc_grey"><span>End Lab</span></span></strong><span>, and then choose </span><strong><span id="ssb_blue"><span>Yes</span></span></strong><span>.  </span></p><p><span>A panel should appear with this message: </span><em><span>DELETE has been initiated... You may close this message box now.</span></em></p></li></ol><ol start="32"><li><p><span>To close the panel, choose the </span><strong><span>X</span></strong><span> in the top-right corner.</span></p></li></ol><p>&nbsp;</p><p><em><span>©2020 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.</span></em></p></div></div>
<script defer="" src="./Challenge Lab Migrating a Database to Amazon RDS_files/vcd15cbe7772f49c399c6a5babf22c1241717689176015" integrity="sha512-ZpsOmlRQV6y907TI0dKBHq9Md29nnaEIPlkf84rnaERnq6zvWvPUqr2ft8M1aS28oN72PdrCzSjY4U6VaAw1EQ==" data-cf-beacon="{&quot;rayId&quot;:&quot;8baea5b37fd41d0b&quot;,&quot;serverTiming&quot;:{&quot;name&quot;:{&quot;cfL4&quot;:true}},&quot;version&quot;:&quot;2024.8.0&quot;,&quot;token&quot;:&quot;a73834a4a1444e9ab89e8da06da41720&quot;}" crossorigin="anonymous"></script>

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