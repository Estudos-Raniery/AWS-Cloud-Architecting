<!DOCTYPE html>
<!-- saved from url=(0089)https://labs.vocareum.com/web/1964919/3231437.0/ASNLIB/public/docs/lang/en_us/README.html -->
<html foxified=""><head><meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
<meta name="viewport" content="width=device-width initial-scale=1">

<link href="./Challenge Lab Creating a Static Website for the Café_files/css" rel="stylesheet" type="text/css"><style type="text/css">html {overflow-x: initial !important;}:root { --bg-color: #ffffff; --text-color: #333333; --select-text-bg-color: #B5D6FC; --select-text-font-color: auto; --monospace: "Lucida Console",Consolas,"Courier",monospace; --title-bar-height: 20px; }
.mac-os-11 { --title-bar-height: 28px; }
html { font-size: 14px; background-color: var(--bg-color); color: var(--text-color); font-family: "Helvetica Neue", Helvetica, Arial, sans-serif; -webkit-font-smoothing: antialiased; }
body { margin: 0px; padding: 0px; height: auto; bottom: 0px; top: 0px; left: 0px; right: 0px; font-size: 1rem; line-height: 1.42857143; overflow-x: hidden; background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; tab-size: 4; background-position: inherit inherit; background-repeat: inherit inherit; }
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
img { max-width: 100%; vertical-align: middle; }
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
sup.md-footnote { padding: 2px 4px; background-color: rgba(238, 238, 238, 0.701961); color: rgb(85, 85, 85); border-top-left-radius: 4px; border-top-right-radius: 4px; border-bottom-right-radius: 4px; border-bottom-left-radius: 4px; cursor: pointer; }
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
.md-fences { font-size: 0.9rem; display: block; break-inside: avoid; text-align: left; overflow: visible; white-space: pre; background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; position: relative !important; background-position: inherit inherit; background-repeat: inherit inherit; }
.md-fences-adv-panel { width: 100%; margin-top: 10px; text-align: center; padding-top: 0px; padding-bottom: 8px; overflow-x: auto; }
#write .md-fences.mock-cm { white-space: pre-wrap; }
.md-fences.md-fences-with-lineno { padding-left: 0px; }
#write.fences-no-line-wrapping .md-fences.mock-cm { white-space: pre; overflow-x: auto; }
.md-fences.mock-cm.md-fences-with-lineno { padding-left: 8px; }
.CodeMirror-line, twitterwidget { break-inside: avoid; }
.footnotes { opacity: 0.8; font-size: 0.9rem; margin-top: 1em; margin-bottom: 1em; }
.footnotes + .footnotes { margin-top: 0px; }
.md-reset { margin: 0px; padding: 0px; border: 0px; outline: 0px; vertical-align: top; text-decoration: none; text-shadow: none; float: none; position: static; width: auto; height: auto; white-space: nowrap; cursor: inherit; line-height: normal; font-weight: 400; text-align: left; box-sizing: content-box; direction: ltr; background-position: 0px 0px; background-repeat: initial initial; }
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
  body, html { border: 1px solid transparent; height: 99%; break-after: avoid-page; break-before: avoid-page; font-variant-ligatures: no-common-ligatures; }
  #write { margin-top: 0px; padding-top: 0px; border-color: transparent !important; }
  .typora-export * { -webkit-print-color-adjust: exact; }
  .typora-export #write { break-after: avoid-page; }
  .typora-export #write::after { height: 0px; }
  .is-mac table { break-inside: avoid; }
  .typora-export-show-outline .typora-export-sidebar { display: none; }
}
.footnote-line { margin-top: 0.714em; font-size: 0.7em; }
a img, img a { cursor: pointer; }
pre.md-meta-block { font-size: 0.8rem; min-height: 0.8rem; white-space: pre-wrap; background-color: rgb(204, 204, 204); display: block; overflow-x: hidden; background-position: initial initial; background-repeat: initial initial; }
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
.md-toc { min-height: 3.58rem; position: relative; font-size: 0.9rem; border-top-left-radius: 10px; border-top-right-radius: 10px; border-bottom-right-radius: 10px; border-bottom-left-radius: 10px; }
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
kbd { margin: 0px 0.1em; padding: 0.1em 0.6em; font-size: 0.8em; color: rgb(36, 39, 41); background-color: rgb(255, 255, 255); border: 1px solid rgb(173, 179, 185); border-top-left-radius: 3px; border-top-right-radius: 3px; border-bottom-right-radius: 3px; border-bottom-left-radius: 3px; box-shadow: rgba(12, 13, 14, 0.2) 0px 1px 0px, rgb(255, 255, 255) 0px 0px 0px 2px inset; white-space: nowrap; vertical-align: middle; background-position: initial initial; background-repeat: initial initial; }
.md-comment { color: rgb(162, 127, 3); opacity: 0.8; font-family: var(--monospace); }
code { text-align: left; }
a.md-print-anchor { white-space: pre !important; border: none !important; display: inline-block !important; position: absolute !important; width: 1px !important; right: 0px !important; outline: 0px !important; text-shadow: initial !important; background-position: 0px 0px !important; background-repeat: initial initial !important; }
.os-windows.monocolor-emoji .md-emoji { font-family: "Segoe UI Symbol", sans-serif; }
.md-diagram-panel > svg { max-width: 100%; }
[lang="flow"] svg, [lang="mermaid"] svg { max-width: 100%; height: auto; }
[lang="mermaid"] .node text { font-size: 1rem; }
table tr th { border-bottom-width: 0px; }
video { max-width: 100%; display: block; margin: 0px auto; }
iframe { max-width: 100%; width: 100%; border: none; }
.highlight td, .highlight tr { border: 0px; }
mark { background-color: rgb(255, 255, 0); color: rgb(0, 0, 0); background-position: initial initial; background-repeat: initial initial; }
.md-html-inline .md-plain, .md-html-inline strong, mark .md-inline-math, mark strong { color: inherit; }
.md-expand mark .md-meta { opacity: 0.3 !important; }
mark .md-meta { color: rgb(0, 0, 0); }
@media print {
  .typora-export h1, .typora-export h2, .typora-export h3, .typora-export h4, .typora-export h5, .typora-export h6 { break-inside: avoid; }
}
.md-diagram-panel .messageText { stroke: none !important; }
.md-diagram-panel .start-state { fill: var(--node-fill); }
.md-diagram-panel .edgeLabel rect { opacity: 1 !important; }
.md-require-zoom-fix { height: auto; margin-top: 16px; margin-bottom: 16px; }
.md-require-zoom-fix foreignObject { font-size: var(--mermaid-font-zoom); }
.md-fences.md-fences-math { font-size: 1em; }
.md-fences-advanced:not(.md-focus) { padding: 0px; white-space: nowrap; border: 0px; }
.md-fences-advanced:not(.md-focus) { background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; background-position: inherit inherit; background-repeat: inherit inherit; }
.typora-export-show-outline .typora-export-content { max-width: 1440px; margin: auto; display: flex; flex-direction: row; }
.typora-export-sidebar { width: 300px; font-size: 0.8rem; margin-top: 80px; margin-right: 18px; }
.typora-export-show-outline #write { --webkit-flex: 2; flex: 2 1 0%; }
.typora-export-sidebar .outline-content { position: fixed; top: 0px; max-height: 100%; overflow-y: auto; padding-bottom: 30px; padding-top: 60px; width: 300px; overflow-x: hidden; }
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
.outline-expander::before { content: ''; position: relative; font-family: Ionicons; display: inline-block; font-size: 8px; vertical-align: middle; }
.outline-item { padding-top: 3px; padding-bottom: 3px; cursor: pointer; }
.outline-expander:hover::before { content: ''; }
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
.outline-item-open > .outline-item > .outline-expander::before { content: ''; }
.outline-children { display: none; }
.info-panel-tab-wrapper { display: none; }
.outline-item-open > .outline-children { display: block; }
.typora-export .outline-item { padding-top: 1px; padding-bottom: 1px; }
.typora-export .outline-item:hover { margin-right: -8px; border-right-width: 8px; border-right-style: solid; border-right-color: transparent; }
.typora-export .outline-expander::before { content: "+"; font-family: inherit; top: -1px; }
.typora-export .outline-expander:hover::before, .typora-export .outline-item-open > .outline-item > .outline-expander::before { content: '−'; }
.typora-export-collapse-outline .outline-children { display: none; }
.typora-export-collapse-outline .outline-item-open > .outline-children, .typora-export-no-collapse-outline .outline-children { display: block; }
.typora-export-no-collapse-outline .outline-expander::before { content: "" !important; }
.typora-export-show-outline .outline-item-active > .outline-item .outline-label { font-weight: 700; }
.md-inline-math-container mjx-container { zoom: 0.95; }


.CodeMirror { height: auto; }
.CodeMirror.cm-s-inner { background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; background-position: inherit inherit; background-repeat: inherit inherit; }
.CodeMirror-scroll { overflow-y: hidden; overflow-x: auto; z-index: 3; }
.CodeMirror-gutter-filler, .CodeMirror-scrollbar-filler { background-color: rgb(255, 255, 255); }
.CodeMirror-gutters { border-right-width: 1px; border-right-style: solid; border-right-color: rgb(221, 221, 221); background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; white-space: nowrap; background-position: inherit inherit; background-repeat: inherit inherit; }
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
.cm-s-inner .CodeMirror-activeline-background { background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; background-position: inherit inherit; background-repeat: inherit inherit; }
.CodeMirror { position: relative; overflow: hidden; }
.CodeMirror-scroll { height: 100%; outline: 0px; position: relative; box-sizing: content-box; background-image: inherit; background-size: inherit; background-attachment: inherit; background-origin: inherit; background-clip: inherit; background-color: inherit; background-position: inherit inherit; background-repeat: inherit inherit; }
.CodeMirror-sizer { position: relative; }
.CodeMirror-gutter-filler, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-filler, .CodeMirror-vscrollbar { position: absolute; z-index: 6; display: none; outline: 0px; }
.CodeMirror-vscrollbar { right: 0px; top: 0px; overflow: hidden; }
.CodeMirror-hscrollbar { bottom: 0px; left: 0px; overflow-y: hidden; overflow-x: auto; }
.CodeMirror-scrollbar-filler { right: 0px; bottom: 0px; }
.CodeMirror-gutter-filler { left: 0px; bottom: 0px; }
.CodeMirror-gutters { position: absolute; left: 0px; top: 0px; padding-bottom: 10px; z-index: 3; overflow-y: hidden; }
.CodeMirror-gutter { white-space: normal; height: 100%; box-sizing: content-box; padding-bottom: 30px; margin-bottom: -32px; display: inline-block; }
.CodeMirror-gutter-wrapper { position: absolute; z-index: 4; border: none !important; background-position: 0px 0px !important; background-repeat: initial initial !important; }
.CodeMirror-gutter-background { position: absolute; top: 0px; bottom: 0px; z-index: 4; }
.CodeMirror-gutter-elt { position: absolute; cursor: default; z-index: 4; }
.CodeMirror-lines { cursor: text; }
.CodeMirror pre { border-top-left-radius: 0px; border-top-right-radius: 0px; border-bottom-right-radius: 0px; border-bottom-left-radius: 0px; border-width: 0px; font-family: inherit; font-size: inherit; margin: 0px; white-space: pre; word-wrap: normal; color: inherit; z-index: 2; position: relative; overflow: visible; background-position: 0px 0px; background-repeat: initial initial; }
.CodeMirror-wrap pre { word-wrap: break-word; white-space: pre-wrap; word-break: normal; }
.CodeMirror-code pre { border-right-width: 30px; border-right-style: solid; border-right-color: transparent; width: fit-content; }
.CodeMirror-wrap .CodeMirror-code pre { border-right-style: none; width: auto; }
.CodeMirror-linebackground { position: absolute; left: 0px; right: 0px; top: 0px; bottom: 0px; z-index: 0; }
.CodeMirror-linewidget { position: relative; z-index: 2; overflow: auto; }
.CodeMirror-wrap .CodeMirror-scroll { overflow-x: hidden; }
.CodeMirror-measure { position: absolute; width: 100%; height: 0px; overflow: hidden; visibility: hidden; }
.CodeMirror-measure pre { position: static; }
.CodeMirror div.CodeMirror-cursor { position: absolute; visibility: hidden; border-right-style: none; width: 0px; }
.CodeMirror div.CodeMirror-cursor { visibility: hidden; }
.CodeMirror-focused div.CodeMirror-cursor { visibility: inherit; }
.cm-searching { background-color: rgba(255, 255, 0, 0.4); background-position: initial initial; background-repeat: initial initial; }
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
    --side-bar-bg-color : #fafafa;
    --control-text-color: #777;
}

@include-when-export url(https://fonts.loli.net/css?family=Open+Sans:400italic,700italic,700,400&subset=latin,latin-ext);

html {
    font-size: 16px;
}

body {
    font-family: "Amazon Ember", "Open Sans", "Clear Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
    color      : rgb(51, 51, 51);
    line-height: 1.6;
}

#write {
    max-width     : 860px;
    margin        : 0 auto;
    padding       : 30px;
    padding-bottom: 100px;
}

#write>ul:first-child,
#write>ol:first-child {
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
    position     : relative;
    margin-top   : 1rem;
    margin-bottom: 1rem;
    font-weight  : bold;
    line-height  : 1.4;
    cursor       : text;
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
    padding-bottom: .3em;
    font-size     : 2.25em;
    line-height   : 1.2;
    border-bottom : 1px solid #eee;
}

h2 {
    padding-bottom: .3em;
    font-size     : 1.75em;
    line-height   : 1.225;
    border-bottom : 1px solid #eee;
}

h3 {
    font-size  : 1.5em;
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
    color    : #777;
}

p,
blockquote,
ul,
ol,
dl,
table {
    margin: 0.8em 0;
}

li>ol,
li>ul {
    margin: 0 0;
}

hr {
    height          : 2px;
    padding         : 0;
    margin          : 16px 0;
    background-color: #e7e7e7;
    border          : 0 none;
    overflow        : hidden;
    box-sizing      : content-box;
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
    padding    : 0 15px;
    color      : #777777;
}

blockquote blockquote {
    padding-right: 0;
}

table {
    padding   : 0;
    word-break: initial;
}

table tr {
    border-top: 1px solid #dfe2e5;
    margin    : 0;
    padding   : 0;
}

table tr:nth-child(2n),
thead {
    background-color: #f8f8f8;
}

table tr th {
    font-weight  : bold;
    border       : 1px solid #dfe2e5;
    border-bottom: 0;
    margin       : 0;
    padding      : 6px 13px;
}

table tr td {
    border : 1px solid #dfe2e5;
    margin : 0;
    padding: 6px 13px;
}

table tr th:first-child,
table tr td:first-child {
    margin-top: 0;
}

table tr th:last-child,
table tr td:last-child {
    margin-bottom: 0;
}

.CodeMirror-lines {
    padding-left: 4px;
}

.code-tooltip {
    box-shadow: 0 1px 1px 0 rgba(0, 28, 36, .3);
    border-top: 1px solid #eef2f2;
}

.md-fences,
code,
tt {
    border          : 1px solid #e7eaed;
    background-color: #f8f8f8;
    border-radius   : 3px;
    padding         : 0;
    padding         : 2px 4px 0px 4px;
    font-size       : 0.9em;
}

code {
    background-color: #f3f4f4;
    padding         : 0 2px 0 2px;
}

.md-fences {
    margin-bottom : 15px;
    margin-top    : 15px;
    padding-top   : 8px;
    padding-bottom: 6px;
}


.md-task-list-item>input {
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
    padding         : 1rem;
    font-size       : 85%;
    line-height     : 1.45;
    background-color: #f7f7f7;
    border          : 0;
    border-radius   : 3px;
    color           : #777777;
    margin-top      : 0 !important;
}

.mathjax-block>.code-tooltip {
    bottom: .375rem;
}

.md-mathjax-midline {
    background: #fafafa;
}

#write>h3.md-focus:before {
    left: -1.5625rem;
    top : .375rem;
}

#write>h4.md-focus:before {
    left: -1.5625rem;
    top : .285714286rem;
}

#write>h5.md-focus:before {
    left: -1.5625rem;
    top : .285714286rem;
}

#write>h6.md-focus:before {
    left: -1.5625rem;
    top : .285714286rem;
}

.md-image>.md-meta {
    /*border     : 1px solid #ddd;*/
    border-radius: 3px;
    padding      : 2px 0px 0px 4px;
    font-size    : 0.9em;
    color        : inherit;
}

.md-tag {
    color  : #a7a7a7;
    opacity: 1;
}

.md-toc {
    margin-top    : 20px;
    padding-bottom: 20px;
}

.sidebar-tabs {
    border-bottom: none;
}

#typora-quick-open {
    border          : 1px solid #ddd;
    background-color: #f8f8f8;
}

#typora-quick-open-item {
    background-color: #FAFAFA;
    border-color    : #FEFEFE #e5e5e5 #e5e5e5 #eee;
    border-style    : solid;
    border-width    : 1px;
}

/** focus mode */
.on-focus-mode blockquote {
    border-left-color: rgba(85, 85, 85, 0.12);
}

header,
.context-menu,
.megamenu-content,
footer {
    font-family: "Segoe UI", "Arial", sans-serif;
}

.file-node-content:hover .file-node-icon,
.file-node-content:hover .file-node-open-state {
    visibility: visible;
}

.mac-seamless-mode #typora-sidebar {
    background-color: #fafafa;
    background-color: var(--side-bar-bg-color);
}

.md-lang {
    color: #b4654d;
}

.html-for-mac .context-menu {
    --item-hover-bg-color: #E6F0FE;
}

#md-notification .btn {
    border: 0;
}

.dropdown-menu .divider {
    border-color: #e5e5e5;
}

.ty-preferences .window-content {
    background-color: #fafafa;
}

.ty-preferences .nav-group-item.active {
    color     : white;
    background: #999;
}


mjx-container[jax="SVG"] {
  direction: ltr;
}

mjx-container[jax="SVG"] > svg {
  overflow: visible;
  min-height: 1px;
  min-width: 1px;
}

mjx-container[jax="SVG"] > svg a {
  fill: blue;
  stroke: blue;
}

mjx-assistive-mml {
  position: absolute !important;
  top: 0px;
  left: 0px;
  clip: rect(1px, 1px, 1px, 1px);
  padding: 1px 0px 0px 0px !important;
  border: 0px !important;
  display: block !important;
  width: auto !important;
  overflow: hidden !important;
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

mjx-assistive-mml[display="block"] {
  width: 100% !important;
}

mjx-container[jax="SVG"][display="true"] {
  display: block;
  text-align: center;
  margin: 1em 0;
}

mjx-container[jax="SVG"][display="true"][width="full"] {
  display: flex;
}

mjx-container[jax="SVG"][justify="left"] {
  text-align: left;
}

mjx-container[jax="SVG"][justify="right"] {
  text-align: right;
}

g[data-mml-node="merror"] > g {
  fill: red;
  stroke: red;
}

g[data-mml-node="merror"] > rect[data-background] {
  fill: yellow;
  stroke: none;
}

g[data-mml-node="mtable"] > line[data-line], svg[data-table] > g > line[data-line] {
  stroke-width: 70px;
  fill: none;
}

g[data-mml-node="mtable"] > rect[data-frame], svg[data-table] > g > rect[data-frame] {
  stroke-width: 70px;
  fill: none;
}

g[data-mml-node="mtable"] > .mjx-dashed, svg[data-table] > g > .mjx-dashed {
  stroke-dasharray: 140;
}

g[data-mml-node="mtable"] > .mjx-dotted, svg[data-table] > g > .mjx-dotted {
  stroke-linecap: round;
  stroke-dasharray: 0,140;
}

g[data-mml-node="mtable"] > g > svg {
  overflow: visible;
}

[jax="SVG"] mjx-tool {
  display: inline-block;
  position: relative;
  width: 0;
  height: 0;
}

[jax="SVG"] mjx-tool > mjx-tip {
  position: absolute;
  top: 0;
  left: 0;
}

mjx-tool > mjx-tip {
  display: inline-block;
  padding: .2em;
  border: 1px solid #888;
  font-size: 70%;
  background-color: #F8F8F8;
  color: black;
  box-shadow: 2px 2px 5px #AAAAAA;
}

g[data-mml-node="maction"][data-toggle] {
  cursor: pointer;
}

mjx-status {
  display: block;
  position: fixed;
  left: 1em;
  bottom: 1em;
  min-width: 25%;
  padding: .2em .4em;
  border: 1px solid #888;
  font-size: 90%;
  background-color: #F8F8F8;
  color: black;
}

foreignObject[data-mjx-xml] {
  font-family: initial;
  line-height: normal;
  overflow: visible;
}

mjx-container[jax="SVG"] path[data-c], mjx-container[jax="SVG"] use[data-c] {
  stroke-width: 3;
}

g[data-mml-node="xypic"] path {
  stroke-width: inherit;
}

.MathJax g[data-mml-node="xypic"] path {
  stroke-width: inherit;
}
 :root {--mermaid-font-zoom:1em ;}  @media print { @page {margin: 0 0 0 0;} body.typora-export {padding-left: 0; padding-right: 0;} #write {padding:0;}} .typora-export li, .typora-export p, .typora-export,  .footnote-line {white-space: normal;}
</style><title>README</title>
<!-- Font Awesome -->
<link rel="stylesheet" href="./Challenge Lab Creating a Static Website for the Café_files/all.css">
<style type="text/css">
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
</style><script type="text/javascript" src="./Challenge Lab Creating a Static Website for the Café_files/c7fa7451-6f95-4815-ac32-b8cc2537837a" data-awssuidacr="53831616-c450-4d58-b234-a61f3b697d56"></script>

</head>
<body class="typora-export vsc-initialized"><div class="typora-export-content">
<div id="write" class=""><!-- Font Awesome -->
<link rel="stylesheet" href="./Challenge Lab Creating a Static Website for the Café_files/all.css"><style type="text/css">
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
</style><h1 id="module-3-challenge-lab-creating-a-static-website-for-the-café"><span>Module 3 Challenge Lab: Creating a Static Website for the Café</span></h1><h2 id="scenario"><span>Scenario</span></h2><p><span>Frank and Martha are a husband-and-wife team who own and operate a small café business that sells desserts and coffee. Their daughter, Sofía, and their other employee, Nikhil—who is a secondary school student—also work at the café. The café has a single location in a large city.</span></p><p><span>The café currently doesn’t have a marketing strategy. They mostly gain new customers when someone walks by, notices the café, and decides to try it. The café has a reputation for high-quality desserts and coffees, but their reputation is limited to people who have visited, or who have heard about them from their customers.</span></p><p><span>Sofía suggests to Frank and Martha that they should expand community awareness of what the café has to offer. The café doesn’t have a web presence yet, and it doesn’t currently use any cloud computing services. However, that situation is about to change.</span></p><br><h2 id="lab-overview-and-objectives"><span>Lab overview and objectives</span></h2><p><span>In this lab, you use Amazon Simple Storage Service (Amazon S3) to build a static website and implement architectural best practices to protect and manage your data.</span></p><p><span>After completing this lab, you should be able to:</span></p><ul><li><span>Host a static website by using Amazon S3</span></li><li><span>Implement one way to protect your data with Amazon S3</span></li><li><span>Implement a data lifecycle strategy in Amazon S3</span></li><li><span>Implement a disaster recovery (DR) strategy in Amazon S3</span>
<br>
<span>At the end of this lab, your architecture should look like the following example:</span></li></ul><p><img src="./Challenge Lab Creating a Static Website for the Café_files/module-3-challenge-lab-cafe-static-website-architecture.PNG" referrerpolicy="no-referrer" alt="cafe website architecture"></p><p><br>
<strong><span>Note:</span></strong><span> In this challenge lab, you will encounter a few tasks where step-by-step instructions are not provided. You must figure out how to complete the tasks on your own.</span></p><br><h2 id="duration"><span>Duration</span></h2><p><span>This lab will require approximately </span><strong><span>60 minutes</span></strong><span> to complete.</span></p><br><h2 id="aws-service-restrictions"><span>AWS service restrictions</span></h2><p><span>In this lab environment, access to AWS services and service actions might be restricted to the ones that are needed to complete the lab instructions. You might encounter errors if you attempt to access other services or perform actions beyond the ones that are described in this lab.</span></p><br><h2 id="accessing-the-aws-management-console"><span>Accessing the AWS Management Console</span></h2><ol start=""><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>Start Lab</span></span><span> to launch your lab.</span></p><p><span>A </span><strong><span>Start Lab</span></strong><span> panel opens, and it displays the lab status.</span></p><p><strong><span>Tip</span></strong><span>: If you need more time to complete the lab, choose the Start Lab button again to restart the timer for the environment.</span></p></li><li><p><span>Wait until you see the message </span><em><span>Lab status: ready</span></em><span>, then close the </span><strong><span>Start Lab</span></strong><span> panel by choosing the </span><strong><span>X</span></strong><span>.</span></p></li><li><p><span>At the top of these instructions, choose </span><span id="ssb_voc_grey"><span>AWS</span></span><span>.</span></p><p><span>This opens the AWS Management Console in a new browser tab. The system will automatically log you in.</span></p><p><strong><span>Tip</span></strong><span>: If a new browser tab does not open, a banner or icon is usually at the top of your browser with a message that your browser is preventing the site from opening pop-up windows. Choose the banner or icon and then choose </span><strong><span>Allow pop ups</span></strong><span>.</span></p></li><li><p><span>Arrange the AWS Management Console tab so that it displays along side these instructions. Ideally, you will be able to see both browser tabs at the same time so that you can follow the lab steps more easily.</span></p></li></ol><br><h2 id="a-business-request-for-the-café-launching-a-static-website-challenge-1"><span>A business request for the café: Launching a static website (Challenge #1)</span></h2><p><span>Sofía mentions to Nikhil that she would like the café to have a website that will visually showcase the café's offerings. It would also provide customers with business details, such as the location of the store, business hours, and telephone number.</span></p><p><span>Nikhil is happy that he was asked to create the first website for the café.</span></p><p><span>For this first challenge, you will take on the role of Nikhil and use Amazon S3 to create a basic website for the café.</span></p><br><h3 id="task-1-extracting-the-files-that-you-need-for-this-lab"><span>Task 1: Extracting the files that you need for this lab</span></h3><p><span>In this task, you will extract the files that you need to create the static website.</span></p><ol start="5"><li><span>Download the </span><em><span>.zip</span></em><span> file you need for this lab by opening </span><a href="https://aws-tc-largeobjects.s3-us-west-2.amazonaws.com/ILT-TF-200-ACACAD-20-EN/Module-3-Challenge-Lab/static-website.zip" target="_blank" rel="noopener noreferrer"><span>this Amazon S3 link</span></a><span>.</span></li><li><span>On your computer, extract the files. Notice that you have an </span><em><span>index.html</span></em><span> file, and two folders that contain Cascading Style Sheets (CSS) and image files.</span></li></ol><br><h3 id="task-2-creating-an-s3-bucket-to-host-your-static-website"><span>Task 2: Creating an S3 bucket to host your static website</span></h3><p><span>In this task, you will create an S3 bucket and configure it to host your static website.</span></p><ol start="7"><li><p><span>Open the </span><strong><span>Amazon S3 console</span></strong><span>.</span></p></li><li><p><span>Create a bucket to host your static website.</span></p><ul><li><span>Create the bucket in the </span><strong><span>N. Virginia</span></strong><span> (us-east-1) AWS Region.</span></li><li><strong><span>Tip</span></strong><span>: You must disable </span><strong><span>Block </span><em><span>all</span></em><span> public access</span></strong><span>.</span></li></ul></li><li><p><span>Enable static website hosting on your bucket.</span></p><ul><li><strong><span>Tip</span></strong><span>: You will use the </span><em><span>index.html</span></em><span> file for your index document.</span></li></ul></li></ol><br><h3 id="task-3-uploading-content-to-your-s3-bucket"><span>Task 3: Uploading content to your S3 bucket</span></h3><p><span>In this task, you will upload the static files to your S3 bucket.</span></p><ol start="10"><li><span>Upload the </span><em><span>index.html</span></em><span> file and the </span><em><span>css</span></em><span> and </span><em><span>images</span></em><span> folders to your S3 bucket.</span></li><li><span>In a separate web browser tab, open the endpoint link for your static website.</span></li></ol><br><h4 id="answering-questions-about-the-lab"><span>Answering questions about the lab</span></h4><p><span>Answers will be recorded when you choose the blue </span><strong><span>Submit</span></strong><span> button above at the end of the lab.</span></p><ol start="12"><li><p><span>Access the questions in this lab.</span></p><ul><li><span>Choose the </span><span id="ssb_voc_grey"><span>Details </span><i class="fas fa-angle-down"></i></span>
<span>menu, and choose </span><span id="ssb_voc_grey"><span>Show</span></span><span>.</span></li><li><span>Choose the </span><strong><span>Access the multiple choice questions</span></strong><span> link that appears at the bottom of the page.</span></li></ul></li><li><p><span>In the page you loaded, answer the first question:</span></p><ul><li><strong><span>Question 1</span></strong><span>: When viewing the website after Task 3, do you see the page in the browser?</span></li></ul></li></ol><p><span>  </span><strong><span>Note</span></strong><span>: Leave the questions webpage open in your browser tab. You will return to it later in this lab.</span></p><br><h3 id="task-4-creating-a-bucket-policy-to-grant-public-read-access"><span>Task 4: Creating a bucket policy to grant public read access</span></h3><p><span>Frank shares his plan to create </span><em><span>many</span></em><span> new types of pastries for the café. You realize that you will need to upload an image for each new dessert that he creates, and enable public access on that object. You don't want to do this process manually. Instead, you decide to create a bucket policy that automatically makes each object public when it's uploaded to the folder.</span></p><ol start="14"><li><span>Create a bucket policy that grants read-only permission to public anonymous users by using the Bucket Policy editor.</span></li></ol><p><span>  </span><strong><span>Hint</span></strong><span>: If you get stuck, refer to the examples in the </span><a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/example-bucket-policies.html" target="_blank" rel="noopener noreferrer"><span>AWS Documentation</span></a><span>.</span></p><ol start="15"><li><span>Confirm that the website for the café is now publicly accessible.</span></li></ol><p><br>
<em><span>Congratulations!</span></em><span> You now have a static website for the café.</span>
<br></p><h2 id="new-business-requirement-protecting-website-data-challenge-2"><span>New business requirement: Protecting website data (Challenge #2)</span></h2><p><span>You show Sofía the new website, and she's very impressed. Good job!</span></p><p><span>You and Sofía discuss that you will likely need to make many updates to the website as the number of café offerings expands.</span></p><p><span>Olivia, an AWS Solutions Architect and café regular, advises you to implement a strategy to prevent the accidental overwrite and deletion of website objects.</span></p><p><span>You already need to make some changes to the website, so you decide that this would be a good time to explore object versioning.</span></p><br><h3 id="task-5-enabling-versioning-on-the-s3-bucket"><span>Task 5: Enabling versioning on the S3 bucket</span></h3><p><span>In this task, you will enable versioning on your S3 bucket and confirm that it works.</span></p><ol start="16"><li><span>In the S3 console, enable versioning on your S3 bucket.</span></li></ol><p><span>  </span><strong><span>Note</span></strong><span>: Notice that after you enable versioning, you can't disable it.</span></p><ol start="17"><li><p><span>In your favorite text editor, open the </span><em><span>index.html</span></em><span> file. For example, you could use Notepad++ or TextWrangler.</span></p></li><li><p><span>Modify the file according to the following instructions:</span></p><ul><li><span>Locate the first line that has the embedded CSS code </span><strong><span>bgcolor="aquamarine"</span></strong><span> in the HTML, and change it to </span><code>bgcolor="gainsboro"</code><span>.</span></li><li><span>Locate the line that has the embedded CSS code </span><strong><span>bgcolor="orange"</span></strong><span> in the HTML, and change it to </span><code>bgcolor="cornsilk"</code><span>.</span></li><li><span>Locate the second line that has the embedded CSS code </span><strong><span>bgcolor="aquamarine"</span></strong><span> in the HTML, and change it to </span><code>bgcolor="gainsboro"</code><span>.</span></li><li><span>Save the changes.</span></li></ul></li><li><p><span>Upload the updated file to your S3 bucket.</span></p></li><li><p><span>Reload the web browser tab with your website and notice the changes.</span></p></li><li><p><span>To see the latest version of the </span><em><span>index.html</span></em><span> file, go to your bucket and choose </span><strong><span>List versions</span></strong><span>. You should see both versions of this file in the dropdown menu.</span></p></li><li><p><span>Return to the browser tab with the multiple-choice questions for this lab, and answer the following question:</span></p><ul><li><strong><span>Question 2</span></strong><span>: What is another way to ensure maximum protection and prevent the accidental deletion of a preserved version? (</span><strong><span>Hint</span></strong><span>: Review the </span><a href="https://aws.amazon.com/s3/faqs/" target="_blank" rel="noopener noreferrer"><span>Amazon S3 FAQs</span></a><span>.)</span></li></ul></li></ol><p><br>
<br>
<strong><span>Architecture best practice</span></strong></p><p><span>In this task, you used one technique to implement the architecture best practice of </span><em><span>protecting your data</span></em><span>.</span></p><details>
	<summary>Expand <b>here</b> to learn more about it.</summary>
	According to the <a href="https://d1.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf" target="_blank" rel="noopener noreferrer">Well-Architected Framework</a>, versioning can be part of a larger data lifecycle management process. Before you architect any system, foundational practices that influence security should be in place. For example, <i>data classification</i> provides a way to categorize organizational data based on levels of sensitivity. <i>Encryption</i> protects data by rendering it unintelligible to unauthorized access. These tools and techniques are important because they support objectives such as preventing financial loss or complying with regulatory obligations.
</details><br><h2 id="new-business-requirement-optimizing-costs-of-s3-object-storage-challenge-3"><span>New business requirement: Optimizing costs of S3 object storage (Challenge #3)</span></h2><p><span>Now that you enabled versioning, you realize that the size of the S3 bucket will continue to grow as you upload new objects and versions. To save costs, you decide to implement a strategy to retire some of those older versions.</span></p><br><h3 id="task-6-setting-lifecycle-policies"><span>Task 6: Setting lifecycle policies</span></h3><p><span>In this task, you will set a lifecycle policy to automatically move older versions of the objects in your source bucket to S3 Standard-Infrequent Access (S3 Standard-IA). The policy should also eventually expire the objects.</span></p><ol start="23"><li><p><span>Configure two rules in the website bucket's lifecycle configuration. To receive full credit, create two separate rules. Do not configure two transitions in a single rule:</span></p><ul><li><span>In one rule, move previous versions of all source bucket objects to S3 Standard-IA after 30 days</span></li><li><span>In the other rule, delete previous versions of the objects after 365 days</span>
<br><strong><span>Hint</span></strong><span>: If you get stuck, refer to the </span><a href="https://docs.aws.amazon.com/AmazonS3/latest/user-guide/create-lifecycle.html" target="_blank" rel="noopener noreferrer"><span>AWS Documentation</span></a><span> for guidance.</span>
<br>
<strong><span>Note</span></strong><span>: To </span><em><span>limit the scope</span></em><span> of the replication to a particular bucket object (for example, the </span><em><span>index.html</span></em><span> file), create a tag for the object before you create the lifecycle rule.</span>
<br></li></ul></li></ol><p><span>Good! You should now have a lifecycle configuration that will move previous versions of your source bucket objects to S3 Standard-IA after 30 days. The policy will also permanently delete the objects that are in S3 Standard-IA after 365 days.</span></p><p><br>
<strong><span>Architecture best practice</span></strong></p><p><span>In this task, you implemented the architecture best practice of </span><em><span>defining data lifecycle management.</span></em></p><details>
	<summary>Expand <b>here</b> to learn more about it.</summary>
	According to the <a href="https://d1.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf" target="_blank" rel="noopener noreferrer">Well-Architected Framework</a>, in practice, your lifecycle strategy should be based on the <i>criticality and sensitivity</i> of your data, and <i>legal and organizational requirements</i>. You should consider factors such as data retention duration, data destruction, data access management, data transformation, and data sharing.
</details><br><h2 id="new-business-requirement-enhancing-durability-and-planning-for-dr-challenge-4"><span>New business requirement: Enhancing durability and planning for DR (Challenge #4)</span></h2><p><span>The next time Olivia comes to the café, you tell her about the updates to the website. You describe the measures that you took to protect the website's static files from being accidentally overwritten or deleted. Olivia tells you that cross-Region replication is another feature of Amazon S3 that you can also use to back up and archive critical data.</span></p><br><h3 id="task-7-enabling-cross-region-replication"><span>Task 7: Enabling cross-Region replication</span></h3><p><span>In this task, you will enable cross-Region replication on your source S3 bucket.</span></p><ol start="24"><li><p><span>In a different Region than your source bucket, create a second bucket and enable versioning on it. The second bucket is your </span><em><span>destination bucket</span></em><span>.</span></p></li><li><p><span>On your source S3 bucket, enable cross-Region replication. When you create the replication rule, make sure that you:</span></p><ul><li><span>Replicate the entire source bucket.</span></li><li><span>Use the </span><strong><span>CafeRole</span></strong><span> for the AWS Identity and Access Management (IAM) role. This IAM role gives Amazon S3 the permissions to read objects from the source bucket and replicate them to the destination bucket.</span></li><li><span>If you encounter the warning </span><em><span>The replication rule is saved, but it might not work</span></em><span>, you can ignore it and proceed to the next step.</span>
<br>
<strong><span>Hint</span></strong><span>: If you get stuck, refer to the </span><a href="https://docs.aws.amazon.com/AmazonS3/latest/user-guide/enable-replication.html#enable-replication-add-rule" target="_blank" rel="noopener noreferrer"><span>AWS Documentation</span></a><span> for guidance.</span>
<br>
<strong><span>Note:</span></strong><span> </span><em><span>CafeRole</span></em><span> has the following permissions:</span></li></ul></li></ol><pre class="md-fences md-end-block ty-contain-cm modeLoaded" spellcheck="false" lang="yaml"><div class="CodeMirror cm-s-inner cm-s-null-scroll CodeMirror-wrap" lang="yaml"><div style="overflow: hidden; position: relative; width: 3px; height: 0px; top: 9px; left: 8px;"><textarea autocorrect="off" autocapitalize="off" spellcheck="false" tabindex="0" style="position: absolute; bottom: -1em; padding: 0px; width: 1000px; height: 1em; outline: none;"></textarea></div><div class="CodeMirror-scrollbar-filler" cm-not-content="true"></div><div class="CodeMirror-gutter-filler" cm-not-content="true"></div><div class="CodeMirror-scroll" tabindex="-1"><div class="CodeMirror-sizer" style="margin-left: 0px; margin-bottom: 0px; border-right-width: 0px; padding-right: 0px; padding-bottom: 0px;"><div style="position: relative; top: 0px;"><div class="CodeMirror-lines" role="presentation"><div role="presentation" style="position: relative; outline: none;"><div class="CodeMirror-measure"></div><div class="CodeMirror-measure"></div><div style="position: relative; z-index: 1;"></div><div class="CodeMirror-code" role="presentation" style=""><div class="CodeMirror-activeline" style="position: relative;"><div class="CodeMirror-activeline-background CodeMirror-linebackground"></div><div class="CodeMirror-gutter-background CodeMirror-activeline-gutter" style="left: 0px; width: 0px;"></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-atom">Version</span><span class="cm-meta">: </span>2012-10-17</span></pre></div><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-atom">Statement</span><span class="cm-meta">:</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-meta">  - </span><span class="cm-atom">Action</span><span class="cm-meta">:</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-meta"><span class="cm-tab" role="presentation" cm-text="	">  </span>- </span>s3:ListBucket</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-meta"><span class="cm-tab" role="presentation" cm-text="	">  </span>- </span>s3:ReplicateObject</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-meta"><span class="cm-tab" role="presentation" cm-text="	">  </span>- </span>s3:ReplicateDelete</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-meta"><span class="cm-tab" role="presentation" cm-text="	">  </span>- </span>s3:ReplicateTags</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-meta"><span class="cm-tab" role="presentation" cm-text="	">  </span>- </span>s3:Get*</span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-atom"> &nbsp;  Resource</span><span class="cm-meta">:</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-meta"><span class="cm-tab" role="presentation" cm-text="	">  </span>- </span><span class="cm-string">'*'</span></span></pre><pre class=" CodeMirror-line " role="presentation"><span role="presentation" style="padding-right: 0.1px;"><span class="cm-atom"> &nbsp;  Effect</span><span class="cm-meta">: </span>Allow</span></pre></div></div></div></div></div><div style="position: absolute; height: 0px; width: 1px; border-bottom-width: 0px; border-bottom-style: solid; border-bottom-color: transparent; top: 242px;"></div><div class="CodeMirror-gutters" style="display: none; height: 242px;"></div></div></div></pre><p><span>This access policy allows the role to perform the replication tasks on </span><em><span>all</span></em><span> S3 buckets. In a real production environment, you should restrict the policy to apply only to your source and destination S3 buckets. For more information about creating an IAM role, refer to </span><a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/setting-repl-config-perm-overview.html" target="_blank" rel="noopener noreferrer"><span>Setting Up Permissions for Replication</span></a><span>.</span>
<br></p><ol start="26"><li><p><span>Return to the browser tab with the multiple-choice questions for this lab, and answer the following question:</span></p><ul><li><strong><span>Question 3</span></strong><span>: Do you see the objects from your source bucket in the destination bucket?</span></li></ul></li><li><p><span>Make a minor change to the </span><em><span>index.html</span></em><span> file and upload the new version to your source bucket.</span></p></li><li><p><span>Verify that the source bucket now has three versions of the </span><em><span>index.html</span></em><span> file.</span></p></li><li><p><span>Confirm that the new object was replicated to your destination bucket. You might need to reload the browser tab.</span></p></li><li><p><span>Go to your source bucket and delete the latest version.</span></p></li><li><p><span>Return to the browser tab with the multiple-choice questions for this lab, and answer the following question:</span></p><ul><li><strong><span>Question 4</span></strong><span>: Was the version that you just deleted from your source bucket also deleted from your destination bucket?</span></li></ul></li></ol><p><br>
<strong><span>Architecture best practice</span></strong></p><p><span>In this task, you implemented the architecture best practice of </span><em><span>automating disaster recovery</span></em><span>.</span></p><details>
	<summary>Expand <b>here</b> to learn more about it.</summary>
	According to the <a href="https://d1.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf" target="_blank" rel="noopener noreferrer">Well-Architected Framework</a>, the start of your DR strategy is <i>having backups and redundant workload components in place</i>. You should use AWS or third-party tools to automate system recovery and route traffic to the DR site or Region.
</details><br><h2 id="submitting-your-work"><span>Submitting your work</span></h2><ol start="32"><li><p><span>At the top of these instructions, choose </span><span id="ssb_blue"><span>Submit</span></span><span> to record your progress and when prompted, choose </span><strong><span>Yes</span></strong><span>.</span></p></li><li><p><span>If the results don't display after a couple of minutes, return to the top of these instructions and choose </span><span id="ssb_voc_grey"><span>Grades</span></span></p><p><span> </span><strong><span>Tip</span></strong><span>: You can submit your work multiple times. After you change your work, choose </span><strong><span>Submit</span></strong><span> again. Your last submission is what will be recorded for this lab.</span></p></li><li><p><span>To find detailed feedback on your work, choose </span><span id="ssb_voc_grey"><span>Details</span></span><span> followed by </span><i class="fas fa-caret-right"></i><span> </span><strong><span>View Submission Report</span></strong><span>.</span></p></li></ol><br><h2 id="lab-complete"><span>Lab complete</span></h2><p><i class="fas fa-flag-checkered"></i><span> Congratulations! You have completed the lab.</span></p><ol start="35"><li><p><span>To confirm that you want to end the lab, at the top of this page, choose </span><strong><span id="ssb_voc_grey"><span>End Lab</span></span></strong><span>, and then choose </span><strong><span id="ssb_blue"><span>Yes</span></span></strong><span>.  </span></p><p><span>A panel should appear with this message: </span><em><span>DELETE has been initiated... You may close this message box now.</span></em></p></li><li><p><span>To close the panel, choose the </span><strong><span>X</span></strong><span> in the top-right corner.</span></p></li></ol><p>&nbsp;</p><p><br>
<em><span>©2020 Amazon Web Services, Inc. and its affiliates. All rights reserved. This work may not be reproduced or redistributed, in whole or in part, without prior written permission from Amazon Web Services, Inc. Commercial copying, lending, or selling is prohibited.</span></em></p></div></div>
<script defer="" src="./Challenge Lab Creating a Static Website for the Café_files/vcd15cbe7772f49c399c6a5babf22c1241717689176015" integrity="sha512-ZpsOmlRQV6y907TI0dKBHq9Md29nnaEIPlkf84rnaERnq6zvWvPUqr2ft8M1aS28oN72PdrCzSjY4U6VaAw1EQ==" data-cf-beacon="{&quot;rayId&quot;:&quot;8ba0a5ac7ffb02fd&quot;,&quot;serverTiming&quot;:{&quot;name&quot;:{&quot;cfL4&quot;:true}},&quot;version&quot;:&quot;2024.8.0&quot;,&quot;token&quot;:&quot;a73834a4a1444e9ab89e8da06da41720&quot;}" crossorigin="anonymous"></script>


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