# jasoncavanaugh.github.io
<!DOCTYPE html>
<html>
<head><meta charset="utf-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>What is the relationship between professor ratings and grades?</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>




<style type="text/css">
    pre { line-height: 125%; }
td.linenos pre { color: #000000; background-color: #f0f0f0; padding-left: 5px; padding-right: 5px; }
span.linenos { color: #000000; background-color: #f0f0f0; padding-left: 5px; padding-right: 5px; }
td.linenos pre.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
span.linenos.special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
.highlight .hll { background-color: var(--jp-cell-editor-active-background) }
.highlight { background: var(--jp-cell-editor-background); color: var(--jp-mirror-editor-variable-color) }
.highlight .c { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment */
.highlight .err { color: var(--jp-mirror-editor-error-color) } /* Error */
.highlight .k { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword */
.highlight .o { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator */
.highlight .p { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation */
.highlight .ch { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Multiline */
.highlight .cp { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Preproc */
.highlight .cpf { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Single */
.highlight .cs { color: var(--jp-mirror-editor-comment-color); font-style: italic } /* Comment.Special */
.highlight .kc { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Pseudo */
.highlight .kr { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: var(--jp-mirror-editor-keyword-color); font-weight: bold } /* Keyword.Type */
.highlight .m { color: var(--jp-mirror-editor-number-color) } /* Literal.Number */
.highlight .s { color: var(--jp-mirror-editor-string-color) } /* Literal.String */
.highlight .ow { color: var(--jp-mirror-editor-operator-color); font-weight: bold } /* Operator.Word */
.highlight .w { color: var(--jp-mirror-editor-variable-color) } /* Text.Whitespace */
.highlight .mb { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Bin */
.highlight .mf { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Float */
.highlight .mh { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Hex */
.highlight .mi { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer */
.highlight .mo { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Oct */
.highlight .sa { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Affix */
.highlight .sb { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Backtick */
.highlight .sc { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Char */
.highlight .dl { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Delimiter */
.highlight .sd { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Doc */
.highlight .s2 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Double */
.highlight .se { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Escape */
.highlight .sh { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Heredoc */
.highlight .si { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Interpol */
.highlight .sx { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Other */
.highlight .sr { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Regex */
.highlight .s1 { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Single */
.highlight .ss { color: var(--jp-mirror-editor-string-color) } /* Literal.String.Symbol */
.highlight .il { color: var(--jp-mirror-editor-number-color) } /* Literal.Number.Integer.Long */
  </style>



<style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
 * Mozilla scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */
[data-jp-theme-scrollbars='true'] {
  scrollbar-color: rgb(var(--jp-scrollbar-thumb-color))
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar. These selectors
 * will match lower in the tree, and so will override the above */
[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
}

/*
 * Webkit scrollbar styling
 */

/* use standard opaque scrollbars for most nodes */

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-corner {
  background: var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-thumb {
  background: rgb(var(--jp-scrollbar-thumb-color));
  border: var(--jp-scrollbar-thumb-margin) solid transparent;
  background-clip: content-box;
  border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:horizontal {
  border-left: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
  border-right: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
}

[data-jp-theme-scrollbars='true'] ::-webkit-scrollbar-track:vertical {
  border-top: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
  border-bottom: var(--jp-scrollbar-endpad) solid
    var(--jp-scrollbar-background-color);
}

/* for code nodes, use a transparent style of scrollbar */

[data-jp-theme-scrollbars='true'] .CodeMirror-hscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true'] .CodeMirror-vscrollbar::-webkit-scrollbar,
[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-corner,
[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-corner {
  background-color: transparent;
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-thumb,
[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
  border: var(--jp-scrollbar-thumb-margin) solid transparent;
  background-clip: content-box;
  border-radius: var(--jp-scrollbar-thumb-radius);
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-hscrollbar::-webkit-scrollbar-track:horizontal {
  border-left: var(--jp-scrollbar-endpad) solid transparent;
  border-right: var(--jp-scrollbar-endpad) solid transparent;
}

[data-jp-theme-scrollbars='true']
  .CodeMirror-vscrollbar::-webkit-scrollbar-track:vertical {
  border-top: var(--jp-scrollbar-endpad) solid transparent;
  border-bottom: var(--jp-scrollbar-endpad) solid transparent;
}

/*
 * Phosphor
 */

.lm-ScrollBar[data-orientation='horizontal'] {
  min-height: 16px;
  max-height: 16px;
  min-width: 45px;
  border-top: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] {
  min-width: 16px;
  max-width: 16px;
  min-height: 45px;
  border-left: 1px solid #a0a0a0;
}

.lm-ScrollBar-button {
  background-color: #f0f0f0;
  background-position: center center;
  min-height: 15px;
  max-height: 15px;
  min-width: 15px;
  max-width: 15px;
}

.lm-ScrollBar-button:hover {
  background-color: #dadada;
}

.lm-ScrollBar-button.lm-mod-active {
  background-color: #cdcdcd;
}

.lm-ScrollBar-track {
  background: #f0f0f0;
}

.lm-ScrollBar-thumb {
  background: #cdcdcd;
}

.lm-ScrollBar-thumb:hover {
  background: #bababa;
}

.lm-ScrollBar-thumb.lm-mod-active {
  background: #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal'] .lm-ScrollBar-thumb {
  height: 100%;
  min-width: 15px;
  border-left: 1px solid #a0a0a0;
  border-right: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='vertical'] .lm-ScrollBar-thumb {
  width: 100%;
  min-height: 15px;
  border-top: 1px solid #a0a0a0;
  border-bottom: 1px solid #a0a0a0;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-left);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='horizontal']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-right);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='decrement'] {
  background-image: var(--jp-icon-caret-up);
  background-size: 17px;
}

.lm-ScrollBar[data-orientation='vertical']
  .lm-ScrollBar-button[data-action='increment'] {
  background-image: var(--jp-icon-caret-down);
  background-size: 17px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-Widget, /* </DEPRECATED> */
.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  cursor: default;
}


/* <DEPRECATED> */ .p-Widget.p-mod-hidden, /* </DEPRECATED> */
.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-CommandPalette, /* </DEPRECATED> */
.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-CommandPalette-search, /* </DEPRECATED> */
.lm-CommandPalette-search {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-content, /* </DEPRECATED> */
.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}


/* <DEPRECATED> */ .p-CommandPalette-header, /* </DEPRECATED> */
.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}


/* <DEPRECATED> */ .p-CommandPalette-item, /* </DEPRECATED> */
.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}


/* <DEPRECATED> */ .p-CommandPalette-itemIcon, /* </DEPRECATED> */
.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-itemContent, /* </DEPRECATED> */
.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}


/* <DEPRECATED> */ .p-CommandPalette-itemShortcut, /* </DEPRECATED> */
.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-CommandPalette-itemLabel, /* </DEPRECATED> */
.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-DockPanel, /* </DEPRECATED> */
.lm-DockPanel {
  z-index: 0;
}


/* <DEPRECATED> */ .p-DockPanel-widget, /* </DEPRECATED> */
.lm-DockPanel-widget {
  z-index: 0;
}


/* <DEPRECATED> */ .p-DockPanel-tabBar, /* </DEPRECATED> */
.lm-DockPanel-tabBar {
  z-index: 1;
}


/* <DEPRECATED> */ .p-DockPanel-handle, /* </DEPRECATED> */
.lm-DockPanel-handle {
  z-index: 2;
}


/* <DEPRECATED> */ .p-DockPanel-handle.p-mod-hidden, /* </DEPRECATED> */
.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-DockPanel-handle:after, /* </DEPRECATED> */
.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='horizontal'],
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='vertical'],
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='horizontal']:after,
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}


/* <DEPRECATED> */
.p-DockPanel-handle[data-orientation='vertical']:after,
/* </DEPRECATED> */
.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}


/* <DEPRECATED> */ .p-DockPanel-overlay, /* </DEPRECATED> */
.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}


/* <DEPRECATED> */ .p-DockPanel-overlay.p-mod-hidden, /* </DEPRECATED> */
.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-Menu, /* </DEPRECATED> */
.lm-Menu {
  z-index: 10000;
  position: absolute;
  white-space: nowrap;
  overflow-x: hidden;
  overflow-y: auto;
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-Menu-content, /* </DEPRECATED> */
.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}


/* <DEPRECATED> */ .p-Menu-item, /* </DEPRECATED> */
.lm-Menu-item {
  display: table-row;
}


/* <DEPRECATED> */
.p-Menu-item.p-mod-hidden,
.p-Menu-item.p-mod-collapsed,
/* </DEPRECATED> */
.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}


/* <DEPRECATED> */
.p-Menu-itemIcon,
.p-Menu-itemSubmenuIcon,
/* </DEPRECATED> */
.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}


/* <DEPRECATED> */ .p-Menu-itemLabel, /* </DEPRECATED> */
.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}


/* <DEPRECATED> */ .p-Menu-itemShortcut, /* </DEPRECATED> */
.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-MenuBar, /* </DEPRECATED> */
.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-MenuBar-content, /* </DEPRECATED> */
.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}


/* <DEPRECATED> */ .p--MenuBar-item, /* </DEPRECATED> */
.lm-MenuBar-item {
  box-sizing: border-box;
}


/* <DEPRECATED> */
.p-MenuBar-itemIcon,
.p-MenuBar-itemLabel,
/* </DEPRECATED> */
.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-ScrollBar, /* </DEPRECATED> */
.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */
.p-ScrollBar[data-orientation='horizontal'],
/* </DEPRECATED> */
.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}


/* <DEPRECATED> */
.p-ScrollBar[data-orientation='vertical'],
/* </DEPRECATED> */
.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-ScrollBar-button, /* </DEPRECATED> */
.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-ScrollBar-track, /* </DEPRECATED> */
.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}


/* <DEPRECATED> */ .p-ScrollBar-thumb, /* </DEPRECATED> */
.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-SplitPanel-child, /* </DEPRECATED> */
.lm-SplitPanel-child {
  z-index: 0;
}


/* <DEPRECATED> */ .p-SplitPanel-handle, /* </DEPRECATED> */
.lm-SplitPanel-handle {
  z-index: 1;
}


/* <DEPRECATED> */ .p-SplitPanel-handle.p-mod-hidden, /* </DEPRECATED> */
.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-SplitPanel-handle:after, /* </DEPRECATED> */
.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='horizontal'] > .p-SplitPanel-handle:after,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}


/* <DEPRECATED> */
.p-SplitPanel[data-orientation='vertical'] > .p-SplitPanel-handle:after,
/* </DEPRECATED> */
.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-TabBar, /* </DEPRECATED> */
.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}


/* <DEPRECATED> */ .p-TabBar[data-orientation='horizontal'], /* </DEPRECATED> */
.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
}


/* <DEPRECATED> */ .p-TabBar[data-orientation='vertical'], /* </DEPRECATED> */
.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-TabBar-content, /* </DEPRECATED> */
.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}


/* <DEPRECATED> */
.p-TabBar[data-orientation='horizontal'] > .p-TabBar-content,
/* </DEPRECATED> */
.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}


/* <DEPRECATED> */
.p-TabBar[data-orientation='vertical'] > .p-TabBar-content,
/* </DEPRECATED> */
.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}


/* <DEPRECATED> */ .p-TabBar-tab, /* </DEPRECATED> */
.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
}


/* <DEPRECATED> */
.p-TabBar-tabIcon,
.p-TabBar-tabCloseIcon,
/* </DEPRECATED> */
.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}


/* <DEPRECATED> */ .p-TabBar-tabLabel, /* </DEPRECATED> */
.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}


/* <DEPRECATED> */ .p-TabBar-tab.p-mod-hidden, /* </DEPRECATED> */
.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}


/* <DEPRECATED> */ .p-TabBar.p-mod-dragging .p-TabBar-tab, /* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging[data-orientation='horizontal'] .p-TabBar-tab,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging[data-orientation='vertical'] .p-TabBar-tab,
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}


/* <DEPRECATED> */
.p-TabBar.p-mod-dragging .p-TabBar-tab.p-mod-dragging
/* </DEPRECATED> */
.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ .p-TabPanel-tabBar, /* </DEPRECATED> */
.lm-TabPanel-tabBar {
  z-index: 1;
}


/* <DEPRECATED> */ .p-TabPanel-stackedPanel, /* </DEPRECATED> */
.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

@charset "UTF-8";
/*!

Copyright 2015-present Palantir Technologies, Inc. All rights reserved.
Licensed under the Apache License, Version 2.0.

*/
html{
  -webkit-box-sizing:border-box;
          box-sizing:border-box; }

*,
*::before,
*::after{
  -webkit-box-sizing:inherit;
          box-sizing:inherit; }

body{
  text-transform:none;
  line-height:1.28581;
  letter-spacing:0;
  font-size:14px;
  font-weight:400;
  color:#182026;
  font-family:-apple-system, "BlinkMacSystemFont", "Segoe UI", "Roboto", "Oxygen", "Ubuntu", "Cantarell", "Open Sans", "Helvetica Neue", "Icons16", sans-serif; }

p{
  margin-top:0;
  margin-bottom:10px; }

small{
  font-size:12px; }

strong{
  font-weight:600; }

::-moz-selection{
  background:rgba(125, 188, 255, 0.6); }

::selection{
  background:rgba(125, 188, 255, 0.6); }
.bp3-heading{
  color:#182026;
  font-weight:600;
  margin:0 0 10px;
  padding:0; }
  .bp3-dark .bp3-heading{
    color:#f5f8fa; }

h1.bp3-heading, .bp3-running-text h1{
  line-height:40px;
  font-size:36px; }

h2.bp3-heading, .bp3-running-text h2{
  line-height:32px;
  font-size:28px; }

h3.bp3-heading, .bp3-running-text h3{
  line-height:25px;
  font-size:22px; }

h4.bp3-heading, .bp3-running-text h4{
  line-height:21px;
  font-size:18px; }

h5.bp3-heading, .bp3-running-text h5{
  line-height:19px;
  font-size:16px; }

h6.bp3-heading, .bp3-running-text h6{
  line-height:16px;
  font-size:14px; }
.bp3-ui-text{
  text-transform:none;
  line-height:1.28581;
  letter-spacing:0;
  font-size:14px;
  font-weight:400; }

.bp3-monospace-text{
  text-transform:none;
  font-family:monospace; }

.bp3-text-muted{
  color:#5c7080; }
  .bp3-dark .bp3-text-muted{
    color:#a7b6c2; }

.bp3-text-disabled{
  color:rgba(92, 112, 128, 0.6); }
  .bp3-dark .bp3-text-disabled{
    color:rgba(167, 182, 194, 0.6); }

.bp3-text-overflow-ellipsis{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal; }
.bp3-running-text{
  line-height:1.5;
  font-size:14px; }
  .bp3-running-text h1{
    color:#182026;
    font-weight:600;
    margin-top:40px;
    margin-bottom:20px; }
    .bp3-dark .bp3-running-text h1{
      color:#f5f8fa; }
  .bp3-running-text h2{
    color:#182026;
    font-weight:600;
    margin-top:40px;
    margin-bottom:20px; }
    .bp3-dark .bp3-running-text h2{
      color:#f5f8fa; }
  .bp3-running-text h3{
    color:#182026;
    font-weight:600;
    margin-top:40px;
    margin-bottom:20px; }
    .bp3-dark .bp3-running-text h3{
      color:#f5f8fa; }
  .bp3-running-text h4{
    color:#182026;
    font-weight:600;
    margin-top:40px;
    margin-bottom:20px; }
    .bp3-dark .bp3-running-text h4{
      color:#f5f8fa; }
  .bp3-running-text h5{
    color:#182026;
    font-weight:600;
    margin-top:40px;
    margin-bottom:20px; }
    .bp3-dark .bp3-running-text h5{
      color:#f5f8fa; }
  .bp3-running-text h6{
    color:#182026;
    font-weight:600;
    margin-top:40px;
    margin-bottom:20px; }
    .bp3-dark .bp3-running-text h6{
      color:#f5f8fa; }
  .bp3-running-text hr{
    margin:20px 0;
    border:none;
    border-bottom:1px solid rgba(16, 22, 26, 0.15); }
    .bp3-dark .bp3-running-text hr{
      border-color:rgba(255, 255, 255, 0.15); }
  .bp3-running-text p{
    margin:0 0 10px;
    padding:0; }

.bp3-text-large{
  font-size:16px; }

.bp3-text-small{
  font-size:12px; }
a{
  text-decoration:none;
  color:#106ba3; }
  a:hover{
    cursor:pointer;
    text-decoration:underline;
    color:#106ba3; }
  a .bp3-icon, a .bp3-icon-standard, a .bp3-icon-large{
    color:inherit; }
  a code,
  .bp3-dark a code{
    color:inherit; }
  .bp3-dark a,
  .bp3-dark a:hover{
    color:#48aff0; }
    .bp3-dark a .bp3-icon, .bp3-dark a .bp3-icon-standard, .bp3-dark a .bp3-icon-large,
    .bp3-dark a:hover .bp3-icon,
    .bp3-dark a:hover .bp3-icon-standard,
    .bp3-dark a:hover .bp3-icon-large{
      color:inherit; }
.bp3-running-text code, .bp3-code{
  text-transform:none;
  font-family:monospace;
  border-radius:3px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2);
  background:rgba(255, 255, 255, 0.7);
  padding:2px 5px;
  color:#5c7080;
  font-size:smaller; }
  .bp3-dark .bp3-running-text code, .bp3-running-text .bp3-dark code, .bp3-dark .bp3-code{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
    background:rgba(16, 22, 26, 0.3);
    color:#a7b6c2; }
  .bp3-running-text a > code, a > .bp3-code{
    color:#137cbd; }
    .bp3-dark .bp3-running-text a > code, .bp3-running-text .bp3-dark a > code, .bp3-dark a > .bp3-code{
      color:inherit; }

.bp3-running-text pre, .bp3-code-block{
  text-transform:none;
  font-family:monospace;
  display:block;
  margin:10px 0;
  border-radius:3px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
  background:rgba(255, 255, 255, 0.7);
  padding:13px 15px 12px;
  line-height:1.4;
  color:#182026;
  font-size:13px;
  word-break:break-all;
  word-wrap:break-word; }
  .bp3-dark .bp3-running-text pre, .bp3-running-text .bp3-dark pre, .bp3-dark .bp3-code-block{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
    background:rgba(16, 22, 26, 0.3);
    color:#f5f8fa; }
  .bp3-running-text pre > code, .bp3-code-block > code{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:none;
    padding:0;
    color:inherit;
    font-size:inherit; }

.bp3-running-text kbd, .bp3-key{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  background:#ffffff;
  min-width:24px;
  height:24px;
  padding:3px 6px;
  vertical-align:middle;
  line-height:24px;
  color:#5c7080;
  font-family:inherit;
  font-size:12px; }
  .bp3-running-text kbd .bp3-icon, .bp3-key .bp3-icon, .bp3-running-text kbd .bp3-icon-standard, .bp3-key .bp3-icon-standard, .bp3-running-text kbd .bp3-icon-large, .bp3-key .bp3-icon-large{
    margin-right:5px; }
  .bp3-dark .bp3-running-text kbd, .bp3-running-text .bp3-dark kbd, .bp3-dark .bp3-key{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
    background:#394b59;
    color:#a7b6c2; }
.bp3-running-text blockquote, .bp3-blockquote{
  margin:0 0 10px;
  border-left:solid 4px rgba(167, 182, 194, 0.5);
  padding:0 20px; }
  .bp3-dark .bp3-running-text blockquote, .bp3-running-text .bp3-dark blockquote, .bp3-dark .bp3-blockquote{
    border-color:rgba(115, 134, 148, 0.5); }
.bp3-running-text ul,
.bp3-running-text ol, .bp3-list{
  margin:10px 0;
  padding-left:30px; }
  .bp3-running-text ul li:not(:last-child), .bp3-running-text ol li:not(:last-child), .bp3-list li:not(:last-child){
    margin-bottom:5px; }
  .bp3-running-text ul ol, .bp3-running-text ol ol, .bp3-list ol,
  .bp3-running-text ul ul,
  .bp3-running-text ol ul,
  .bp3-list ul{
    margin-top:5px; }

.bp3-list-unstyled{
  margin:0;
  padding:0;
  list-style:none; }
  .bp3-list-unstyled li{
    padding:0; }
.bp3-rtl{
  text-align:right; }

.bp3-dark{
  color:#f5f8fa; }

:focus{
  outline:rgba(19, 124, 189, 0.6) auto 2px;
  outline-offset:2px;
  -moz-outline-radius:6px; }

.bp3-focus-disabled :focus{
  outline:none !important; }
  .bp3-focus-disabled :focus ~ .bp3-control-indicator{
    outline:none !important; }

.bp3-alert{
  max-width:400px;
  padding:20px; }

.bp3-alert-body{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }
  .bp3-alert-body .bp3-icon{
    margin-top:0;
    margin-right:20px;
    font-size:40px; }

.bp3-alert-footer{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:reverse;
      -ms-flex-direction:row-reverse;
          flex-direction:row-reverse;
  margin-top:10px; }
  .bp3-alert-footer .bp3-button{
    margin-left:10px; }
.bp3-breadcrumbs{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-wrap:wrap;
      flex-wrap:wrap;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  margin:0;
  cursor:default;
  height:30px;
  padding:0;
  list-style:none; }
  .bp3-breadcrumbs > li{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center; }
    .bp3-breadcrumbs > li::after{
      display:block;
      margin:0 5px;
      background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M10.71 7.29l-4-4a1.003 1.003 0 0 0-1.42 1.42L8.59 8 5.3 11.29c-.19.18-.3.43-.3.71a1.003 1.003 0 0 0 1.71.71l4-4c.18-.18.29-.43.29-.71 0-.28-.11-.53-.29-.71z' fill='%235C7080'/%3e%3c/svg%3e");
      width:16px;
      height:16px;
      content:""; }
    .bp3-breadcrumbs > li:last-of-type::after{
      display:none; }

.bp3-breadcrumb,
.bp3-breadcrumb-current,
.bp3-breadcrumbs-collapsed{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  font-size:16px; }

.bp3-breadcrumb,
.bp3-breadcrumbs-collapsed{
  color:#5c7080; }

.bp3-breadcrumb:hover{
  text-decoration:none; }

.bp3-breadcrumb.bp3-disabled{
  cursor:not-allowed;
  color:rgba(92, 112, 128, 0.6); }

.bp3-breadcrumb .bp3-icon{
  margin-right:5px; }

.bp3-breadcrumb-current{
  color:inherit;
  font-weight:600; }
  .bp3-breadcrumb-current .bp3-input{
    vertical-align:baseline;
    font-size:inherit;
    font-weight:inherit; }

.bp3-breadcrumbs-collapsed{
  margin-right:2px;
  border:none;
  border-radius:3px;
  background:#ced9e0;
  cursor:pointer;
  padding:1px 5px;
  vertical-align:text-bottom; }
  .bp3-breadcrumbs-collapsed::before{
    display:block;
    background:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cg fill='%235C7080'%3e%3ccircle cx='2' cy='8.03' r='2'/%3e%3ccircle cx='14' cy='8.03' r='2'/%3e%3ccircle cx='8' cy='8.03' r='2'/%3e%3c/g%3e%3c/svg%3e") center no-repeat;
    width:16px;
    height:16px;
    content:""; }
  .bp3-breadcrumbs-collapsed:hover{
    background:#bfccd6;
    text-decoration:none;
    color:#182026; }

.bp3-dark .bp3-breadcrumb,
.bp3-dark .bp3-breadcrumbs-collapsed{
  color:#a7b6c2; }

.bp3-dark .bp3-breadcrumbs > li::after{
  color:#a7b6c2; }

.bp3-dark .bp3-breadcrumb.bp3-disabled{
  color:rgba(167, 182, 194, 0.6); }

.bp3-dark .bp3-breadcrumb-current{
  color:#f5f8fa; }

.bp3-dark .bp3-breadcrumbs-collapsed{
  background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-breadcrumbs-collapsed:hover{
    background:rgba(16, 22, 26, 0.6);
    color:#f5f8fa; }
.bp3-button{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  border:none;
  border-radius:3px;
  cursor:pointer;
  padding:5px 10px;
  vertical-align:middle;
  text-align:left;
  font-size:14px;
  min-width:30px;
  min-height:30px; }
  .bp3-button > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-button > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-button::before,
  .bp3-button > *{
    margin-right:7px; }
  .bp3-button:empty::before,
  .bp3-button > :last-child{
    margin-right:0; }
  .bp3-button:empty{
    padding:0 !important; }
  .bp3-button:disabled, .bp3-button.bp3-disabled{
    cursor:not-allowed; }
  .bp3-button.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-button.bp3-align-right,
  .bp3-align-right .bp3-button{
    text-align:right; }
  .bp3-button.bp3-align-left,
  .bp3-align-left .bp3-button{
    text-align:left; }
  .bp3-button:not([class*="bp3-intent-"]){
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    color:#182026; }
    .bp3-button:not([class*="bp3-intent-"]):hover{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
      background-clip:padding-box;
      background-color:#ebf1f5; }
    .bp3-button:not([class*="bp3-intent-"]):active, .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#d8e1e8;
      background-image:none; }
    .bp3-button:not([class*="bp3-intent-"]):disabled, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled{
      outline:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      background-color:rgba(206, 217, 224, 0.5);
      background-image:none;
      cursor:not-allowed;
      color:rgba(92, 112, 128, 0.6); }
      .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active, .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active:hover, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active, .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active:hover{
        background:rgba(206, 217, 224, 0.7); }
  .bp3-button.bp3-intent-primary{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    color:#ffffff; }
    .bp3-button.bp3-intent-primary:hover, .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-primary:hover{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
      background-color:#106ba3; }
    .bp3-button.bp3-intent-primary:active, .bp3-button.bp3-intent-primary.bp3-active{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#0e5a8a;
      background-image:none; }
    .bp3-button.bp3-intent-primary:disabled, .bp3-button.bp3-intent-primary.bp3-disabled{
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      background-color:rgba(19, 124, 189, 0.5);
      background-image:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-success{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    background-color:#0f9960;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    color:#ffffff; }
    .bp3-button.bp3-intent-success:hover, .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-success:hover{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
      background-color:#0d8050; }
    .bp3-button.bp3-intent-success:active, .bp3-button.bp3-intent-success.bp3-active{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#0a6640;
      background-image:none; }
    .bp3-button.bp3-intent-success:disabled, .bp3-button.bp3-intent-success.bp3-disabled{
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      background-color:rgba(15, 153, 96, 0.5);
      background-image:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-warning{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    background-color:#d9822b;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    color:#ffffff; }
    .bp3-button.bp3-intent-warning:hover, .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-warning:hover{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
      background-color:#bf7326; }
    .bp3-button.bp3-intent-warning:active, .bp3-button.bp3-intent-warning.bp3-active{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#a66321;
      background-image:none; }
    .bp3-button.bp3-intent-warning:disabled, .bp3-button.bp3-intent-warning.bp3-disabled{
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      background-color:rgba(217, 130, 43, 0.5);
      background-image:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button.bp3-intent-danger{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    background-color:#db3737;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    color:#ffffff; }
    .bp3-button.bp3-intent-danger:hover, .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
      color:#ffffff; }
    .bp3-button.bp3-intent-danger:hover{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
      background-color:#c23030; }
    .bp3-button.bp3-intent-danger:active, .bp3-button.bp3-intent-danger.bp3-active{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#a82a2a;
      background-image:none; }
    .bp3-button.bp3-intent-danger:disabled, .bp3-button.bp3-intent-danger.bp3-disabled{
      border-color:transparent;
      -webkit-box-shadow:none;
              box-shadow:none;
      background-color:rgba(219, 55, 55, 0.5);
      background-image:none;
      color:rgba(255, 255, 255, 0.6); }
  .bp3-button[class*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
    stroke:#ffffff; }
  .bp3-button.bp3-large,
  .bp3-large .bp3-button{
    min-width:40px;
    min-height:40px;
    padding:5px 15px;
    font-size:16px; }
    .bp3-button.bp3-large::before,
    .bp3-button.bp3-large > *,
    .bp3-large .bp3-button::before,
    .bp3-large .bp3-button > *{
      margin-right:10px; }
    .bp3-button.bp3-large:empty::before,
    .bp3-button.bp3-large > :last-child,
    .bp3-large .bp3-button:empty::before,
    .bp3-large .bp3-button > :last-child{
      margin-right:0; }
  .bp3-button.bp3-small,
  .bp3-small .bp3-button{
    min-width:24px;
    min-height:24px;
    padding:0 7px; }
  .bp3-button.bp3-loading{
    position:relative; }
    .bp3-button.bp3-loading[class*="bp3-icon-"]::before{
      visibility:hidden; }
    .bp3-button.bp3-loading .bp3-button-spinner{
      position:absolute;
      margin:0; }
    .bp3-button.bp3-loading > :not(.bp3-button-spinner){
      visibility:hidden; }
  .bp3-button[class*="bp3-icon-"]::before{
    line-height:1;
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-weight:400;
    font-style:normal;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    color:#5c7080; }
  .bp3-button .bp3-icon, .bp3-button .bp3-icon-standard, .bp3-button .bp3-icon-large{
    color:#5c7080; }
    .bp3-button .bp3-icon.bp3-align-right, .bp3-button .bp3-icon-standard.bp3-align-right, .bp3-button .bp3-icon-large.bp3-align-right{
      margin-left:7px; }
  .bp3-button .bp3-icon:first-child:last-child,
  .bp3-button .bp3-spinner + .bp3-icon:last-child{
    margin:0 -7px; }
  .bp3-dark .bp3-button:not([class*="bp3-intent-"]){
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    background-color:#394b59;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
    color:#f5f8fa; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):hover, .bp3-dark .bp3-button:not([class*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      color:#f5f8fa; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):hover{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
      background-color:#30404d; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-active{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#202b33;
      background-image:none; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]):disabled, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none;
      background-color:rgba(57, 75, 89, 0.5);
      background-image:none;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-button:not([class*="bp3-intent-"]):disabled.bp3-active, .bp3-dark .bp3-button:not([class*="bp3-intent-"]).bp3-disabled.bp3-active{
        background:rgba(57, 75, 89, 0.7); }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-button-spinner .bp3-spinner-head{
      background:rgba(16, 22, 26, 0.5);
      stroke:#8a9ba8; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"])[class*="bp3-icon-"]::before{
      color:#a7b6c2; }
    .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon, .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-button:not([class*="bp3-intent-"]) .bp3-icon-large{
      color:#a7b6c2; }
  .bp3-dark .bp3-button[class*="bp3-intent-"]{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:hover{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:active, .bp3-dark .bp3-button[class*="bp3-intent-"].bp3-active{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2); }
    .bp3-dark .bp3-button[class*="bp3-intent-"]:disabled, .bp3-dark .bp3-button[class*="bp3-intent-"].bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none;
      background-image:none;
      color:rgba(255, 255, 255, 0.3); }
    .bp3-dark .bp3-button[class*="bp3-intent-"] .bp3-button-spinner .bp3-spinner-head{
      stroke:#8a9ba8; }
  .bp3-button:disabled::before,
  .bp3-button:disabled .bp3-icon, .bp3-button:disabled .bp3-icon-standard, .bp3-button:disabled .bp3-icon-large, .bp3-button.bp3-disabled::before,
  .bp3-button.bp3-disabled .bp3-icon, .bp3-button.bp3-disabled .bp3-icon-standard, .bp3-button.bp3-disabled .bp3-icon-large, .bp3-button[class*="bp3-intent-"]::before,
  .bp3-button[class*="bp3-intent-"] .bp3-icon, .bp3-button[class*="bp3-intent-"] .bp3-icon-standard, .bp3-button[class*="bp3-intent-"] .bp3-icon-large{
    color:inherit !important; }
  .bp3-button.bp3-minimal{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:none; }
    .bp3-button.bp3-minimal:hover{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(167, 182, 194, 0.3);
      text-decoration:none;
      color:#182026; }
    .bp3-button.bp3-minimal:active, .bp3-button.bp3-minimal.bp3-active{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(115, 134, 148, 0.3);
      color:#182026; }
    .bp3-button.bp3-minimal:disabled, .bp3-button.bp3-minimal:disabled:hover, .bp3-button.bp3-minimal.bp3-disabled, .bp3-button.bp3-minimal.bp3-disabled:hover{
      background:none;
      cursor:not-allowed;
      color:rgba(92, 112, 128, 0.6); }
      .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button.bp3-minimal{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:none;
      color:inherit; }
      .bp3-dark .bp3-button.bp3-minimal:hover, .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none; }
      .bp3-dark .bp3-button.bp3-minimal:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button.bp3-minimal:active, .bp3-dark .bp3-button.bp3-minimal.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button.bp3-minimal:disabled, .bp3-dark .bp3-button.bp3-minimal:disabled:hover, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover{
        background:none;
        cursor:not-allowed;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-button.bp3-minimal:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal:disabled:hover.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:hover, .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none;
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-success{
      color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:hover, .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none;
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:hover, .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none;
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button.bp3-minimal.bp3-intent-danger{
      color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:hover, .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none;
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button.bp3-minimal.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button.bp3-minimal.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }

a.bp3-button{
  text-align:center;
  text-decoration:none;
  -webkit-transition:none;
  transition:none; }
  a.bp3-button, a.bp3-button:hover, a.bp3-button:active{
    color:#182026; }
  a.bp3-button.bp3-disabled{
    color:rgba(92, 112, 128, 0.6); }

.bp3-button-text{
  -webkit-box-flex:0;
      -ms-flex:0 1 auto;
          flex:0 1 auto; }

.bp3-button.bp3-align-left .bp3-button-text, .bp3-button.bp3-align-right .bp3-button-text,
.bp3-button-group.bp3-align-left .bp3-button-text,
.bp3-button-group.bp3-align-right .bp3-button-text{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto; }
.bp3-button-group{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex; }
  .bp3-button-group .bp3-button{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    position:relative;
    z-index:4; }
    .bp3-button-group .bp3-button:focus{
      z-index:5; }
    .bp3-button-group .bp3-button:hover{
      z-index:6; }
    .bp3-button-group .bp3-button:active, .bp3-button-group .bp3-button.bp3-active{
      z-index:7; }
    .bp3-button-group .bp3-button:disabled, .bp3-button-group .bp3-button.bp3-disabled{
      z-index:3; }
    .bp3-button-group .bp3-button[class*="bp3-intent-"]{
      z-index:9; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:focus{
        z-index:10; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:hover{
        z-index:11; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:active, .bp3-button-group .bp3-button[class*="bp3-intent-"].bp3-active{
        z-index:12; }
      .bp3-button-group .bp3-button[class*="bp3-intent-"]:disabled, .bp3-button-group .bp3-button[class*="bp3-intent-"].bp3-disabled{
        z-index:8; }
  .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:first-child) .bp3-button,
  .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:first-child){
    border-top-left-radius:0;
    border-bottom-left-radius:0; }
  .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
    margin-right:-1px;
    border-top-right-radius:0;
    border-bottom-right-radius:0; }
  .bp3-button-group.bp3-minimal .bp3-button{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:none; }
    .bp3-button-group.bp3-minimal .bp3-button:hover{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(167, 182, 194, 0.3);
      text-decoration:none;
      color:#182026; }
    .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(115, 134, 148, 0.3);
      color:#182026; }
    .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
      background:none;
      cursor:not-allowed;
      color:rgba(92, 112, 128, 0.6); }
      .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
        background:rgba(115, 134, 148, 0.3); }
    .bp3-dark .bp3-button-group.bp3-minimal .bp3-button{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:none;
      color:inherit; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:hover{
        background:rgba(138, 155, 168, 0.15); }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-active{
        background:rgba(138, 155, 168, 0.3);
        color:#f5f8fa; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover{
        background:none;
        cursor:not-allowed;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button:disabled:hover.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-disabled:hover.bp3-active{
          background:rgba(138, 155, 168, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
      color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none;
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.15);
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#106ba3; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(16, 107, 163, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
        stroke:#106ba3; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary{
        color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:hover{
          background:rgba(19, 124, 189, 0.2);
          color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-active{
          background:rgba(19, 124, 189, 0.3);
          color:#48aff0; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled{
          background:none;
          color:rgba(72, 175, 240, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-primary.bp3-disabled.bp3-active{
            background:rgba(19, 124, 189, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
      color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none;
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.15);
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#0d8050; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(13, 128, 80, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
        stroke:#0d8050; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success{
        color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:hover{
          background:rgba(15, 153, 96, 0.2);
          color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-active{
          background:rgba(15, 153, 96, 0.3);
          color:#3dcc91; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled{
          background:none;
          color:rgba(61, 204, 145, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-success.bp3-disabled.bp3-active{
            background:rgba(15, 153, 96, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
      color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none;
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.15);
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#bf7326; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(191, 115, 38, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
        stroke:#bf7326; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning{
        color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:hover{
          background:rgba(217, 130, 43, 0.2);
          color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-active{
          background:rgba(217, 130, 43, 0.3);
          color:#ffb366; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled{
          background:none;
          color:rgba(255, 179, 102, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-warning.bp3-disabled.bp3-active{
            background:rgba(217, 130, 43, 0.3); }
    .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
      color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:none;
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.15);
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#c23030; }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(194, 48, 48, 0.5); }
        .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }
      .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
        stroke:#c23030; }
      .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger{
        color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:hover{
          background:rgba(219, 55, 55, 0.2);
          color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-active{
          background:rgba(219, 55, 55, 0.3);
          color:#ff7373; }
        .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled{
          background:none;
          color:rgba(255, 115, 115, 0.5); }
          .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-button-group.bp3-minimal .bp3-button.bp3-intent-danger.bp3-disabled.bp3-active{
            background:rgba(219, 55, 55, 0.3); }
  .bp3-button-group .bp3-popover-wrapper,
  .bp3-button-group .bp3-popover-target{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-button-group.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-button-group .bp3-button.bp3-fill,
  .bp3-button-group.bp3-fill .bp3-button:not(.bp3-fixed){
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-button-group.bp3-vertical{
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column;
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch;
    vertical-align:top; }
    .bp3-button-group.bp3-vertical.bp3-fill{
      width:unset;
      height:100%; }
    .bp3-button-group.bp3-vertical .bp3-button{
      margin-right:0 !important;
      width:100%; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:first-child .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:first-child{
      border-radius:3px 3px 0 0; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:last-child .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:last-child{
      border-radius:0 0 3px 3px; }
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
    .bp3-button-group.bp3-vertical:not(.bp3-minimal) > .bp3-button:not(:last-child){
      margin-bottom:-1px; }
  .bp3-button-group.bp3-align-left .bp3-button{
    text-align:left; }
  .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-dark .bp3-button-group:not(.bp3-minimal) > .bp3-button:not(:last-child){
    margin-right:1px; }
  .bp3-dark .bp3-button-group.bp3-vertical > .bp3-popover-wrapper:not(:last-child) .bp3-button,
  .bp3-dark .bp3-button-group.bp3-vertical > .bp3-button:not(:last-child){
    margin-bottom:1px; }
.bp3-callout{
  line-height:1.5;
  font-size:14px;
  position:relative;
  border-radius:3px;
  background-color:rgba(138, 155, 168, 0.15);
  width:100%;
  padding:10px 12px 9px; }
  .bp3-callout[class*="bp3-icon-"]{
    padding-left:40px; }
    .bp3-callout[class*="bp3-icon-"]::before{
      line-height:1;
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-weight:400;
      font-style:normal;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased;
      position:absolute;
      top:10px;
      left:10px;
      color:#5c7080; }
  .bp3-callout.bp3-callout-icon{
    padding-left:40px; }
    .bp3-callout.bp3-callout-icon > .bp3-icon:first-child{
      position:absolute;
      top:10px;
      left:10px;
      color:#5c7080; }
  .bp3-callout .bp3-heading{
    margin-top:0;
    margin-bottom:5px;
    line-height:20px; }
    .bp3-callout .bp3-heading:last-child{
      margin-bottom:0; }
  .bp3-dark .bp3-callout{
    background-color:rgba(138, 155, 168, 0.2); }
    .bp3-dark .bp3-callout[class*="bp3-icon-"]::before{
      color:#a7b6c2; }
  .bp3-callout.bp3-intent-primary{
    background-color:rgba(19, 124, 189, 0.15); }
    .bp3-callout.bp3-intent-primary[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-primary .bp3-heading{
      color:#106ba3; }
    .bp3-dark .bp3-callout.bp3-intent-primary{
      background-color:rgba(19, 124, 189, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-primary[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-primary > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-primary .bp3-heading{
        color:#48aff0; }
  .bp3-callout.bp3-intent-success{
    background-color:rgba(15, 153, 96, 0.15); }
    .bp3-callout.bp3-intent-success[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-success .bp3-heading{
      color:#0d8050; }
    .bp3-dark .bp3-callout.bp3-intent-success{
      background-color:rgba(15, 153, 96, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-success[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-success > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-success .bp3-heading{
        color:#3dcc91; }
  .bp3-callout.bp3-intent-warning{
    background-color:rgba(217, 130, 43, 0.15); }
    .bp3-callout.bp3-intent-warning[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-warning .bp3-heading{
      color:#bf7326; }
    .bp3-dark .bp3-callout.bp3-intent-warning{
      background-color:rgba(217, 130, 43, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-warning[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-warning > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-warning .bp3-heading{
        color:#ffb366; }
  .bp3-callout.bp3-intent-danger{
    background-color:rgba(219, 55, 55, 0.15); }
    .bp3-callout.bp3-intent-danger[class*="bp3-icon-"]::before,
    .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
    .bp3-callout.bp3-intent-danger .bp3-heading{
      color:#c23030; }
    .bp3-dark .bp3-callout.bp3-intent-danger{
      background-color:rgba(219, 55, 55, 0.25); }
      .bp3-dark .bp3-callout.bp3-intent-danger[class*="bp3-icon-"]::before,
      .bp3-dark .bp3-callout.bp3-intent-danger > .bp3-icon:first-child,
      .bp3-dark .bp3-callout.bp3-intent-danger .bp3-heading{
        color:#ff7373; }
  .bp3-running-text .bp3-callout{
    margin:20px 0; }
.bp3-card{
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
  background-color:#ffffff;
  padding:20px;
  -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-card.bp3-dark,
  .bp3-dark .bp3-card{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
    background-color:#30404d; }

.bp3-elevation-0{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.15), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }
  .bp3-elevation-0.bp3-dark,
  .bp3-dark .bp3-elevation-0{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), 0 0 0 rgba(16, 22, 26, 0), 0 0 0 rgba(16, 22, 26, 0); }

.bp3-elevation-1{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-1.bp3-dark,
  .bp3-dark .bp3-elevation-1{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-elevation-2{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 1px 1px rgba(16, 22, 26, 0.2), 0 2px 6px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-2.bp3-dark,
  .bp3-dark .bp3-elevation-2{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.4), 0 2px 6px rgba(16, 22, 26, 0.4); }

.bp3-elevation-3{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-3.bp3-dark,
  .bp3-dark .bp3-elevation-3{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-elevation-4{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2); }
  .bp3-elevation-4.bp3-dark,
  .bp3-dark .bp3-elevation-4{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:hover{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  cursor:pointer; }
  .bp3-card.bp3-interactive:hover.bp3-dark,
  .bp3-dark .bp3-card.bp3-interactive:hover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }

.bp3-card.bp3-interactive:active{
  opacity:0.9;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  -webkit-transition-duration:0;
          transition-duration:0; }
  .bp3-card.bp3-interactive:active.bp3-dark,
  .bp3-dark .bp3-card.bp3-interactive:active{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-collapse{
  height:0;
  overflow-y:hidden;
  -webkit-transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:height 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-collapse .bp3-collapse-body{
    -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-collapse .bp3-collapse-body[aria-hidden="true"]{
      display:none; }

.bp3-context-menu .bp3-popover-target{
  display:block; }

.bp3-context-menu-popover-target{
  position:fixed; }

.bp3-divider{
  margin:5px;
  border-right:1px solid rgba(16, 22, 26, 0.15);
  border-bottom:1px solid rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-divider{
    border-color:rgba(16, 22, 26, 0.4); }
.bp3-dialog-container{
  opacity:1;
  -webkit-transform:scale(1);
          transform:scale(1);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  width:100%;
  min-height:100%;
  pointer-events:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-dialog-container.bp3-overlay-enter > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear > .bp3-dialog{
    opacity:0;
    -webkit-transform:scale(0.5);
            transform:scale(0.5); }
  .bp3-dialog-container.bp3-overlay-enter-active > .bp3-dialog, .bp3-dialog-container.bp3-overlay-appear-active > .bp3-dialog{
    opacity:1;
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-property:opacity, -webkit-transform;
    transition-property:opacity, -webkit-transform;
    transition-property:opacity, transform;
    transition-property:opacity, transform, -webkit-transform;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-dialog-container.bp3-overlay-exit > .bp3-dialog{
    opacity:1;
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-dialog-container.bp3-overlay-exit-active > .bp3-dialog{
    opacity:0;
    -webkit-transform:scale(0.5);
            transform:scale(0.5);
    -webkit-transition-property:opacity, -webkit-transform;
    transition-property:opacity, -webkit-transform;
    transition-property:opacity, transform;
    transition-property:opacity, transform, -webkit-transform;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
    -webkit-transition-delay:0;
            transition-delay:0; }

.bp3-dialog{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:30px 0;
  border-radius:6px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  background:#ebf1f5;
  width:500px;
  padding-bottom:20px;
  pointer-events:all;
  -webkit-user-select:text;
     -moz-user-select:text;
      -ms-user-select:text;
          user-select:text; }
  .bp3-dialog:focus{
    outline:0; }
  .bp3-dialog.bp3-dark,
  .bp3-dark .bp3-dialog{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    background:#293742;
    color:#f5f8fa; }

.bp3-dialog-header{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  border-radius:6px 6px 0 0;
  -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
  background:#ffffff;
  min-height:40px;
  padding-right:5px;
  padding-left:20px; }
  .bp3-dialog-header .bp3-icon-large,
  .bp3-dialog-header .bp3-icon{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    margin-right:10px;
    color:#5c7080; }
  .bp3-dialog-header .bp3-heading{
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    margin:0;
    line-height:inherit; }
    .bp3-dialog-header .bp3-heading:last-child{
      margin-right:20px; }
  .bp3-dark .bp3-dialog-header{
    -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
    background:#30404d; }
    .bp3-dark .bp3-dialog-header .bp3-icon-large,
    .bp3-dark .bp3-dialog-header .bp3-icon{
      color:#a7b6c2; }

.bp3-dialog-body{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  margin:20px;
  line-height:18px; }

.bp3-dialog-footer{
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  margin:0 20px; }

.bp3-dialog-footer-actions{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-pack:end;
      -ms-flex-pack:end;
          justify-content:flex-end; }
  .bp3-dialog-footer-actions .bp3-button{
    margin-left:10px; }
.bp3-drawer{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:0;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  background:#ffffff;
  padding:0; }
  .bp3-drawer:focus{
    outline:0; }
  .bp3-drawer.bp3-position-top{
    top:0;
    right:0;
    left:0;
    height:50%; }
    .bp3-drawer.bp3-position-top.bp3-overlay-enter, .bp3-drawer.bp3-position-top.bp3-overlay-appear{
      -webkit-transform:translateY(-100%);
              transform:translateY(-100%); }
    .bp3-drawer.bp3-position-top.bp3-overlay-enter-active, .bp3-drawer.bp3-position-top.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
    .bp3-drawer.bp3-position-top.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer.bp3-position-top.bp3-overlay-exit-active{
      -webkit-transform:translateY(-100%);
              transform:translateY(-100%);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
  .bp3-drawer.bp3-position-bottom{
    right:0;
    bottom:0;
    left:0;
    height:50%; }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-enter, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear{
      -webkit-transform:translateY(100%);
              transform:translateY(100%); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-enter-active, .bp3-drawer.bp3-position-bottom.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer.bp3-position-bottom.bp3-overlay-exit-active{
      -webkit-transform:translateY(100%);
              transform:translateY(100%);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
  .bp3-drawer.bp3-position-left{
    top:0;
    bottom:0;
    left:0;
    width:50%; }
    .bp3-drawer.bp3-position-left.bp3-overlay-enter, .bp3-drawer.bp3-position-left.bp3-overlay-appear{
      -webkit-transform:translateX(-100%);
              transform:translateX(-100%); }
    .bp3-drawer.bp3-position-left.bp3-overlay-enter-active, .bp3-drawer.bp3-position-left.bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
    .bp3-drawer.bp3-position-left.bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer.bp3-position-left.bp3-overlay-exit-active{
      -webkit-transform:translateX(-100%);
              transform:translateX(-100%);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
  .bp3-drawer.bp3-position-right{
    top:0;
    right:0;
    bottom:0;
    width:50%; }
    .bp3-drawer.bp3-position-right.bp3-overlay-enter, .bp3-drawer.bp3-position-right.bp3-overlay-appear{
      -webkit-transform:translateX(100%);
              transform:translateX(100%); }
    .bp3-drawer.bp3-position-right.bp3-overlay-enter-active, .bp3-drawer.bp3-position-right.bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
    .bp3-drawer.bp3-position-right.bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer.bp3-position-right.bp3-overlay-exit-active{
      -webkit-transform:translateX(100%);
              transform:translateX(100%);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
  .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
  .bp3-position-right):not(.bp3-vertical){
    top:0;
    right:0;
    bottom:0;
    width:50%; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear{
      -webkit-transform:translateX(100%);
              transform:translateX(100%); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-appear-active{
      -webkit-transform:translateX(0);
              transform:translateX(0);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit{
      -webkit-transform:translateX(0);
              transform:translateX(0); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right):not(.bp3-vertical).bp3-overlay-exit-active{
      -webkit-transform:translateX(100%);
              transform:translateX(100%);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
  .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
  .bp3-position-right).bp3-vertical{
    right:0;
    bottom:0;
    left:0;
    height:50%; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-enter, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-appear{
      -webkit-transform:translateY(100%);
              transform:translateY(100%); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-enter-active, .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-appear-active{
      -webkit-transform:translateY(0);
              transform:translateY(0);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:200ms;
              transition-duration:200ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-exit{
      -webkit-transform:translateY(0);
              transform:translateY(0); }
    .bp3-drawer:not(.bp3-position-top):not(.bp3-position-bottom):not(.bp3-position-left):not(
    .bp3-position-right).bp3-vertical.bp3-overlay-exit-active{
      -webkit-transform:translateY(100%);
              transform:translateY(100%);
      -webkit-transition-property:-webkit-transform;
      transition-property:-webkit-transform;
      transition-property:transform;
      transition-property:transform, -webkit-transform;
      -webkit-transition-duration:100ms;
              transition-duration:100ms;
      -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
              transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
      -webkit-transition-delay:0;
              transition-delay:0; }
  .bp3-drawer.bp3-dark,
  .bp3-dark .bp3-drawer{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    background:#30404d;
    color:#f5f8fa; }

.bp3-drawer-header{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  position:relative;
  border-radius:0;
  -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:0 1px 0 rgba(16, 22, 26, 0.15);
  min-height:40px;
  padding:5px;
  padding-left:20px; }
  .bp3-drawer-header .bp3-icon-large,
  .bp3-drawer-header .bp3-icon{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    margin-right:10px;
    color:#5c7080; }
  .bp3-drawer-header .bp3-heading{
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    margin:0;
    line-height:inherit; }
    .bp3-drawer-header .bp3-heading:last-child{
      margin-right:20px; }
  .bp3-dark .bp3-drawer-header{
    -webkit-box-shadow:0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:0 1px 0 rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-drawer-header .bp3-icon-large,
    .bp3-dark .bp3-drawer-header .bp3-icon{
      color:#a7b6c2; }

.bp3-drawer-body{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  overflow:auto;
  line-height:18px; }

.bp3-drawer-footer{
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  position:relative;
  -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
  padding:10px 20px; }
  .bp3-dark .bp3-drawer-footer{
    -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.4); }
.bp3-editable-text{
  display:inline-block;
  position:relative;
  cursor:text;
  max-width:100%;
  vertical-align:top;
  white-space:nowrap; }
  .bp3-editable-text::before{
    position:absolute;
    top:-3px;
    right:-3px;
    bottom:-3px;
    left:-3px;
    border-radius:3px;
    content:"";
    -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9), box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-editable-text:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-editable-text.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
    background-color:#ffffff; }
  .bp3-editable-text.bp3-disabled::before{
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-editable-text.bp3-intent-primary .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
    color:#137cbd; }
  .bp3-editable-text.bp3-intent-primary:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(19, 124, 189, 0.4); }
  .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-success .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
    color:#0f9960; }
  .bp3-editable-text.bp3-intent-success:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px rgba(15, 153, 96, 0.4); }
  .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-warning .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
    color:#d9822b; }
  .bp3-editable-text.bp3-intent-warning:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px rgba(217, 130, 43, 0.4); }
  .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-editable-text.bp3-intent-danger .bp3-editable-text-input,
  .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
    color:#db3737; }
  .bp3-editable-text.bp3-intent-danger:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px rgba(219, 55, 55, 0.4); }
  .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-editable-text:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(255, 255, 255, 0.15); }
  .bp3-dark .bp3-editable-text.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    background-color:rgba(16, 22, 26, 0.3); }
  .bp3-dark .bp3-editable-text.bp3-disabled::before{
    -webkit-box-shadow:none;
            box-shadow:none; }
  .bp3-dark .bp3-editable-text.bp3-intent-primary .bp3-editable-text-content{
    color:#48aff0; }
  .bp3-dark .bp3-editable-text.bp3-intent-primary:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4);
            box-shadow:0 0 0 0 rgba(72, 175, 240, 0), 0 0 0 0 rgba(72, 175, 240, 0), inset 0 0 0 1px rgba(72, 175, 240, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-primary.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #48aff0, 0 0 0 3px rgba(72, 175, 240, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-success .bp3-editable-text-content{
    color:#3dcc91; }
  .bp3-dark .bp3-editable-text.bp3-intent-success:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4);
            box-shadow:0 0 0 0 rgba(61, 204, 145, 0), 0 0 0 0 rgba(61, 204, 145, 0), inset 0 0 0 1px rgba(61, 204, 145, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-success.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #3dcc91, 0 0 0 3px rgba(61, 204, 145, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-warning .bp3-editable-text-content{
    color:#ffb366; }
  .bp3-dark .bp3-editable-text.bp3-intent-warning:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4);
            box-shadow:0 0 0 0 rgba(255, 179, 102, 0), 0 0 0 0 rgba(255, 179, 102, 0), inset 0 0 0 1px rgba(255, 179, 102, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-warning.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #ffb366, 0 0 0 3px rgba(255, 179, 102, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-danger .bp3-editable-text-content{
    color:#ff7373; }
  .bp3-dark .bp3-editable-text.bp3-intent-danger:hover::before{
    -webkit-box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4);
            box-shadow:0 0 0 0 rgba(255, 115, 115, 0), 0 0 0 0 rgba(255, 115, 115, 0), inset 0 0 0 1px rgba(255, 115, 115, 0.4); }
  .bp3-dark .bp3-editable-text.bp3-intent-danger.bp3-editable-text-editing::before{
    -webkit-box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #ff7373, 0 0 0 3px rgba(255, 115, 115, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-editable-text-input,
.bp3-editable-text-content{
  display:inherit;
  position:relative;
  min-width:inherit;
  max-width:inherit;
  vertical-align:top;
  text-transform:inherit;
  letter-spacing:inherit;
  color:inherit;
  font:inherit;
  resize:none; }

.bp3-editable-text-input{
  border:none;
  -webkit-box-shadow:none;
          box-shadow:none;
  background:none;
  width:100%;
  padding:0;
  white-space:pre-wrap; }
  .bp3-editable-text-input::-webkit-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-editable-text-input::-moz-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-editable-text-input:-ms-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-editable-text-input::-ms-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-editable-text-input::placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-editable-text-input:focus{
    outline:none; }
  .bp3-editable-text-input::-ms-clear{
    display:none; }

.bp3-editable-text-content{
  overflow:hidden;
  padding-right:2px;
  text-overflow:ellipsis;
  white-space:pre; }
  .bp3-editable-text-editing > .bp3-editable-text-content{
    position:absolute;
    left:0;
    visibility:hidden; }
  .bp3-editable-text-placeholder > .bp3-editable-text-content{
    color:rgba(92, 112, 128, 0.6); }
    .bp3-dark .bp3-editable-text-placeholder > .bp3-editable-text-content{
      color:rgba(167, 182, 194, 0.6); }

.bp3-editable-text.bp3-multiline{
  display:block; }
  .bp3-editable-text.bp3-multiline .bp3-editable-text-content{
    overflow:auto;
    white-space:pre-wrap;
    word-wrap:break-word; }
.bp3-control-group{
  -webkit-transform:translateZ(0);
          transform:translateZ(0);
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:stretch;
      -ms-flex-align:stretch;
          align-items:stretch; }
  .bp3-control-group > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-control-group > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-control-group .bp3-button,
  .bp3-control-group .bp3-html-select,
  .bp3-control-group .bp3-input,
  .bp3-control-group .bp3-select{
    position:relative; }
  .bp3-control-group .bp3-input{
    z-index:2;
    border-radius:inherit; }
    .bp3-control-group .bp3-input:focus{
      z-index:14;
      border-radius:3px; }
    .bp3-control-group .bp3-input[class*="bp3-intent"]{
      z-index:13; }
      .bp3-control-group .bp3-input[class*="bp3-intent"]:focus{
        z-index:15; }
    .bp3-control-group .bp3-input[readonly], .bp3-control-group .bp3-input:disabled, .bp3-control-group .bp3-input.bp3-disabled{
      z-index:1; }
  .bp3-control-group .bp3-input-group[class*="bp3-intent"] .bp3-input{
    z-index:13; }
    .bp3-control-group .bp3-input-group[class*="bp3-intent"] .bp3-input:focus{
      z-index:15; }
  .bp3-control-group .bp3-button,
  .bp3-control-group .bp3-html-select select,
  .bp3-control-group .bp3-select select{
    -webkit-transform:translateZ(0);
            transform:translateZ(0);
    z-index:4;
    border-radius:inherit; }
    .bp3-control-group .bp3-button:focus,
    .bp3-control-group .bp3-html-select select:focus,
    .bp3-control-group .bp3-select select:focus{
      z-index:5; }
    .bp3-control-group .bp3-button:hover,
    .bp3-control-group .bp3-html-select select:hover,
    .bp3-control-group .bp3-select select:hover{
      z-index:6; }
    .bp3-control-group .bp3-button:active,
    .bp3-control-group .bp3-html-select select:active,
    .bp3-control-group .bp3-select select:active{
      z-index:7; }
    .bp3-control-group .bp3-button[readonly], .bp3-control-group .bp3-button:disabled, .bp3-control-group .bp3-button.bp3-disabled,
    .bp3-control-group .bp3-html-select select[readonly],
    .bp3-control-group .bp3-html-select select:disabled,
    .bp3-control-group .bp3-html-select select.bp3-disabled,
    .bp3-control-group .bp3-select select[readonly],
    .bp3-control-group .bp3-select select:disabled,
    .bp3-control-group .bp3-select select.bp3-disabled{
      z-index:3; }
    .bp3-control-group .bp3-button[class*="bp3-intent"],
    .bp3-control-group .bp3-html-select select[class*="bp3-intent"],
    .bp3-control-group .bp3-select select[class*="bp3-intent"]{
      z-index:9; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:focus,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:focus,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:focus{
        z-index:10; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:hover,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:hover,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:hover{
        z-index:11; }
      .bp3-control-group .bp3-button[class*="bp3-intent"]:active,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:active,
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:active{
        z-index:12; }
      .bp3-control-group .bp3-button[class*="bp3-intent"][readonly], .bp3-control-group .bp3-button[class*="bp3-intent"]:disabled, .bp3-control-group .bp3-button[class*="bp3-intent"].bp3-disabled,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"][readonly],
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"]:disabled,
      .bp3-control-group .bp3-html-select select[class*="bp3-intent"].bp3-disabled,
      .bp3-control-group .bp3-select select[class*="bp3-intent"][readonly],
      .bp3-control-group .bp3-select select[class*="bp3-intent"]:disabled,
      .bp3-control-group .bp3-select select[class*="bp3-intent"].bp3-disabled{
        z-index:8; }
  .bp3-control-group .bp3-input-group > .bp3-icon,
  .bp3-control-group .bp3-input-group > .bp3-button,
  .bp3-control-group .bp3-input-group > .bp3-input-action{
    z-index:16; }
  .bp3-control-group .bp3-select::after,
  .bp3-control-group .bp3-html-select::after,
  .bp3-control-group .bp3-select > .bp3-icon,
  .bp3-control-group .bp3-html-select > .bp3-icon{
    z-index:17; }
  .bp3-control-group:not(.bp3-vertical) > *{
    margin-right:-1px; }
  .bp3-dark .bp3-control-group:not(.bp3-vertical) > *{
    margin-right:0; }
  .bp3-dark .bp3-control-group:not(.bp3-vertical) > .bp3-button + .bp3-button{
    margin-left:1px; }
  .bp3-control-group .bp3-popover-wrapper,
  .bp3-control-group .bp3-popover-target{
    border-radius:inherit; }
  .bp3-control-group > :first-child{
    border-radius:3px 0 0 3px; }
  .bp3-control-group > :last-child{
    margin-right:0;
    border-radius:0 3px 3px 0; }
  .bp3-control-group > :only-child{
    margin-right:0;
    border-radius:3px; }
  .bp3-control-group .bp3-input-group .bp3-button{
    border-radius:3px; }
  .bp3-control-group > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-control-group.bp3-fill > *:not(.bp3-fixed){
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto; }
  .bp3-control-group.bp3-vertical{
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column; }
    .bp3-control-group.bp3-vertical > *{
      margin-top:-1px; }
    .bp3-control-group.bp3-vertical > :first-child{
      margin-top:0;
      border-radius:3px 3px 0 0; }
    .bp3-control-group.bp3-vertical > :last-child{
      border-radius:0 0 3px 3px; }
.bp3-control{
  display:block;
  position:relative;
  margin-bottom:10px;
  cursor:pointer;
  text-transform:none; }
  .bp3-control input:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    color:#ffffff; }
  .bp3-control:hover input:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    background-color:#106ba3; }
  .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background:#0e5a8a; }
  .bp3-control input:disabled:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(19, 124, 189, 0.5); }
  .bp3-dark .bp3-control input:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control:hover input:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    background-color:#106ba3; }
  .bp3-dark .bp3-control input:not(:disabled):active:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background-color:#0e5a8a; }
  .bp3-dark .bp3-control input:disabled:checked ~ .bp3-control-indicator{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(14, 90, 138, 0.5); }
  .bp3-control:not(.bp3-align-right){
    padding-left:26px; }
    .bp3-control:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-26px; }
  .bp3-control.bp3-align-right{
    padding-right:26px; }
    .bp3-control.bp3-align-right .bp3-control-indicator{
      margin-right:-26px; }
  .bp3-control.bp3-disabled{
    cursor:not-allowed;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-control.bp3-inline{
    display:inline-block;
    margin-right:20px; }
  .bp3-control input{
    position:absolute;
    top:0;
    left:0;
    opacity:0;
    z-index:-1; }
  .bp3-control .bp3-control-indicator{
    display:inline-block;
    position:relative;
    margin-top:-3px;
    margin-right:10px;
    border:none;
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    background-clip:padding-box;
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    cursor:pointer;
    width:1em;
    height:1em;
    vertical-align:middle;
    font-size:16px;
    -webkit-user-select:none;
       -moz-user-select:none;
        -ms-user-select:none;
            user-select:none; }
    .bp3-control .bp3-control-indicator::before{
      display:block;
      width:1em;
      height:1em;
      content:""; }
  .bp3-control:hover .bp3-control-indicator{
    background-color:#ebf1f5; }
  .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background:#d8e1e8; }
  .bp3-control input:disabled ~ .bp3-control-indicator{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(206, 217, 224, 0.5);
    cursor:not-allowed; }
  .bp3-control input:focus ~ .bp3-control-indicator{
    outline:rgba(19, 124, 189, 0.6) auto 2px;
    outline-offset:2px;
    -moz-outline-radius:6px; }
  .bp3-control.bp3-align-right .bp3-control-indicator{
    float:right;
    margin-top:1px;
    margin-left:10px; }
  .bp3-control.bp3-large{
    font-size:16px; }
    .bp3-control.bp3-large:not(.bp3-align-right){
      padding-left:30px; }
      .bp3-control.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
        margin-left:-30px; }
    .bp3-control.bp3-large.bp3-align-right{
      padding-right:30px; }
      .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
        margin-right:-30px; }
    .bp3-control.bp3-large .bp3-control-indicator{
      font-size:20px; }
    .bp3-control.bp3-large.bp3-align-right .bp3-control-indicator{
      margin-top:0; }
  .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    background-color:#137cbd;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.1)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.1), rgba(255, 255, 255, 0));
    color:#ffffff; }
  .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 -1px 0 rgba(16, 22, 26, 0.2);
    background-color:#106ba3; }
  .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background:#0e5a8a; }
  .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(19, 124, 189, 0.5); }
  .bp3-dark .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-checkbox:hover input:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    background-color:#106ba3; }
  .bp3-dark .bp3-control.bp3-checkbox input:not(:disabled):active:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background-color:#0e5a8a; }
  .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(14, 90, 138, 0.5); }
  .bp3-control.bp3-checkbox .bp3-control-indicator{
    border-radius:3px; }
  .bp3-control.bp3-checkbox input:checked ~ .bp3-control-indicator::before{
    background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M12 5c-.28 0-.53.11-.71.29L7 9.59l-2.29-2.3a1.003 1.003 0 0 0-1.42 1.42l3 3c.18.18.43.29.71.29s.53-.11.71-.29l5-5A1.003 1.003 0 0 0 12 5z' fill='white'/%3e%3c/svg%3e"); }
  .bp3-control.bp3-checkbox input:indeterminate ~ .bp3-control-indicator::before{
    background-image:url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 16 16'%3e%3cpath fill-rule='evenodd' clip-rule='evenodd' d='M11 7H5c-.55 0-1 .45-1 1s.45 1 1 1h6c.55 0 1-.45 1-1s-.45-1-1-1z' fill='white'/%3e%3c/svg%3e"); }
  .bp3-control.bp3-radio .bp3-control-indicator{
    border-radius:50%; }
  .bp3-control.bp3-radio input:checked ~ .bp3-control-indicator::before{
    background-image:radial-gradient(#ffffff, #ffffff 28%, transparent 32%); }
  .bp3-control.bp3-radio input:checked:disabled ~ .bp3-control-indicator::before{
    opacity:0.5; }
  .bp3-control.bp3-radio input:focus ~ .bp3-control-indicator{
    -moz-outline-radius:16px; }
  .bp3-control.bp3-switch input ~ .bp3-control-indicator{
    background:rgba(167, 182, 194, 0.5); }
  .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
    background:rgba(115, 134, 148, 0.5); }
  .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
    background:rgba(92, 112, 128, 0.5); }
  .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
    background:rgba(206, 217, 224, 0.5); }
    .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
      background:rgba(255, 255, 255, 0.8); }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
    background:#137cbd; }
  .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
    background:#106ba3; }
  .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
    background:#0e5a8a; }
  .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
    background:rgba(19, 124, 189, 0.5); }
    .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
      background:rgba(255, 255, 255, 0.8); }
  .bp3-control.bp3-switch:not(.bp3-align-right){
    padding-left:38px; }
    .bp3-control.bp3-switch:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-38px; }
  .bp3-control.bp3-switch.bp3-align-right{
    padding-right:38px; }
    .bp3-control.bp3-switch.bp3-align-right .bp3-control-indicator{
      margin-right:-38px; }
  .bp3-control.bp3-switch .bp3-control-indicator{
    border:none;
    border-radius:1.75em;
    -webkit-box-shadow:none !important;
            box-shadow:none !important;
    width:auto;
    min-width:1.75em;
    -webkit-transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:background-color 100ms cubic-bezier(0.4, 1, 0.75, 0.9); }
    .bp3-control.bp3-switch .bp3-control-indicator::before{
      position:absolute;
      left:0;
      margin:2px;
      border-radius:50%;
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
      background:#ffffff;
      width:calc(1em - 4px);
      height:calc(1em - 4px);
      -webkit-transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
      transition:left 100ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
    left:calc(100% - 1em); }
  .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right){
    padding-left:45px; }
    .bp3-control.bp3-switch.bp3-large:not(.bp3-align-right) .bp3-control-indicator{
      margin-left:-45px; }
  .bp3-control.bp3-switch.bp3-large.bp3-align-right{
    padding-right:45px; }
    .bp3-control.bp3-switch.bp3-large.bp3-align-right .bp3-control-indicator{
      margin-right:-45px; }
  .bp3-dark .bp3-control.bp3-switch input ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.5); }
  .bp3-dark .bp3-control.bp3-switch:hover input ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.7); }
  .bp3-dark .bp3-control.bp3-switch input:not(:disabled):active ~ .bp3-control-indicator{
    background:rgba(16, 22, 26, 0.9); }
  .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator{
    background:rgba(57, 75, 89, 0.5); }
    .bp3-dark .bp3-control.bp3-switch input:disabled ~ .bp3-control-indicator::before{
      background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator{
    background:#137cbd; }
  .bp3-dark .bp3-control.bp3-switch:hover input:checked ~ .bp3-control-indicator{
    background:#106ba3; }
  .bp3-dark .bp3-control.bp3-switch input:checked:not(:disabled):active ~ .bp3-control-indicator{
    background:#0e5a8a; }
  .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator{
    background:rgba(14, 90, 138, 0.5); }
    .bp3-dark .bp3-control.bp3-switch input:checked:disabled ~ .bp3-control-indicator::before{
      background:rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-control.bp3-switch .bp3-control-indicator::before{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    background:#394b59; }
  .bp3-dark .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator::before{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
  .bp3-control.bp3-switch .bp3-switch-inner-text{
    text-align:center;
    font-size:0.7em; }
  .bp3-control.bp3-switch .bp3-control-indicator-child:first-child{
    visibility:hidden;
    margin-right:1.2em;
    margin-left:0.5em;
    line-height:0; }
  .bp3-control.bp3-switch .bp3-control-indicator-child:last-child{
    visibility:visible;
    margin-right:0.5em;
    margin-left:1.2em;
    line-height:1em; }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:first-child{
    visibility:visible;
    line-height:1em; }
  .bp3-control.bp3-switch input:checked ~ .bp3-control-indicator .bp3-control-indicator-child:last-child{
    visibility:hidden;
    line-height:0; }
  .bp3-dark .bp3-control{
    color:#f5f8fa; }
    .bp3-dark .bp3-control.bp3-disabled{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-control .bp3-control-indicator{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
      background-color:#394b59;
      background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
      background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0)); }
    .bp3-dark .bp3-control:hover .bp3-control-indicator{
      background-color:#30404d; }
    .bp3-dark .bp3-control input:not(:disabled):active ~ .bp3-control-indicator{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background:#202b33; }
    .bp3-dark .bp3-control input:disabled ~ .bp3-control-indicator{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(57, 75, 89, 0.5);
      cursor:not-allowed; }
    .bp3-dark .bp3-control.bp3-checkbox input:disabled:checked ~ .bp3-control-indicator, .bp3-dark .bp3-control.bp3-checkbox input:disabled:indeterminate ~ .bp3-control-indicator{
      color:rgba(167, 182, 194, 0.6); }
.bp3-file-input{
  display:inline-block;
  position:relative;
  cursor:pointer;
  height:30px; }
  .bp3-file-input input{
    opacity:0;
    margin:0;
    min-width:200px; }
    .bp3-file-input input:disabled + .bp3-file-upload-input,
    .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(206, 217, 224, 0.5);
      cursor:not-allowed;
      color:rgba(92, 112, 128, 0.6);
      resize:none; }
      .bp3-file-input input:disabled + .bp3-file-upload-input::after,
      .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
        outline:none;
        -webkit-box-shadow:none;
                box-shadow:none;
        background-color:rgba(206, 217, 224, 0.5);
        background-image:none;
        cursor:not-allowed;
        color:rgba(92, 112, 128, 0.6); }
        .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active:hover,
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active,
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active:hover{
          background:rgba(206, 217, 224, 0.7); }
      .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input, .bp3-dark
      .bp3-file-input input.bp3-disabled + .bp3-file-upload-input{
        -webkit-box-shadow:none;
                box-shadow:none;
        background:rgba(57, 75, 89, 0.5);
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after, .bp3-dark
        .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after{
          -webkit-box-shadow:none;
                  box-shadow:none;
          background-color:rgba(57, 75, 89, 0.5);
          background-image:none;
          color:rgba(167, 182, 194, 0.6); }
          .bp3-dark .bp3-file-input input:disabled + .bp3-file-upload-input::after.bp3-active, .bp3-dark
          .bp3-file-input input.bp3-disabled + .bp3-file-upload-input::after.bp3-active{
            background:rgba(57, 75, 89, 0.7); }
  .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
    color:#182026; }
  .bp3-dark .bp3-file-input.bp3-file-input-has-selection .bp3-file-upload-input{
    color:#f5f8fa; }
  .bp3-file-input.bp3-fill{
    width:100%; }
  .bp3-file-input.bp3-large,
  .bp3-large .bp3-file-input{
    height:40px; }
  .bp3-file-input .bp3-file-upload-input-custom-text::after{
    content:attr(bp3-button-text); }

.bp3-file-upload-input{
  outline:none;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
  background:#ffffff;
  height:30px;
  padding:0 10px;
  vertical-align:middle;
  line-height:30px;
  color:#182026;
  font-size:14px;
  font-weight:400;
  -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  -webkit-appearance:none;
     -moz-appearance:none;
          appearance:none;
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  position:absolute;
  top:0;
  right:0;
  left:0;
  padding-right:80px;
  color:rgba(92, 112, 128, 0.6);
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-file-upload-input::-webkit-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-file-upload-input::-moz-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-file-upload-input:-ms-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-file-upload-input::-ms-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-file-upload-input::placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-file-upload-input:focus, .bp3-file-upload-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-file-upload-input[type="search"], .bp3-file-upload-input.bp3-round{
    border-radius:30px;
    -webkit-box-sizing:border-box;
            box-sizing:border-box;
    padding-left:10px; }
  .bp3-file-upload-input[readonly]{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-file-upload-input:disabled, .bp3-file-upload-input.bp3-disabled{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(206, 217, 224, 0.5);
    cursor:not-allowed;
    color:rgba(92, 112, 128, 0.6);
    resize:none; }
  .bp3-file-upload-input::after{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    background-color:#f5f8fa;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
    color:#182026;
    min-width:24px;
    min-height:24px;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    position:absolute;
    top:0;
    right:0;
    margin:3px;
    border-radius:3px;
    width:70px;
    text-align:center;
    line-height:24px;
    content:"Browse"; }
    .bp3-file-upload-input::after:hover{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
      background-clip:padding-box;
      background-color:#ebf1f5; }
    .bp3-file-upload-input::after:active, .bp3-file-upload-input::after.bp3-active{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#d8e1e8;
      background-image:none; }
    .bp3-file-upload-input::after:disabled, .bp3-file-upload-input::after.bp3-disabled{
      outline:none;
      -webkit-box-shadow:none;
              box-shadow:none;
      background-color:rgba(206, 217, 224, 0.5);
      background-image:none;
      cursor:not-allowed;
      color:rgba(92, 112, 128, 0.6); }
      .bp3-file-upload-input::after:disabled.bp3-active, .bp3-file-upload-input::after:disabled.bp3-active:hover, .bp3-file-upload-input::after.bp3-disabled.bp3-active, .bp3-file-upload-input::after.bp3-disabled.bp3-active:hover{
        background:rgba(206, 217, 224, 0.7); }
  .bp3-file-upload-input:hover::after{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    background-clip:padding-box;
    background-color:#ebf1f5; }
  .bp3-file-upload-input:active::after{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background-color:#d8e1e8;
    background-image:none; }
  .bp3-large .bp3-file-upload-input{
    height:40px;
    line-height:40px;
    font-size:16px;
    padding-right:95px; }
    .bp3-large .bp3-file-upload-input[type="search"], .bp3-large .bp3-file-upload-input.bp3-round{
      padding:0 15px; }
    .bp3-large .bp3-file-upload-input::after{
      min-width:30px;
      min-height:30px;
      margin:5px;
      width:85px;
      line-height:30px; }
  .bp3-dark .bp3-file-upload-input{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    background:rgba(16, 22, 26, 0.3);
    color:#f5f8fa;
    color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-file-upload-input:disabled, .bp3-dark .bp3-file-upload-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(57, 75, 89, 0.5);
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-file-upload-input::after{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
      background-color:#394b59;
      background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
      background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
      color:#f5f8fa; }
      .bp3-dark .bp3-file-upload-input::after:hover, .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
        color:#f5f8fa; }
      .bp3-dark .bp3-file-upload-input::after:hover{
        -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
        background-color:#30404d; }
      .bp3-dark .bp3-file-upload-input::after:active, .bp3-dark .bp3-file-upload-input::after.bp3-active{
        -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
                box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
        background-color:#202b33;
        background-image:none; }
      .bp3-dark .bp3-file-upload-input::after:disabled, .bp3-dark .bp3-file-upload-input::after.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none;
        background-color:rgba(57, 75, 89, 0.5);
        background-image:none;
        color:rgba(167, 182, 194, 0.6); }
        .bp3-dark .bp3-file-upload-input::after:disabled.bp3-active, .bp3-dark .bp3-file-upload-input::after.bp3-disabled.bp3-active{
          background:rgba(57, 75, 89, 0.7); }
      .bp3-dark .bp3-file-upload-input::after .bp3-button-spinner .bp3-spinner-head{
        background:rgba(16, 22, 26, 0.5);
        stroke:#8a9ba8; }
    .bp3-dark .bp3-file-upload-input:hover::after{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
      background-color:#30404d; }
    .bp3-dark .bp3-file-upload-input:active::after{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#202b33;
      background-image:none; }

.bp3-file-upload-input::after{
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1); }
.bp3-form-group{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin:0 0 15px; }
  .bp3-form-group label.bp3-label{
    margin-bottom:5px; }
  .bp3-form-group .bp3-control{
    margin-top:7px; }
  .bp3-form-group .bp3-form-helper-text{
    margin-top:5px;
    color:#5c7080;
    font-size:12px; }
  .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
    color:#106ba3; }
  .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
    color:#0d8050; }
  .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
    color:#bf7326; }
  .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
    color:#c23030; }
  .bp3-form-group.bp3-inline{
    -webkit-box-orient:horizontal;
    -webkit-box-direction:normal;
        -ms-flex-direction:row;
            flex-direction:row;
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start; }
    .bp3-form-group.bp3-inline.bp3-large label.bp3-label{
      margin:0 10px 0 0;
      line-height:40px; }
    .bp3-form-group.bp3-inline label.bp3-label{
      margin:0 10px 0 0;
      line-height:30px; }
  .bp3-form-group.bp3-disabled .bp3-label,
  .bp3-form-group.bp3-disabled .bp3-text-muted,
  .bp3-form-group.bp3-disabled .bp3-form-helper-text{
    color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-dark .bp3-form-group.bp3-intent-primary .bp3-form-helper-text{
    color:#48aff0; }
  .bp3-dark .bp3-form-group.bp3-intent-success .bp3-form-helper-text{
    color:#3dcc91; }
  .bp3-dark .bp3-form-group.bp3-intent-warning .bp3-form-helper-text{
    color:#ffb366; }
  .bp3-dark .bp3-form-group.bp3-intent-danger .bp3-form-helper-text{
    color:#ff7373; }
  .bp3-dark .bp3-form-group .bp3-form-helper-text{
    color:#a7b6c2; }
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-label,
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-text-muted,
  .bp3-dark .bp3-form-group.bp3-disabled .bp3-form-helper-text{
    color:rgba(167, 182, 194, 0.6) !important; }
.bp3-input-group{
  display:block;
  position:relative; }
  .bp3-input-group .bp3-input{
    position:relative;
    width:100%; }
    .bp3-input-group .bp3-input:not(:first-child){
      padding-left:30px; }
    .bp3-input-group .bp3-input:not(:last-child){
      padding-right:30px; }
  .bp3-input-group .bp3-input-action,
  .bp3-input-group > .bp3-button,
  .bp3-input-group > .bp3-icon{
    position:absolute;
    top:0; }
    .bp3-input-group .bp3-input-action:first-child,
    .bp3-input-group > .bp3-button:first-child,
    .bp3-input-group > .bp3-icon:first-child{
      left:0; }
    .bp3-input-group .bp3-input-action:last-child,
    .bp3-input-group > .bp3-button:last-child,
    .bp3-input-group > .bp3-icon:last-child{
      right:0; }
  .bp3-input-group .bp3-button{
    min-width:24px;
    min-height:24px;
    margin:3px;
    padding:0 7px; }
    .bp3-input-group .bp3-button:empty{
      padding:0; }
  .bp3-input-group > .bp3-icon{
    z-index:1;
    color:#5c7080; }
    .bp3-input-group > .bp3-icon:empty{
      line-height:1;
      font-family:"Icons16", sans-serif;
      font-size:16px;
      font-weight:400;
      font-style:normal;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased; }
  .bp3-input-group > .bp3-icon,
  .bp3-input-group .bp3-input-action > .bp3-spinner{
    margin:7px; }
  .bp3-input-group .bp3-tag{
    margin:5px; }
  .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus),
  .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
    color:#5c7080; }
    .bp3-dark .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus), .bp3-dark
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus){
      color:#a7b6c2; }
    .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-standard,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:not(:hover):not(:focus) .bp3-icon-large{
      color:#5c7080; }
  .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled,
  .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled{
    color:rgba(92, 112, 128, 0.6) !important; }
    .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-standard, .bp3-input-group .bp3-input:not(:focus) + .bp3-button.bp3-minimal:disabled .bp3-icon-large,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-standard,
    .bp3-input-group .bp3-input:not(:focus) + .bp3-input-action .bp3-button.bp3-minimal:disabled .bp3-icon-large{
      color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-input-group.bp3-disabled{
    cursor:not-allowed; }
    .bp3-input-group.bp3-disabled .bp3-icon{
      color:rgba(92, 112, 128, 0.6); }
  .bp3-input-group.bp3-large .bp3-button{
    min-width:30px;
    min-height:30px;
    margin:5px; }
  .bp3-input-group.bp3-large > .bp3-icon,
  .bp3-input-group.bp3-large .bp3-input-action > .bp3-spinner{
    margin:12px; }
  .bp3-input-group.bp3-large .bp3-input{
    height:40px;
    line-height:40px;
    font-size:16px; }
    .bp3-input-group.bp3-large .bp3-input[type="search"], .bp3-input-group.bp3-large .bp3-input.bp3-round{
      padding:0 15px; }
    .bp3-input-group.bp3-large .bp3-input:not(:first-child){
      padding-left:40px; }
    .bp3-input-group.bp3-large .bp3-input:not(:last-child){
      padding-right:40px; }
  .bp3-input-group.bp3-small .bp3-button{
    min-width:20px;
    min-height:20px;
    margin:2px; }
  .bp3-input-group.bp3-small .bp3-tag{
    min-width:20px;
    min-height:20px;
    margin:2px; }
  .bp3-input-group.bp3-small > .bp3-icon,
  .bp3-input-group.bp3-small .bp3-input-action > .bp3-spinner{
    margin:4px; }
  .bp3-input-group.bp3-small .bp3-input{
    height:24px;
    padding-right:8px;
    padding-left:8px;
    line-height:24px;
    font-size:12px; }
    .bp3-input-group.bp3-small .bp3-input[type="search"], .bp3-input-group.bp3-small .bp3-input.bp3-round{
      padding:0 12px; }
    .bp3-input-group.bp3-small .bp3-input:not(:first-child){
      padding-left:24px; }
    .bp3-input-group.bp3-small .bp3-input:not(:last-child){
      padding-right:24px; }
  .bp3-input-group.bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:100%; }
  .bp3-input-group.bp3-round .bp3-button,
  .bp3-input-group.bp3-round .bp3-input,
  .bp3-input-group.bp3-round .bp3-tag{
    border-radius:30px; }
  .bp3-dark .bp3-input-group .bp3-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-input-group.bp3-disabled .bp3-icon{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-input-group.bp3-intent-primary .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-primary .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-primary .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #137cbd;
              box-shadow:inset 0 0 0 1px #137cbd; }
    .bp3-input-group.bp3-intent-primary .bp3-input:disabled, .bp3-input-group.bp3-intent-primary .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-primary > .bp3-icon{
    color:#106ba3; }
    .bp3-dark .bp3-input-group.bp3-intent-primary > .bp3-icon{
      color:#48aff0; }
  .bp3-input-group.bp3-intent-success .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-success .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-success .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #0f9960;
              box-shadow:inset 0 0 0 1px #0f9960; }
    .bp3-input-group.bp3-intent-success .bp3-input:disabled, .bp3-input-group.bp3-intent-success .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-success > .bp3-icon{
    color:#0d8050; }
    .bp3-dark .bp3-input-group.bp3-intent-success > .bp3-icon{
      color:#3dcc91; }
  .bp3-input-group.bp3-intent-warning .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-warning .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-warning .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #d9822b;
              box-shadow:inset 0 0 0 1px #d9822b; }
    .bp3-input-group.bp3-intent-warning .bp3-input:disabled, .bp3-input-group.bp3-intent-warning .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-warning > .bp3-icon{
    color:#bf7326; }
    .bp3-dark .bp3-input-group.bp3-intent-warning > .bp3-icon{
      color:#ffb366; }
  .bp3-input-group.bp3-intent-danger .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-danger .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input-group.bp3-intent-danger .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #db3737;
              box-shadow:inset 0 0 0 1px #db3737; }
    .bp3-input-group.bp3-intent-danger .bp3-input:disabled, .bp3-input-group.bp3-intent-danger .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-input-group.bp3-intent-danger > .bp3-icon{
    color:#c23030; }
    .bp3-dark .bp3-input-group.bp3-intent-danger > .bp3-icon{
      color:#ff7373; }
.bp3-input{
  outline:none;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
  background:#ffffff;
  height:30px;
  padding:0 10px;
  vertical-align:middle;
  line-height:30px;
  color:#182026;
  font-size:14px;
  font-weight:400;
  -webkit-transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-box-shadow 100ms cubic-bezier(0.4, 1, 0.75, 0.9);
  -webkit-appearance:none;
     -moz-appearance:none;
          appearance:none; }
  .bp3-input::-webkit-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input::-moz-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input:-ms-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input::-ms-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input::placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input:focus, .bp3-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-input[type="search"], .bp3-input.bp3-round{
    border-radius:30px;
    -webkit-box-sizing:border-box;
            box-sizing:border-box;
    padding-left:10px; }
  .bp3-input[readonly]{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.15); }
  .bp3-input:disabled, .bp3-input.bp3-disabled{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(206, 217, 224, 0.5);
    cursor:not-allowed;
    color:rgba(92, 112, 128, 0.6);
    resize:none; }
  .bp3-input.bp3-large{
    height:40px;
    line-height:40px;
    font-size:16px; }
    .bp3-input.bp3-large[type="search"], .bp3-input.bp3-large.bp3-round{
      padding:0 15px; }
  .bp3-input.bp3-small{
    height:24px;
    padding-right:8px;
    padding-left:8px;
    line-height:24px;
    font-size:12px; }
    .bp3-input.bp3-small[type="search"], .bp3-input.bp3-small.bp3-round{
      padding:0 12px; }
  .bp3-input.bp3-fill{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:100%; }
  .bp3-dark .bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    background:rgba(16, 22, 26, 0.3);
    color:#f5f8fa; }
    .bp3-dark .bp3-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-input:disabled, .bp3-dark .bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(57, 75, 89, 0.5);
      color:rgba(167, 182, 194, 0.6); }
  .bp3-input.bp3-intent-primary{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-primary:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-primary[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #137cbd;
              box-shadow:inset 0 0 0 1px #137cbd; }
    .bp3-input.bp3-intent-primary:disabled, .bp3-input.bp3-intent-primary.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px #137cbd, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-primary:focus{
        -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-primary[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #137cbd;
                box-shadow:inset 0 0 0 1px #137cbd; }
      .bp3-dark .bp3-input.bp3-intent-primary:disabled, .bp3-dark .bp3-input.bp3-intent-primary.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-success{
    -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-success:focus{
      -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-success[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #0f9960;
              box-shadow:inset 0 0 0 1px #0f9960; }
    .bp3-input.bp3-intent-success:disabled, .bp3-input.bp3-intent-success.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-success{
      -webkit-box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), 0 0 0 0 rgba(15, 153, 96, 0), inset 0 0 0 1px #0f9960, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-success:focus{
        -webkit-box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #0f9960, 0 0 0 1px #0f9960, 0 0 0 3px rgba(15, 153, 96, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-success[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #0f9960;
                box-shadow:inset 0 0 0 1px #0f9960; }
      .bp3-dark .bp3-input.bp3-intent-success:disabled, .bp3-dark .bp3-input.bp3-intent-success.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-warning{
    -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-warning:focus{
      -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-warning[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #d9822b;
              box-shadow:inset 0 0 0 1px #d9822b; }
    .bp3-input.bp3-intent-warning:disabled, .bp3-input.bp3-intent-warning.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), 0 0 0 0 rgba(217, 130, 43, 0), inset 0 0 0 1px #d9822b, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-warning:focus{
        -webkit-box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #d9822b, 0 0 0 1px #d9822b, 0 0 0 3px rgba(217, 130, 43, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-warning[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #d9822b;
                box-shadow:inset 0 0 0 1px #d9822b; }
      .bp3-dark .bp3-input.bp3-intent-warning:disabled, .bp3-dark .bp3-input.bp3-intent-warning.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input.bp3-intent-danger{
    -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.15), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-danger:focus{
      -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-input.bp3-intent-danger[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px #db3737;
              box-shadow:inset 0 0 0 1px #db3737; }
    .bp3-input.bp3-intent-danger:disabled, .bp3-input.bp3-intent-danger.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none; }
    .bp3-dark .bp3-input.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), 0 0 0 0 rgba(219, 55, 55, 0), inset 0 0 0 1px #db3737, inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-danger:focus{
        -webkit-box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
                box-shadow:0 0 0 1px #db3737, 0 0 0 1px #db3737, 0 0 0 3px rgba(219, 55, 55, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
      .bp3-dark .bp3-input.bp3-intent-danger[readonly]{
        -webkit-box-shadow:inset 0 0 0 1px #db3737;
                box-shadow:inset 0 0 0 1px #db3737; }
      .bp3-dark .bp3-input.bp3-intent-danger:disabled, .bp3-dark .bp3-input.bp3-intent-danger.bp3-disabled{
        -webkit-box-shadow:none;
                box-shadow:none; }
  .bp3-input::-ms-clear{
    display:none; }
textarea.bp3-input{
  max-width:100%;
  padding:10px; }
  textarea.bp3-input, textarea.bp3-input.bp3-large, textarea.bp3-input.bp3-small{
    height:auto;
    line-height:inherit; }
  textarea.bp3-input.bp3-small{
    padding:8px; }
  .bp3-dark textarea.bp3-input{
    -webkit-box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), 0 0 0 0 rgba(19, 124, 189, 0), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    background:rgba(16, 22, 26, 0.3);
    color:#f5f8fa; }
    .bp3-dark textarea.bp3-input::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input::placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark textarea.bp3-input:focus{
      -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark textarea.bp3-input[readonly]{
      -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark textarea.bp3-input:disabled, .bp3-dark textarea.bp3-input.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:rgba(57, 75, 89, 0.5);
      color:rgba(167, 182, 194, 0.6); }
label.bp3-label{
  display:block;
  margin-top:0;
  margin-bottom:15px; }
  label.bp3-label .bp3-html-select,
  label.bp3-label .bp3-input,
  label.bp3-label .bp3-select,
  label.bp3-label .bp3-slider,
  label.bp3-label .bp3-popover-wrapper{
    display:block;
    margin-top:5px;
    text-transform:none; }
  label.bp3-label .bp3-button-group{
    margin-top:5px; }
  label.bp3-label .bp3-select select,
  label.bp3-label .bp3-html-select select{
    width:100%;
    vertical-align:top;
    font-weight:400; }
  label.bp3-label.bp3-disabled,
  label.bp3-label.bp3-disabled .bp3-text-muted{
    color:rgba(92, 112, 128, 0.6); }
  label.bp3-label.bp3-inline{
    line-height:30px; }
    label.bp3-label.bp3-inline .bp3-html-select,
    label.bp3-label.bp3-inline .bp3-input,
    label.bp3-label.bp3-inline .bp3-input-group,
    label.bp3-label.bp3-inline .bp3-select,
    label.bp3-label.bp3-inline .bp3-popover-wrapper{
      display:inline-block;
      margin:0 0 0 5px;
      vertical-align:top; }
    label.bp3-label.bp3-inline .bp3-button-group{
      margin:0 0 0 5px; }
    label.bp3-label.bp3-inline .bp3-input-group .bp3-input{
      margin-left:0; }
    label.bp3-label.bp3-inline.bp3-large{
      line-height:40px; }
  label.bp3-label:not(.bp3-inline) .bp3-popover-target{
    display:block; }
  .bp3-dark label.bp3-label{
    color:#f5f8fa; }
    .bp3-dark label.bp3-label.bp3-disabled,
    .bp3-dark label.bp3-label.bp3-disabled .bp3-text-muted{
      color:rgba(167, 182, 194, 0.6); }
.bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button{
  -webkit-box-flex:1;
      -ms-flex:1 1 14px;
          flex:1 1 14px;
  width:30px;
  min-height:0;
  padding:0; }
  .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:first-child{
    border-radius:0 3px 0 0; }
  .bp3-numeric-input .bp3-button-group.bp3-vertical > .bp3-button:last-child{
    border-radius:0 0 3px 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:first-child{
  border-radius:3px 0 0 0; }

.bp3-numeric-input .bp3-button-group.bp3-vertical:first-child > .bp3-button:last-child{
  border-radius:0 0 0 3px; }

.bp3-numeric-input.bp3-large .bp3-button-group.bp3-vertical > .bp3-button{
  width:40px; }

form{
  display:block; }
.bp3-html-select select,
.bp3-select select{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  border:none;
  border-radius:3px;
  cursor:pointer;
  padding:5px 10px;
  vertical-align:middle;
  text-align:left;
  font-size:14px;
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
  background-color:#f5f8fa;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
  color:#182026;
  border-radius:3px;
  width:100%;
  height:30px;
  padding:0 25px 0 10px;
  -moz-appearance:none;
  -webkit-appearance:none; }
  .bp3-html-select select > *, .bp3-select select > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-html-select select > .bp3-fill, .bp3-select select > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-html-select select::before,
  .bp3-select select::before, .bp3-html-select select > *, .bp3-select select > *{
    margin-right:7px; }
  .bp3-html-select select:empty::before,
  .bp3-select select:empty::before,
  .bp3-html-select select > :last-child,
  .bp3-select select > :last-child{
    margin-right:0; }
  .bp3-html-select select:hover,
  .bp3-select select:hover{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    background-clip:padding-box;
    background-color:#ebf1f5; }
  .bp3-html-select select:active,
  .bp3-select select:active, .bp3-html-select select.bp3-active,
  .bp3-select select.bp3-active{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background-color:#d8e1e8;
    background-image:none; }
  .bp3-html-select select:disabled,
  .bp3-select select:disabled, .bp3-html-select select.bp3-disabled,
  .bp3-select select.bp3-disabled{
    outline:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    background-color:rgba(206, 217, 224, 0.5);
    background-image:none;
    cursor:not-allowed;
    color:rgba(92, 112, 128, 0.6); }
    .bp3-html-select select:disabled.bp3-active,
    .bp3-select select:disabled.bp3-active, .bp3-html-select select:disabled.bp3-active:hover,
    .bp3-select select:disabled.bp3-active:hover, .bp3-html-select select.bp3-disabled.bp3-active,
    .bp3-select select.bp3-disabled.bp3-active, .bp3-html-select select.bp3-disabled.bp3-active:hover,
    .bp3-select select.bp3-disabled.bp3-active:hover{
      background:rgba(206, 217, 224, 0.7); }

.bp3-html-select.bp3-minimal select,
.bp3-select.bp3-minimal select{
  -webkit-box-shadow:none;
          box-shadow:none;
  background:none; }
  .bp3-html-select.bp3-minimal select:hover,
  .bp3-select.bp3-minimal select:hover{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(167, 182, 194, 0.3);
    text-decoration:none;
    color:#182026; }
  .bp3-html-select.bp3-minimal select:active,
  .bp3-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal select.bp3-active,
  .bp3-select.bp3-minimal select.bp3-active{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:rgba(115, 134, 148, 0.3);
    color:#182026; }
  .bp3-html-select.bp3-minimal select:disabled,
  .bp3-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal select:disabled:hover,
  .bp3-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal select.bp3-disabled,
  .bp3-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal select.bp3-disabled:hover,
  .bp3-select.bp3-minimal select.bp3-disabled:hover{
    background:none;
    cursor:not-allowed;
    color:rgba(92, 112, 128, 0.6); }
    .bp3-html-select.bp3-minimal select:disabled.bp3-active,
    .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active,
    .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active,
    .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active,
    .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active{
      background:rgba(115, 134, 148, 0.3); }
  .bp3-dark .bp3-html-select.bp3-minimal select, .bp3-html-select.bp3-minimal .bp3-dark select,
  .bp3-dark .bp3-select.bp3-minimal select, .bp3-select.bp3-minimal .bp3-dark select{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:none;
    color:inherit; }
    .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
    .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover, .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
    .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:none; }
    .bp3-dark .bp3-html-select.bp3-minimal select:hover, .bp3-html-select.bp3-minimal .bp3-dark select:hover,
    .bp3-dark .bp3-select.bp3-minimal select:hover, .bp3-select.bp3-minimal .bp3-dark select:hover{
      background:rgba(138, 155, 168, 0.15); }
    .bp3-dark .bp3-html-select.bp3-minimal select:active, .bp3-html-select.bp3-minimal .bp3-dark select:active,
    .bp3-dark .bp3-select.bp3-minimal select:active, .bp3-select.bp3-minimal .bp3-dark select:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-active,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-active{
      background:rgba(138, 155, 168, 0.3);
      color:#f5f8fa; }
    .bp3-dark .bp3-html-select.bp3-minimal select:disabled, .bp3-html-select.bp3-minimal .bp3-dark select:disabled,
    .bp3-dark .bp3-select.bp3-minimal select:disabled, .bp3-select.bp3-minimal .bp3-dark select:disabled, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover,
    .bp3-dark .bp3-select.bp3-minimal select:disabled:hover, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover{
      background:none;
      cursor:not-allowed;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-html-select.bp3-minimal select:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select:disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select:disabled:hover.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-disabled:hover.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-disabled:hover.bp3-active{
        background:rgba(138, 155, 168, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-primary,
  .bp3-select.bp3-minimal select.bp3-intent-primary{
    color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
    .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
    .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:none;
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover,
    .bp3-select.bp3-minimal select.bp3-intent-primary:hover{
      background:rgba(19, 124, 189, 0.15);
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:active,
    .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active{
      background:rgba(19, 124, 189, 0.3);
      color:#106ba3; }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled{
      background:none;
      color:rgba(16, 107, 163, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active{
        background:rgba(19, 124, 189, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-primary .bp3-button-spinner .bp3-spinner-head{
      stroke:#106ba3; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary{
      color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:hover{
        background:rgba(19, 124, 189, 0.2);
        color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-active{
        background:rgba(19, 124, 189, 0.3);
        color:#48aff0; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled{
        background:none;
        color:rgba(72, 175, 240, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-primary.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-primary.bp3-disabled.bp3-active{
          background:rgba(19, 124, 189, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-success,
  .bp3-select.bp3-minimal select.bp3-intent-success{
    color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
    .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
    .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:none;
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:hover,
    .bp3-select.bp3-minimal select.bp3-intent-success:hover{
      background:rgba(15, 153, 96, 0.15);
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:active,
    .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active{
      background:rgba(15, 153, 96, 0.3);
      color:#0d8050; }
    .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled{
      background:none;
      color:rgba(13, 128, 80, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active{
        background:rgba(15, 153, 96, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-success .bp3-button-spinner .bp3-spinner-head{
      stroke:#0d8050; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success{
      color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:hover{
        background:rgba(15, 153, 96, 0.2);
        color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-active{
        background:rgba(15, 153, 96, 0.3);
        color:#3dcc91; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled{
        background:none;
        color:rgba(61, 204, 145, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-success.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-success.bp3-disabled.bp3-active{
          background:rgba(15, 153, 96, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-warning,
  .bp3-select.bp3-minimal select.bp3-intent-warning{
    color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
    .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
    .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:none;
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover,
    .bp3-select.bp3-minimal select.bp3-intent-warning:hover{
      background:rgba(217, 130, 43, 0.15);
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:active,
    .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active{
      background:rgba(217, 130, 43, 0.3);
      color:#bf7326; }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled{
      background:none;
      color:rgba(191, 115, 38, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active{
        background:rgba(217, 130, 43, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-warning .bp3-button-spinner .bp3-spinner-head{
      stroke:#bf7326; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning{
      color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:hover{
        background:rgba(217, 130, 43, 0.2);
        color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-active{
        background:rgba(217, 130, 43, 0.3);
        color:#ffb366; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled{
        background:none;
        color:rgba(255, 179, 102, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-warning.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-warning.bp3-disabled.bp3-active{
          background:rgba(217, 130, 43, 0.3); }
  .bp3-html-select.bp3-minimal select.bp3-intent-danger,
  .bp3-select.bp3-minimal select.bp3-intent-danger{
    color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
    .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
    .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
      -webkit-box-shadow:none;
              box-shadow:none;
      background:none;
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover,
    .bp3-select.bp3-minimal select.bp3-intent-danger:hover{
      background:rgba(219, 55, 55, 0.15);
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:active,
    .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active{
      background:rgba(219, 55, 55, 0.3);
      color:#c23030; }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled,
    .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled,
    .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled{
      background:none;
      color:rgba(194, 48, 48, 0.5); }
      .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active,
      .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active{
        background:rgba(219, 55, 55, 0.3); }
    .bp3-html-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head, .bp3-select.bp3-minimal select.bp3-intent-danger .bp3-button-spinner .bp3-spinner-head{
      stroke:#c23030; }
    .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger,
    .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger{
      color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:hover, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:hover{
        background:rgba(219, 55, 55, 0.2);
        color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-active{
        background:rgba(219, 55, 55, 0.3);
        color:#ff7373; }
      .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled,
      .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled{
        background:none;
        color:rgba(255, 115, 115, 0.5); }
        .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger:disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger:disabled.bp3-active, .bp3-dark .bp3-html-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-html-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active,
        .bp3-dark .bp3-select.bp3-minimal select.bp3-intent-danger.bp3-disabled.bp3-active, .bp3-select.bp3-minimal .bp3-dark select.bp3-intent-danger.bp3-disabled.bp3-active{
          background:rgba(219, 55, 55, 0.3); }

.bp3-html-select.bp3-large select,
.bp3-select.bp3-large select{
  height:40px;
  padding-right:35px;
  font-size:16px; }

.bp3-dark .bp3-html-select select, .bp3-dark .bp3-select select{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
  background-color:#394b59;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
  color:#f5f8fa; }
  .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover, .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
    color:#f5f8fa; }
  .bp3-dark .bp3-html-select select:hover, .bp3-dark .bp3-select select:hover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    background-color:#30404d; }
  .bp3-dark .bp3-html-select select:active, .bp3-dark .bp3-select select:active, .bp3-dark .bp3-html-select select.bp3-active, .bp3-dark .bp3-select select.bp3-active{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background-color:#202b33;
    background-image:none; }
  .bp3-dark .bp3-html-select select:disabled, .bp3-dark .bp3-select select:disabled, .bp3-dark .bp3-html-select select.bp3-disabled, .bp3-dark .bp3-select select.bp3-disabled{
    -webkit-box-shadow:none;
            box-shadow:none;
    background-color:rgba(57, 75, 89, 0.5);
    background-image:none;
    color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-html-select select:disabled.bp3-active, .bp3-dark .bp3-select select:disabled.bp3-active, .bp3-dark .bp3-html-select select.bp3-disabled.bp3-active, .bp3-dark .bp3-select select.bp3-disabled.bp3-active{
      background:rgba(57, 75, 89, 0.7); }
  .bp3-dark .bp3-html-select select .bp3-button-spinner .bp3-spinner-head, .bp3-dark .bp3-select select .bp3-button-spinner .bp3-spinner-head{
    background:rgba(16, 22, 26, 0.5);
    stroke:#8a9ba8; }

.bp3-html-select select:disabled,
.bp3-select select:disabled{
  -webkit-box-shadow:none;
          box-shadow:none;
  background-color:rgba(206, 217, 224, 0.5);
  cursor:not-allowed;
  color:rgba(92, 112, 128, 0.6); }

.bp3-html-select .bp3-icon,
.bp3-select .bp3-icon, .bp3-select::after{
  position:absolute;
  top:7px;
  right:7px;
  color:#5c7080;
  pointer-events:none; }
  .bp3-html-select .bp3-disabled.bp3-icon,
  .bp3-select .bp3-disabled.bp3-icon, .bp3-disabled.bp3-select::after{
    color:rgba(92, 112, 128, 0.6); }
.bp3-html-select,
.bp3-select{
  display:inline-block;
  position:relative;
  vertical-align:middle;
  letter-spacing:normal; }
  .bp3-html-select select::-ms-expand,
  .bp3-select select::-ms-expand{
    display:none; }
  .bp3-html-select .bp3-icon,
  .bp3-select .bp3-icon{
    color:#5c7080; }
    .bp3-html-select .bp3-icon:hover,
    .bp3-select .bp3-icon:hover{
      color:#182026; }
    .bp3-dark .bp3-html-select .bp3-icon, .bp3-dark
    .bp3-select .bp3-icon{
      color:#a7b6c2; }
      .bp3-dark .bp3-html-select .bp3-icon:hover, .bp3-dark
      .bp3-select .bp3-icon:hover{
        color:#f5f8fa; }
  .bp3-html-select.bp3-large::after,
  .bp3-html-select.bp3-large .bp3-icon,
  .bp3-select.bp3-large::after,
  .bp3-select.bp3-large .bp3-icon{
    top:12px;
    right:12px; }
  .bp3-html-select.bp3-fill,
  .bp3-html-select.bp3-fill select,
  .bp3-select.bp3-fill,
  .bp3-select.bp3-fill select{
    width:100%; }
  .bp3-dark .bp3-html-select option, .bp3-dark
  .bp3-select option{
    background-color:#30404d;
    color:#f5f8fa; }
  .bp3-dark .bp3-html-select::after, .bp3-dark
  .bp3-select::after{
    color:#a7b6c2; }

.bp3-select::after{
  line-height:1;
  font-family:"Icons16", sans-serif;
  font-size:16px;
  font-weight:400;
  font-style:normal;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  content:""; }
.bp3-running-text table, table.bp3-html-table{
  border-spacing:0;
  font-size:14px; }
  .bp3-running-text table th, table.bp3-html-table th,
  .bp3-running-text table td,
  table.bp3-html-table td{
    padding:11px;
    vertical-align:top;
    text-align:left; }
  .bp3-running-text table th, table.bp3-html-table th{
    color:#182026;
    font-weight:600; }
  
  .bp3-running-text table td,
  table.bp3-html-table td{
    color:#182026; }
  .bp3-running-text table tbody tr:first-child th, table.bp3-html-table tbody tr:first-child th,
  .bp3-running-text table tbody tr:first-child td,
  table.bp3-html-table tbody tr:first-child td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-running-text table th, .bp3-running-text .bp3-dark table th, .bp3-dark table.bp3-html-table th{
    color:#f5f8fa; }
  .bp3-dark .bp3-running-text table td, .bp3-running-text .bp3-dark table td, .bp3-dark table.bp3-html-table td{
    color:#f5f8fa; }
  .bp3-dark .bp3-running-text table tbody tr:first-child th, .bp3-running-text .bp3-dark table tbody tr:first-child th, .bp3-dark table.bp3-html-table tbody tr:first-child th,
  .bp3-dark .bp3-running-text table tbody tr:first-child td,
  .bp3-running-text .bp3-dark table tbody tr:first-child td,
  .bp3-dark table.bp3-html-table tbody tr:first-child td{
    -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }

table.bp3-html-table.bp3-html-table-condensed th,
table.bp3-html-table.bp3-html-table-condensed td, table.bp3-html-table.bp3-small th,
table.bp3-html-table.bp3-small td{
  padding-top:6px;
  padding-bottom:6px; }

table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
  background:rgba(191, 204, 214, 0.15); }

table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
  -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered tbody tr td{
  -webkit-box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15);
          box-shadow:inset 0 1px 0 0 rgba(16, 22, 26, 0.15); }
  table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child){
    -webkit-box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 1px 1px 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
  -webkit-box-shadow:none;
          box-shadow:none; }
  table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:not(:first-child){
    -webkit-box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 1px 0 0 0 rgba(16, 22, 26, 0.15); }

table.bp3-html-table.bp3-interactive tbody tr:hover td{
  background-color:rgba(191, 204, 214, 0.3);
  cursor:pointer; }

table.bp3-html-table.bp3-interactive tbody tr:active td{
  background-color:rgba(191, 204, 214, 0.4); }

.bp3-dark table.bp3-html-table.bp3-html-table-striped tbody tr:nth-child(odd) td{
  background:rgba(92, 112, 128, 0.15); }

.bp3-dark table.bp3-html-table.bp3-html-table-bordered th:not(:first-child){
  -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
          box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }

.bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td{
  -webkit-box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15);
          box-shadow:inset 0 1px 0 0 rgba(255, 255, 255, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered tbody tr td:not(:first-child){
    -webkit-box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15);
            box-shadow:inset 1px 1px 0 0 rgba(255, 255, 255, 0.15); }

.bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td{
  -webkit-box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15);
          box-shadow:inset 1px 0 0 0 rgba(255, 255, 255, 0.15); }
  .bp3-dark table.bp3-html-table.bp3-html-table-bordered.bp3-html-table-striped tbody tr:not(:first-child) td:first-child{
    -webkit-box-shadow:none;
            box-shadow:none; }

.bp3-dark table.bp3-html-table.bp3-interactive tbody tr:hover td{
  background-color:rgba(92, 112, 128, 0.3);
  cursor:pointer; }

.bp3-dark table.bp3-html-table.bp3-interactive tbody tr:active td{
  background-color:rgba(92, 112, 128, 0.4); }

.bp3-key-combo{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center; }
  .bp3-key-combo > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-key-combo > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-key-combo::before,
  .bp3-key-combo > *{
    margin-right:5px; }
  .bp3-key-combo:empty::before,
  .bp3-key-combo > :last-child{
    margin-right:0; }

.bp3-hotkey-dialog{
  top:40px;
  padding-bottom:0; }
  .bp3-hotkey-dialog .bp3-dialog-body{
    margin:0;
    padding:0; }
  .bp3-hotkey-dialog .bp3-hotkey-label{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1; }

.bp3-hotkey-column{
  margin:auto;
  max-height:80vh;
  overflow-y:auto;
  padding:30px; }
  .bp3-hotkey-column .bp3-heading{
    margin-bottom:20px; }
    .bp3-hotkey-column .bp3-heading:not(:first-child){
      margin-top:40px; }

.bp3-hotkey{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-pack:justify;
      -ms-flex-pack:justify;
          justify-content:space-between;
  margin-right:0;
  margin-left:0; }
  .bp3-hotkey:not(:last-child){
    margin-bottom:10px; }
.bp3-icon{
  display:inline-block;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  vertical-align:text-bottom; }
  .bp3-icon:not(:empty)::before{
    content:"" !important;
    content:unset !important; }
  .bp3-icon > svg{
    display:block; }
    .bp3-icon > svg:not([fill]){
      fill:currentColor; }

.bp3-icon.bp3-intent-primary, .bp3-icon-standard.bp3-intent-primary, .bp3-icon-large.bp3-intent-primary{
  color:#106ba3; }
  .bp3-dark .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-icon-large.bp3-intent-primary{
    color:#48aff0; }

.bp3-icon.bp3-intent-success, .bp3-icon-standard.bp3-intent-success, .bp3-icon-large.bp3-intent-success{
  color:#0d8050; }
  .bp3-dark .bp3-icon.bp3-intent-success, .bp3-dark .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-icon-large.bp3-intent-success{
    color:#3dcc91; }

.bp3-icon.bp3-intent-warning, .bp3-icon-standard.bp3-intent-warning, .bp3-icon-large.bp3-intent-warning{
  color:#bf7326; }
  .bp3-dark .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-icon-large.bp3-intent-warning{
    color:#ffb366; }

.bp3-icon.bp3-intent-danger, .bp3-icon-standard.bp3-intent-danger, .bp3-icon-large.bp3-intent-danger{
  color:#c23030; }
  .bp3-dark .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-icon-large.bp3-intent-danger{
    color:#ff7373; }

span.bp3-icon-standard{
  line-height:1;
  font-family:"Icons16", sans-serif;
  font-size:16px;
  font-weight:400;
  font-style:normal;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  display:inline-block; }

span.bp3-icon-large{
  line-height:1;
  font-family:"Icons20", sans-serif;
  font-size:20px;
  font-weight:400;
  font-style:normal;
  -moz-osx-font-smoothing:grayscale;
  -webkit-font-smoothing:antialiased;
  display:inline-block; }

span.bp3-icon:empty{
  line-height:1;
  font-family:"Icons20";
  font-size:inherit;
  font-weight:400;
  font-style:normal; }
  span.bp3-icon:empty::before{
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased; }

.bp3-icon-add::before{
  content:""; }

.bp3-icon-add-column-left::before{
  content:""; }

.bp3-icon-add-column-right::before{
  content:""; }

.bp3-icon-add-row-bottom::before{
  content:""; }

.bp3-icon-add-row-top::before{
  content:""; }

.bp3-icon-add-to-artifact::before{
  content:""; }

.bp3-icon-add-to-folder::before{
  content:""; }

.bp3-icon-airplane::before{
  content:""; }

.bp3-icon-align-center::before{
  content:""; }

.bp3-icon-align-justify::before{
  content:""; }

.bp3-icon-align-left::before{
  content:""; }

.bp3-icon-align-right::before{
  content:""; }

.bp3-icon-alignment-bottom::before{
  content:""; }

.bp3-icon-alignment-horizontal-center::before{
  content:""; }

.bp3-icon-alignment-left::before{
  content:""; }

.bp3-icon-alignment-right::before{
  content:""; }

.bp3-icon-alignment-top::before{
  content:""; }

.bp3-icon-alignment-vertical-center::before{
  content:""; }

.bp3-icon-annotation::before{
  content:""; }

.bp3-icon-application::before{
  content:""; }

.bp3-icon-applications::before{
  content:""; }

.bp3-icon-archive::before{
  content:""; }

.bp3-icon-arrow-bottom-left::before{
  content:"↙"; }

.bp3-icon-arrow-bottom-right::before{
  content:"↘"; }

.bp3-icon-arrow-down::before{
  content:"↓"; }

.bp3-icon-arrow-left::before{
  content:"←"; }

.bp3-icon-arrow-right::before{
  content:"→"; }

.bp3-icon-arrow-top-left::before{
  content:"↖"; }

.bp3-icon-arrow-top-right::before{
  content:"↗"; }

.bp3-icon-arrow-up::before{
  content:"↑"; }

.bp3-icon-arrows-horizontal::before{
  content:"↔"; }

.bp3-icon-arrows-vertical::before{
  content:"↕"; }

.bp3-icon-asterisk::before{
  content:"*"; }

.bp3-icon-automatic-updates::before{
  content:""; }

.bp3-icon-badge::before{
  content:""; }

.bp3-icon-ban-circle::before{
  content:""; }

.bp3-icon-bank-account::before{
  content:""; }

.bp3-icon-barcode::before{
  content:""; }

.bp3-icon-blank::before{
  content:""; }

.bp3-icon-blocked-person::before{
  content:""; }

.bp3-icon-bold::before{
  content:""; }

.bp3-icon-book::before{
  content:""; }

.bp3-icon-bookmark::before{
  content:""; }

.bp3-icon-box::before{
  content:""; }

.bp3-icon-briefcase::before{
  content:""; }

.bp3-icon-bring-data::before{
  content:""; }

.bp3-icon-build::before{
  content:""; }

.bp3-icon-calculator::before{
  content:""; }

.bp3-icon-calendar::before{
  content:""; }

.bp3-icon-camera::before{
  content:""; }

.bp3-icon-caret-down::before{
  content:"⌄"; }

.bp3-icon-caret-left::before{
  content:"〈"; }

.bp3-icon-caret-right::before{
  content:"〉"; }

.bp3-icon-caret-up::before{
  content:"⌃"; }

.bp3-icon-cell-tower::before{
  content:""; }

.bp3-icon-changes::before{
  content:""; }

.bp3-icon-chart::before{
  content:""; }

.bp3-icon-chat::before{
  content:""; }

.bp3-icon-chevron-backward::before{
  content:""; }

.bp3-icon-chevron-down::before{
  content:""; }

.bp3-icon-chevron-forward::before{
  content:""; }

.bp3-icon-chevron-left::before{
  content:""; }

.bp3-icon-chevron-right::before{
  content:""; }

.bp3-icon-chevron-up::before{
  content:""; }

.bp3-icon-circle::before{
  content:""; }

.bp3-icon-circle-arrow-down::before{
  content:""; }

.bp3-icon-circle-arrow-left::before{
  content:""; }

.bp3-icon-circle-arrow-right::before{
  content:""; }

.bp3-icon-circle-arrow-up::before{
  content:""; }

.bp3-icon-citation::before{
  content:""; }

.bp3-icon-clean::before{
  content:""; }

.bp3-icon-clipboard::before{
  content:""; }

.bp3-icon-cloud::before{
  content:"☁"; }

.bp3-icon-cloud-download::before{
  content:""; }

.bp3-icon-cloud-upload::before{
  content:""; }

.bp3-icon-code::before{
  content:""; }

.bp3-icon-code-block::before{
  content:""; }

.bp3-icon-cog::before{
  content:""; }

.bp3-icon-collapse-all::before{
  content:""; }

.bp3-icon-column-layout::before{
  content:""; }

.bp3-icon-comment::before{
  content:""; }

.bp3-icon-comparison::before{
  content:""; }

.bp3-icon-compass::before{
  content:""; }

.bp3-icon-compressed::before{
  content:""; }

.bp3-icon-confirm::before{
  content:""; }

.bp3-icon-console::before{
  content:""; }

.bp3-icon-contrast::before{
  content:""; }

.bp3-icon-control::before{
  content:""; }

.bp3-icon-credit-card::before{
  content:""; }

.bp3-icon-cross::before{
  content:"✗"; }

.bp3-icon-crown::before{
  content:""; }

.bp3-icon-cube::before{
  content:""; }

.bp3-icon-cube-add::before{
  content:""; }

.bp3-icon-cube-remove::before{
  content:""; }

.bp3-icon-curved-range-chart::before{
  content:""; }

.bp3-icon-cut::before{
  content:""; }

.bp3-icon-dashboard::before{
  content:""; }

.bp3-icon-data-lineage::before{
  content:""; }

.bp3-icon-database::before{
  content:""; }

.bp3-icon-delete::before{
  content:""; }

.bp3-icon-delta::before{
  content:"Δ"; }

.bp3-icon-derive-column::before{
  content:""; }

.bp3-icon-desktop::before{
  content:""; }

.bp3-icon-diagram-tree::before{
  content:""; }

.bp3-icon-direction-left::before{
  content:""; }

.bp3-icon-direction-right::before{
  content:""; }

.bp3-icon-disable::before{
  content:""; }

.bp3-icon-document::before{
  content:""; }

.bp3-icon-document-open::before{
  content:""; }

.bp3-icon-document-share::before{
  content:""; }

.bp3-icon-dollar::before{
  content:"$"; }

.bp3-icon-dot::before{
  content:"•"; }

.bp3-icon-double-caret-horizontal::before{
  content:""; }

.bp3-icon-double-caret-vertical::before{
  content:""; }

.bp3-icon-double-chevron-down::before{
  content:""; }

.bp3-icon-double-chevron-left::before{
  content:""; }

.bp3-icon-double-chevron-right::before{
  content:""; }

.bp3-icon-double-chevron-up::before{
  content:""; }

.bp3-icon-doughnut-chart::before{
  content:""; }

.bp3-icon-download::before{
  content:""; }

.bp3-icon-drag-handle-horizontal::before{
  content:""; }

.bp3-icon-drag-handle-vertical::before{
  content:""; }

.bp3-icon-draw::before{
  content:""; }

.bp3-icon-drive-time::before{
  content:""; }

.bp3-icon-duplicate::before{
  content:""; }

.bp3-icon-edit::before{
  content:"✎"; }

.bp3-icon-eject::before{
  content:"⏏"; }

.bp3-icon-endorsed::before{
  content:""; }

.bp3-icon-envelope::before{
  content:"✉"; }

.bp3-icon-equals::before{
  content:""; }

.bp3-icon-eraser::before{
  content:""; }

.bp3-icon-error::before{
  content:""; }

.bp3-icon-euro::before{
  content:"€"; }

.bp3-icon-exchange::before{
  content:""; }

.bp3-icon-exclude-row::before{
  content:""; }

.bp3-icon-expand-all::before{
  content:""; }

.bp3-icon-export::before{
  content:""; }

.bp3-icon-eye-off::before{
  content:""; }

.bp3-icon-eye-on::before{
  content:""; }

.bp3-icon-eye-open::before{
  content:""; }

.bp3-icon-fast-backward::before{
  content:""; }

.bp3-icon-fast-forward::before{
  content:""; }

.bp3-icon-feed::before{
  content:""; }

.bp3-icon-feed-subscribed::before{
  content:""; }

.bp3-icon-film::before{
  content:""; }

.bp3-icon-filter::before{
  content:""; }

.bp3-icon-filter-keep::before{
  content:""; }

.bp3-icon-filter-list::before{
  content:""; }

.bp3-icon-filter-open::before{
  content:""; }

.bp3-icon-filter-remove::before{
  content:""; }

.bp3-icon-flag::before{
  content:"⚑"; }

.bp3-icon-flame::before{
  content:""; }

.bp3-icon-flash::before{
  content:""; }

.bp3-icon-floppy-disk::before{
  content:""; }

.bp3-icon-flow-branch::before{
  content:""; }

.bp3-icon-flow-end::before{
  content:""; }

.bp3-icon-flow-linear::before{
  content:""; }

.bp3-icon-flow-review::before{
  content:""; }

.bp3-icon-flow-review-branch::before{
  content:""; }

.bp3-icon-flows::before{
  content:""; }

.bp3-icon-folder-close::before{
  content:""; }

.bp3-icon-folder-new::before{
  content:""; }

.bp3-icon-folder-open::before{
  content:""; }

.bp3-icon-folder-shared::before{
  content:""; }

.bp3-icon-folder-shared-open::before{
  content:""; }

.bp3-icon-follower::before{
  content:""; }

.bp3-icon-following::before{
  content:""; }

.bp3-icon-font::before{
  content:""; }

.bp3-icon-fork::before{
  content:""; }

.bp3-icon-form::before{
  content:""; }

.bp3-icon-full-circle::before{
  content:""; }

.bp3-icon-full-stacked-chart::before{
  content:""; }

.bp3-icon-fullscreen::before{
  content:""; }

.bp3-icon-function::before{
  content:""; }

.bp3-icon-gantt-chart::before{
  content:""; }

.bp3-icon-geolocation::before{
  content:""; }

.bp3-icon-geosearch::before{
  content:""; }

.bp3-icon-git-branch::before{
  content:""; }

.bp3-icon-git-commit::before{
  content:""; }

.bp3-icon-git-merge::before{
  content:""; }

.bp3-icon-git-new-branch::before{
  content:""; }

.bp3-icon-git-pull::before{
  content:""; }

.bp3-icon-git-push::before{
  content:""; }

.bp3-icon-git-repo::before{
  content:""; }

.bp3-icon-glass::before{
  content:""; }

.bp3-icon-globe::before{
  content:""; }

.bp3-icon-globe-network::before{
  content:""; }

.bp3-icon-graph::before{
  content:""; }

.bp3-icon-graph-remove::before{
  content:""; }

.bp3-icon-greater-than::before{
  content:""; }

.bp3-icon-greater-than-or-equal-to::before{
  content:""; }

.bp3-icon-grid::before{
  content:""; }

.bp3-icon-grid-view::before{
  content:""; }

.bp3-icon-group-objects::before{
  content:""; }

.bp3-icon-grouped-bar-chart::before{
  content:""; }

.bp3-icon-hand::before{
  content:""; }

.bp3-icon-hand-down::before{
  content:""; }

.bp3-icon-hand-left::before{
  content:""; }

.bp3-icon-hand-right::before{
  content:""; }

.bp3-icon-hand-up::before{
  content:""; }

.bp3-icon-header::before{
  content:""; }

.bp3-icon-header-one::before{
  content:""; }

.bp3-icon-header-two::before{
  content:""; }

.bp3-icon-headset::before{
  content:""; }

.bp3-icon-heart::before{
  content:"♥"; }

.bp3-icon-heart-broken::before{
  content:""; }

.bp3-icon-heat-grid::before{
  content:""; }

.bp3-icon-heatmap::before{
  content:""; }

.bp3-icon-help::before{
  content:"?"; }

.bp3-icon-helper-management::before{
  content:""; }

.bp3-icon-highlight::before{
  content:""; }

.bp3-icon-history::before{
  content:""; }

.bp3-icon-home::before{
  content:"⌂"; }

.bp3-icon-horizontal-bar-chart::before{
  content:""; }

.bp3-icon-horizontal-bar-chart-asc::before{
  content:""; }

.bp3-icon-horizontal-bar-chart-desc::before{
  content:""; }

.bp3-icon-horizontal-distribution::before{
  content:""; }

.bp3-icon-id-number::before{
  content:""; }

.bp3-icon-image-rotate-left::before{
  content:""; }

.bp3-icon-image-rotate-right::before{
  content:""; }

.bp3-icon-import::before{
  content:""; }

.bp3-icon-inbox::before{
  content:""; }

.bp3-icon-inbox-filtered::before{
  content:""; }

.bp3-icon-inbox-geo::before{
  content:""; }

.bp3-icon-inbox-search::before{
  content:""; }

.bp3-icon-inbox-update::before{
  content:""; }

.bp3-icon-info-sign::before{
  content:"ℹ"; }

.bp3-icon-inheritance::before{
  content:""; }

.bp3-icon-inner-join::before{
  content:""; }

.bp3-icon-insert::before{
  content:""; }

.bp3-icon-intersection::before{
  content:""; }

.bp3-icon-ip-address::before{
  content:""; }

.bp3-icon-issue::before{
  content:""; }

.bp3-icon-issue-closed::before{
  content:""; }

.bp3-icon-issue-new::before{
  content:""; }

.bp3-icon-italic::before{
  content:""; }

.bp3-icon-join-table::before{
  content:""; }

.bp3-icon-key::before{
  content:""; }

.bp3-icon-key-backspace::before{
  content:""; }

.bp3-icon-key-command::before{
  content:""; }

.bp3-icon-key-control::before{
  content:""; }

.bp3-icon-key-delete::before{
  content:""; }

.bp3-icon-key-enter::before{
  content:""; }

.bp3-icon-key-escape::before{
  content:""; }

.bp3-icon-key-option::before{
  content:""; }

.bp3-icon-key-shift::before{
  content:""; }

.bp3-icon-key-tab::before{
  content:""; }

.bp3-icon-known-vehicle::before{
  content:""; }

.bp3-icon-label::before{
  content:""; }

.bp3-icon-layer::before{
  content:""; }

.bp3-icon-layers::before{
  content:""; }

.bp3-icon-layout::before{
  content:""; }

.bp3-icon-layout-auto::before{
  content:""; }

.bp3-icon-layout-balloon::before{
  content:""; }

.bp3-icon-layout-circle::before{
  content:""; }

.bp3-icon-layout-grid::before{
  content:""; }

.bp3-icon-layout-group-by::before{
  content:""; }

.bp3-icon-layout-hierarchy::before{
  content:""; }

.bp3-icon-layout-linear::before{
  content:""; }

.bp3-icon-layout-skew-grid::before{
  content:""; }

.bp3-icon-layout-sorted-clusters::before{
  content:""; }

.bp3-icon-learning::before{
  content:""; }

.bp3-icon-left-join::before{
  content:""; }

.bp3-icon-less-than::before{
  content:""; }

.bp3-icon-less-than-or-equal-to::before{
  content:""; }

.bp3-icon-lifesaver::before{
  content:""; }

.bp3-icon-lightbulb::before{
  content:""; }

.bp3-icon-link::before{
  content:""; }

.bp3-icon-list::before{
  content:"☰"; }

.bp3-icon-list-columns::before{
  content:""; }

.bp3-icon-list-detail-view::before{
  content:""; }

.bp3-icon-locate::before{
  content:""; }

.bp3-icon-lock::before{
  content:""; }

.bp3-icon-log-in::before{
  content:""; }

.bp3-icon-log-out::before{
  content:""; }

.bp3-icon-manual::before{
  content:""; }

.bp3-icon-manually-entered-data::before{
  content:""; }

.bp3-icon-map::before{
  content:""; }

.bp3-icon-map-create::before{
  content:""; }

.bp3-icon-map-marker::before{
  content:""; }

.bp3-icon-maximize::before{
  content:""; }

.bp3-icon-media::before{
  content:""; }

.bp3-icon-menu::before{
  content:""; }

.bp3-icon-menu-closed::before{
  content:""; }

.bp3-icon-menu-open::before{
  content:""; }

.bp3-icon-merge-columns::before{
  content:""; }

.bp3-icon-merge-links::before{
  content:""; }

.bp3-icon-minimize::before{
  content:""; }

.bp3-icon-minus::before{
  content:"−"; }

.bp3-icon-mobile-phone::before{
  content:""; }

.bp3-icon-mobile-video::before{
  content:""; }

.bp3-icon-moon::before{
  content:""; }

.bp3-icon-more::before{
  content:""; }

.bp3-icon-mountain::before{
  content:""; }

.bp3-icon-move::before{
  content:""; }

.bp3-icon-mugshot::before{
  content:""; }

.bp3-icon-multi-select::before{
  content:""; }

.bp3-icon-music::before{
  content:""; }

.bp3-icon-new-drawing::before{
  content:""; }

.bp3-icon-new-grid-item::before{
  content:""; }

.bp3-icon-new-layer::before{
  content:""; }

.bp3-icon-new-layers::before{
  content:""; }

.bp3-icon-new-link::before{
  content:""; }

.bp3-icon-new-object::before{
  content:""; }

.bp3-icon-new-person::before{
  content:""; }

.bp3-icon-new-prescription::before{
  content:""; }

.bp3-icon-new-text-box::before{
  content:""; }

.bp3-icon-ninja::before{
  content:""; }

.bp3-icon-not-equal-to::before{
  content:""; }

.bp3-icon-notifications::before{
  content:""; }

.bp3-icon-notifications-updated::before{
  content:""; }

.bp3-icon-numbered-list::before{
  content:""; }

.bp3-icon-numerical::before{
  content:""; }

.bp3-icon-office::before{
  content:""; }

.bp3-icon-offline::before{
  content:""; }

.bp3-icon-oil-field::before{
  content:""; }

.bp3-icon-one-column::before{
  content:""; }

.bp3-icon-outdated::before{
  content:""; }

.bp3-icon-page-layout::before{
  content:""; }

.bp3-icon-panel-stats::before{
  content:""; }

.bp3-icon-panel-table::before{
  content:""; }

.bp3-icon-paperclip::before{
  content:""; }

.bp3-icon-paragraph::before{
  content:""; }

.bp3-icon-path::before{
  content:""; }

.bp3-icon-path-search::before{
  content:""; }

.bp3-icon-pause::before{
  content:""; }

.bp3-icon-people::before{
  content:""; }

.bp3-icon-percentage::before{
  content:""; }

.bp3-icon-person::before{
  content:""; }

.bp3-icon-phone::before{
  content:"☎"; }

.bp3-icon-pie-chart::before{
  content:""; }

.bp3-icon-pin::before{
  content:""; }

.bp3-icon-pivot::before{
  content:""; }

.bp3-icon-pivot-table::before{
  content:""; }

.bp3-icon-play::before{
  content:""; }

.bp3-icon-plus::before{
  content:"+"; }

.bp3-icon-polygon-filter::before{
  content:""; }

.bp3-icon-power::before{
  content:""; }

.bp3-icon-predictive-analysis::before{
  content:""; }

.bp3-icon-prescription::before{
  content:""; }

.bp3-icon-presentation::before{
  content:""; }

.bp3-icon-print::before{
  content:"⎙"; }

.bp3-icon-projects::before{
  content:""; }

.bp3-icon-properties::before{
  content:""; }

.bp3-icon-property::before{
  content:""; }

.bp3-icon-publish-function::before{
  content:""; }

.bp3-icon-pulse::before{
  content:""; }

.bp3-icon-random::before{
  content:""; }

.bp3-icon-record::before{
  content:""; }

.bp3-icon-redo::before{
  content:""; }

.bp3-icon-refresh::before{
  content:""; }

.bp3-icon-regression-chart::before{
  content:""; }

.bp3-icon-remove::before{
  content:""; }

.bp3-icon-remove-column::before{
  content:""; }

.bp3-icon-remove-column-left::before{
  content:""; }

.bp3-icon-remove-column-right::before{
  content:""; }

.bp3-icon-remove-row-bottom::before{
  content:""; }

.bp3-icon-remove-row-top::before{
  content:""; }

.bp3-icon-repeat::before{
  content:""; }

.bp3-icon-reset::before{
  content:""; }

.bp3-icon-resolve::before{
  content:""; }

.bp3-icon-rig::before{
  content:""; }

.bp3-icon-right-join::before{
  content:""; }

.bp3-icon-ring::before{
  content:""; }

.bp3-icon-rotate-document::before{
  content:""; }

.bp3-icon-rotate-page::before{
  content:""; }

.bp3-icon-satellite::before{
  content:""; }

.bp3-icon-saved::before{
  content:""; }

.bp3-icon-scatter-plot::before{
  content:""; }

.bp3-icon-search::before{
  content:""; }

.bp3-icon-search-around::before{
  content:""; }

.bp3-icon-search-template::before{
  content:""; }

.bp3-icon-search-text::before{
  content:""; }

.bp3-icon-segmented-control::before{
  content:""; }

.bp3-icon-select::before{
  content:""; }

.bp3-icon-selection::before{
  content:"⦿"; }

.bp3-icon-send-to::before{
  content:""; }

.bp3-icon-send-to-graph::before{
  content:""; }

.bp3-icon-send-to-map::before{
  content:""; }

.bp3-icon-series-add::before{
  content:""; }

.bp3-icon-series-configuration::before{
  content:""; }

.bp3-icon-series-derived::before{
  content:""; }

.bp3-icon-series-filtered::before{
  content:""; }

.bp3-icon-series-search::before{
  content:""; }

.bp3-icon-settings::before{
  content:""; }

.bp3-icon-share::before{
  content:""; }

.bp3-icon-shield::before{
  content:""; }

.bp3-icon-shop::before{
  content:""; }

.bp3-icon-shopping-cart::before{
  content:""; }

.bp3-icon-signal-search::before{
  content:""; }

.bp3-icon-sim-card::before{
  content:""; }

.bp3-icon-slash::before{
  content:""; }

.bp3-icon-small-cross::before{
  content:""; }

.bp3-icon-small-minus::before{
  content:""; }

.bp3-icon-small-plus::before{
  content:""; }

.bp3-icon-small-tick::before{
  content:""; }

.bp3-icon-snowflake::before{
  content:""; }

.bp3-icon-social-media::before{
  content:""; }

.bp3-icon-sort::before{
  content:""; }

.bp3-icon-sort-alphabetical::before{
  content:""; }

.bp3-icon-sort-alphabetical-desc::before{
  content:""; }

.bp3-icon-sort-asc::before{
  content:""; }

.bp3-icon-sort-desc::before{
  content:""; }

.bp3-icon-sort-numerical::before{
  content:""; }

.bp3-icon-sort-numerical-desc::before{
  content:""; }

.bp3-icon-split-columns::before{
  content:""; }

.bp3-icon-square::before{
  content:""; }

.bp3-icon-stacked-chart::before{
  content:""; }

.bp3-icon-star::before{
  content:"★"; }

.bp3-icon-star-empty::before{
  content:"☆"; }

.bp3-icon-step-backward::before{
  content:""; }

.bp3-icon-step-chart::before{
  content:""; }

.bp3-icon-step-forward::before{
  content:""; }

.bp3-icon-stop::before{
  content:""; }

.bp3-icon-stopwatch::before{
  content:""; }

.bp3-icon-strikethrough::before{
  content:""; }

.bp3-icon-style::before{
  content:""; }

.bp3-icon-swap-horizontal::before{
  content:""; }

.bp3-icon-swap-vertical::before{
  content:""; }

.bp3-icon-symbol-circle::before{
  content:""; }

.bp3-icon-symbol-cross::before{
  content:""; }

.bp3-icon-symbol-diamond::before{
  content:""; }

.bp3-icon-symbol-square::before{
  content:""; }

.bp3-icon-symbol-triangle-down::before{
  content:""; }

.bp3-icon-symbol-triangle-up::before{
  content:""; }

.bp3-icon-tag::before{
  content:""; }

.bp3-icon-take-action::before{
  content:""; }

.bp3-icon-taxi::before{
  content:""; }

.bp3-icon-text-highlight::before{
  content:""; }

.bp3-icon-th::before{
  content:""; }

.bp3-icon-th-derived::before{
  content:""; }

.bp3-icon-th-disconnect::before{
  content:""; }

.bp3-icon-th-filtered::before{
  content:""; }

.bp3-icon-th-list::before{
  content:""; }

.bp3-icon-thumbs-down::before{
  content:""; }

.bp3-icon-thumbs-up::before{
  content:""; }

.bp3-icon-tick::before{
  content:"✓"; }

.bp3-icon-tick-circle::before{
  content:""; }

.bp3-icon-time::before{
  content:"⏲"; }

.bp3-icon-timeline-area-chart::before{
  content:""; }

.bp3-icon-timeline-bar-chart::before{
  content:""; }

.bp3-icon-timeline-events::before{
  content:""; }

.bp3-icon-timeline-line-chart::before{
  content:""; }

.bp3-icon-tint::before{
  content:""; }

.bp3-icon-torch::before{
  content:""; }

.bp3-icon-tractor::before{
  content:""; }

.bp3-icon-train::before{
  content:""; }

.bp3-icon-translate::before{
  content:""; }

.bp3-icon-trash::before{
  content:""; }

.bp3-icon-tree::before{
  content:""; }

.bp3-icon-trending-down::before{
  content:""; }

.bp3-icon-trending-up::before{
  content:""; }

.bp3-icon-truck::before{
  content:""; }

.bp3-icon-two-columns::before{
  content:""; }

.bp3-icon-unarchive::before{
  content:""; }

.bp3-icon-underline::before{
  content:"⎁"; }

.bp3-icon-undo::before{
  content:"⎌"; }

.bp3-icon-ungroup-objects::before{
  content:""; }

.bp3-icon-unknown-vehicle::before{
  content:""; }

.bp3-icon-unlock::before{
  content:""; }

.bp3-icon-unpin::before{
  content:""; }

.bp3-icon-unresolve::before{
  content:""; }

.bp3-icon-updated::before{
  content:""; }

.bp3-icon-upload::before{
  content:""; }

.bp3-icon-user::before{
  content:""; }

.bp3-icon-variable::before{
  content:""; }

.bp3-icon-vertical-bar-chart-asc::before{
  content:""; }

.bp3-icon-vertical-bar-chart-desc::before{
  content:""; }

.bp3-icon-vertical-distribution::before{
  content:""; }

.bp3-icon-video::before{
  content:""; }

.bp3-icon-volume-down::before{
  content:""; }

.bp3-icon-volume-off::before{
  content:""; }

.bp3-icon-volume-up::before{
  content:""; }

.bp3-icon-walk::before{
  content:""; }

.bp3-icon-warning-sign::before{
  content:""; }

.bp3-icon-waterfall-chart::before{
  content:""; }

.bp3-icon-widget::before{
  content:""; }

.bp3-icon-widget-button::before{
  content:""; }

.bp3-icon-widget-footer::before{
  content:""; }

.bp3-icon-widget-header::before{
  content:""; }

.bp3-icon-wrench::before{
  content:""; }

.bp3-icon-zoom-in::before{
  content:""; }

.bp3-icon-zoom-out::before{
  content:""; }

.bp3-icon-zoom-to-fit::before{
  content:""; }
.bp3-submenu > .bp3-popover-wrapper{
  display:block; }

.bp3-submenu .bp3-popover-target{
  display:block; }

.bp3-submenu.bp3-popover{
  -webkit-box-shadow:none;
          box-shadow:none;
  padding:0 5px; }
  .bp3-submenu.bp3-popover > .bp3-popover-content{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-submenu.bp3-popover, .bp3-submenu.bp3-popover.bp3-dark{
    -webkit-box-shadow:none;
            box-shadow:none; }
    .bp3-dark .bp3-submenu.bp3-popover > .bp3-popover-content, .bp3-submenu.bp3-popover.bp3-dark > .bp3-popover-content{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
.bp3-menu{
  margin:0;
  border-radius:3px;
  background:#ffffff;
  min-width:180px;
  padding:5px;
  list-style:none;
  text-align:left;
  color:#182026; }

.bp3-menu-divider{
  display:block;
  margin:5px;
  border-top:1px solid rgba(16, 22, 26, 0.15); }
  .bp3-dark .bp3-menu-divider{
    border-top-color:rgba(255, 255, 255, 0.15); }

.bp3-menu-item{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  border-radius:2px;
  padding:5px 7px;
  text-decoration:none;
  line-height:20px;
  color:inherit;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-menu-item > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-menu-item > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-menu-item::before,
  .bp3-menu-item > *{
    margin-right:7px; }
  .bp3-menu-item:empty::before,
  .bp3-menu-item > :last-child{
    margin-right:0; }
  .bp3-menu-item > .bp3-fill{
    word-break:break-word; }
  .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
    background-color:rgba(167, 182, 194, 0.3);
    cursor:pointer;
    text-decoration:none; }
  .bp3-menu-item.bp3-disabled{
    background-color:inherit;
    cursor:not-allowed;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-dark .bp3-menu-item{
    color:inherit; }
    .bp3-dark .bp3-menu-item:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
      background-color:rgba(138, 155, 168, 0.15);
      color:inherit; }
    .bp3-dark .bp3-menu-item.bp3-disabled{
      background-color:inherit;
      color:rgba(167, 182, 194, 0.6); }
  .bp3-menu-item.bp3-intent-primary{
    color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-primary::before, .bp3-menu-item.bp3-intent-primary::after,
    .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
      color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary.bp3-active{
      background-color:#137cbd; }
    .bp3-menu-item.bp3-intent-primary:active{
      background-color:#106ba3; }
    .bp3-menu-item.bp3-intent-primary:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary:active, .bp3-menu-item.bp3-intent-primary:active::before, .bp3-menu-item.bp3-intent-primary:active::after,
    .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-menu-item.bp3-intent-primary.bp3-active::after,
    .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-success{
    color:#0d8050; }
    .bp3-menu-item.bp3-intent-success .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-success::before, .bp3-menu-item.bp3-intent-success::after,
    .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
      color:#0d8050; }
    .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success.bp3-active{
      background-color:#0f9960; }
    .bp3-menu-item.bp3-intent-success:active{
      background-color:#0d8050; }
    .bp3-menu-item.bp3-intent-success:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-menu-item.bp3-intent-success:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-menu-item.bp3-intent-success:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success:active, .bp3-menu-item.bp3-intent-success:active::before, .bp3-menu-item.bp3-intent-success:active::after,
    .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-menu-item.bp3-intent-success.bp3-active::after,
    .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-warning{
    color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-warning::before, .bp3-menu-item.bp3-intent-warning::after,
    .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
      color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning.bp3-active{
      background-color:#d9822b; }
    .bp3-menu-item.bp3-intent-warning:active{
      background-color:#bf7326; }
    .bp3-menu-item.bp3-intent-warning:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning:active, .bp3-menu-item.bp3-intent-warning:active::before, .bp3-menu-item.bp3-intent-warning:active::after,
    .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-menu-item.bp3-intent-warning.bp3-active::after,
    .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item.bp3-intent-danger{
    color:#c23030; }
    .bp3-menu-item.bp3-intent-danger .bp3-icon{
      color:inherit; }
    .bp3-menu-item.bp3-intent-danger::before, .bp3-menu-item.bp3-intent-danger::after,
    .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
      color:#c23030; }
    .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger.bp3-active{
      background-color:#db3737; }
    .bp3-menu-item.bp3-intent-danger:active{
      background-color:#c23030; }
    .bp3-menu-item.bp3-intent-danger:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
    .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
    .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger:active, .bp3-menu-item.bp3-intent-danger:active::before, .bp3-menu-item.bp3-intent-danger:active::after,
    .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-menu-item.bp3-intent-danger.bp3-active::after,
    .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
      color:#ffffff; }
  .bp3-menu-item::before{
    line-height:1;
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-weight:400;
    font-style:normal;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    margin-right:7px; }
  .bp3-menu-item::before,
  .bp3-menu-item > .bp3-icon{
    margin-top:2px;
    color:#5c7080; }
  .bp3-menu-item .bp3-menu-item-label{
    color:#5c7080; }
  .bp3-menu-item:hover, .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-menu-item{
    color:inherit; }
  .bp3-menu-item.bp3-active, .bp3-menu-item:active{
    background-color:rgba(115, 134, 148, 0.3); }
  .bp3-menu-item.bp3-disabled{
    outline:none !important;
    background-color:inherit !important;
    cursor:not-allowed !important;
    color:rgba(92, 112, 128, 0.6) !important; }
    .bp3-menu-item.bp3-disabled::before,
    .bp3-menu-item.bp3-disabled > .bp3-icon,
    .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
      color:rgba(92, 112, 128, 0.6) !important; }
  .bp3-large .bp3-menu-item{
    padding:9px 7px;
    line-height:22px;
    font-size:16px; }
    .bp3-large .bp3-menu-item .bp3-icon{
      margin-top:3px; }
    .bp3-large .bp3-menu-item::before{
      line-height:1;
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-weight:400;
      font-style:normal;
      -moz-osx-font-smoothing:grayscale;
      -webkit-font-smoothing:antialiased;
      margin-top:1px;
      margin-right:10px; }

button.bp3-menu-item{
  border:none;
  background:none;
  width:100%;
  text-align:left; }
.bp3-menu-header{
  display:block;
  margin:5px;
  border-top:1px solid rgba(16, 22, 26, 0.15);
  cursor:default;
  padding-left:2px; }
  .bp3-dark .bp3-menu-header{
    border-top-color:rgba(255, 255, 255, 0.15); }
  .bp3-menu-header:first-of-type{
    border-top:none; }
  .bp3-menu-header > h6{
    color:#182026;
    font-weight:600;
    overflow:hidden;
    text-overflow:ellipsis;
    white-space:nowrap;
    word-wrap:normal;
    margin:0;
    padding:10px 7px 0 1px;
    line-height:17px; }
    .bp3-dark .bp3-menu-header > h6{
      color:#f5f8fa; }
  .bp3-menu-header:first-of-type > h6{
    padding-top:0; }
  .bp3-large .bp3-menu-header > h6{
    padding-top:15px;
    padding-bottom:5px;
    font-size:18px; }
  .bp3-large .bp3-menu-header:first-of-type > h6{
    padding-top:0; }

.bp3-dark .bp3-menu{
  background:#30404d;
  color:#f5f8fa; }

.bp3-dark .bp3-menu-item.bp3-intent-primary{
  color:#48aff0; }
  .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-icon{
    color:inherit; }
  .bp3-dark .bp3-menu-item.bp3-intent-primary::before, .bp3-dark .bp3-menu-item.bp3-intent-primary::after,
  .bp3-dark .bp3-menu-item.bp3-intent-primary .bp3-menu-item-label{
    color:#48aff0; }
  .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active{
    background-color:#137cbd; }
  .bp3-dark .bp3-menu-item.bp3-intent-primary:active{
    background-color:#106ba3; }
  .bp3-dark .bp3-menu-item.bp3-intent-primary:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item::after,
  .bp3-dark .bp3-menu-item.bp3-intent-primary:hover .bp3-menu-item-label,
  .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label,
  .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-primary.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary:active, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary:active::after,
  .bp3-dark .bp3-menu-item.bp3-intent-primary:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active::after,
  .bp3-dark .bp3-menu-item.bp3-intent-primary.bp3-active .bp3-menu-item-label{
    color:#ffffff; }

.bp3-dark .bp3-menu-item.bp3-intent-success{
  color:#3dcc91; }
  .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-icon{
    color:inherit; }
  .bp3-dark .bp3-menu-item.bp3-intent-success::before, .bp3-dark .bp3-menu-item.bp3-intent-success::after,
  .bp3-dark .bp3-menu-item.bp3-intent-success .bp3-menu-item-label{
    color:#3dcc91; }
  .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active{
    background-color:#0f9960; }
  .bp3-dark .bp3-menu-item.bp3-intent-success:active{
    background-color:#0d8050; }
  .bp3-dark .bp3-menu-item.bp3-intent-success:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-success:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item::after,
  .bp3-dark .bp3-menu-item.bp3-intent-success:hover .bp3-menu-item-label,
  .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label,
  .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-success.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success:active, .bp3-dark .bp3-menu-item.bp3-intent-success:active::before, .bp3-dark .bp3-menu-item.bp3-intent-success:active::after,
  .bp3-dark .bp3-menu-item.bp3-intent-success:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active::after,
  .bp3-dark .bp3-menu-item.bp3-intent-success.bp3-active .bp3-menu-item-label{
    color:#ffffff; }

.bp3-dark .bp3-menu-item.bp3-intent-warning{
  color:#ffb366; }
  .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-icon{
    color:inherit; }
  .bp3-dark .bp3-menu-item.bp3-intent-warning::before, .bp3-dark .bp3-menu-item.bp3-intent-warning::after,
  .bp3-dark .bp3-menu-item.bp3-intent-warning .bp3-menu-item-label{
    color:#ffb366; }
  .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active{
    background-color:#d9822b; }
  .bp3-dark .bp3-menu-item.bp3-intent-warning:active{
    background-color:#bf7326; }
  .bp3-dark .bp3-menu-item.bp3-intent-warning:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item::after,
  .bp3-dark .bp3-menu-item.bp3-intent-warning:hover .bp3-menu-item-label,
  .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label,
  .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-warning.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning:active, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning:active::after,
  .bp3-dark .bp3-menu-item.bp3-intent-warning:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active::after,
  .bp3-dark .bp3-menu-item.bp3-intent-warning.bp3-active .bp3-menu-item-label{
    color:#ffffff; }

.bp3-dark .bp3-menu-item.bp3-intent-danger{
  color:#ff7373; }
  .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-icon{
    color:inherit; }
  .bp3-dark .bp3-menu-item.bp3-intent-danger::before, .bp3-dark .bp3-menu-item.bp3-intent-danger::after,
  .bp3-dark .bp3-menu-item.bp3-intent-danger .bp3-menu-item-label{
    color:#ff7373; }
  .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active{
    background-color:#db3737; }
  .bp3-dark .bp3-menu-item.bp3-intent-danger:active{
    background-color:#c23030; }
  .bp3-dark .bp3-menu-item.bp3-intent-danger:hover, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::before, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:hover::after, .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after, .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item::after,
  .bp3-dark .bp3-menu-item.bp3-intent-danger:hover .bp3-menu-item-label,
  .bp3-dark .bp3-submenu .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label,
  .bp3-submenu .bp3-dark .bp3-popover-target.bp3-popover-open > .bp3-intent-danger.bp3-menu-item .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger:active, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger:active::after,
  .bp3-dark .bp3-menu-item.bp3-intent-danger:active .bp3-menu-item-label, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::before, .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active::after,
  .bp3-dark .bp3-menu-item.bp3-intent-danger.bp3-active .bp3-menu-item-label{
    color:#ffffff; }

.bp3-dark .bp3-menu-item::before,
.bp3-dark .bp3-menu-item > .bp3-icon{
  color:#a7b6c2; }

.bp3-dark .bp3-menu-item .bp3-menu-item-label{
  color:#a7b6c2; }

.bp3-dark .bp3-menu-item.bp3-active, .bp3-dark .bp3-menu-item:active{
  background-color:rgba(138, 155, 168, 0.3); }

.bp3-dark .bp3-menu-item.bp3-disabled{
  color:rgba(167, 182, 194, 0.6) !important; }
  .bp3-dark .bp3-menu-item.bp3-disabled::before,
  .bp3-dark .bp3-menu-item.bp3-disabled > .bp3-icon,
  .bp3-dark .bp3-menu-item.bp3-disabled .bp3-menu-item-label{
    color:rgba(167, 182, 194, 0.6) !important; }

.bp3-dark .bp3-menu-divider,
.bp3-dark .bp3-menu-header{
  border-color:rgba(255, 255, 255, 0.15); }

.bp3-dark .bp3-menu-header > h6{
  color:#f5f8fa; }

.bp3-label .bp3-menu{
  margin-top:5px; }
.bp3-navbar{
  position:relative;
  z-index:10;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.2);
  background-color:#ffffff;
  width:100%;
  height:50px;
  padding:0 15px; }
  .bp3-navbar.bp3-dark,
  .bp3-dark .bp3-navbar{
    background-color:#394b59; }
  .bp3-navbar.bp3-dark{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-dark .bp3-navbar{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 0 0 rgba(16, 22, 26, 0), 0 1px 1px rgba(16, 22, 26, 0.4); }
  .bp3-navbar.bp3-fixed-top{
    position:fixed;
    top:0;
    right:0;
    left:0; }

.bp3-navbar-heading{
  margin-right:15px;
  font-size:16px; }

.bp3-navbar-group{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  height:50px; }
  .bp3-navbar-group.bp3-align-left{
    float:left; }
  .bp3-navbar-group.bp3-align-right{
    float:right; }

.bp3-navbar-divider{
  margin:0 10px;
  border-left:1px solid rgba(16, 22, 26, 0.15);
  height:20px; }
  .bp3-dark .bp3-navbar-divider{
    border-left-color:rgba(255, 255, 255, 0.15); }
.bp3-non-ideal-state{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  width:100%;
  height:100%;
  text-align:center; }
  .bp3-non-ideal-state > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-non-ideal-state > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-non-ideal-state::before,
  .bp3-non-ideal-state > *{
    margin-bottom:20px; }
  .bp3-non-ideal-state:empty::before,
  .bp3-non-ideal-state > :last-child{
    margin-bottom:0; }
  .bp3-non-ideal-state > *{
    max-width:400px; }

.bp3-non-ideal-state-visual{
  color:rgba(92, 112, 128, 0.6);
  font-size:60px; }
  .bp3-dark .bp3-non-ideal-state-visual{
    color:rgba(167, 182, 194, 0.6); }

.bp3-overflow-list{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-wrap:nowrap;
      flex-wrap:nowrap;
  min-width:0; }

.bp3-overflow-list-spacer{
  -ms-flex-negative:1;
      flex-shrink:1;
  width:1px; }

body.bp3-overlay-open{
  overflow:hidden; }

.bp3-overlay{
  position:static;
  top:0;
  right:0;
  bottom:0;
  left:0;
  z-index:20; }
  .bp3-overlay:not(.bp3-overlay-open){
    pointer-events:none; }
  .bp3-overlay.bp3-overlay-container{
    position:fixed;
    overflow:hidden; }
    .bp3-overlay.bp3-overlay-container.bp3-overlay-inline{
      position:absolute; }
  .bp3-overlay.bp3-overlay-scroll-container{
    position:fixed;
    overflow:auto; }
    .bp3-overlay.bp3-overlay-scroll-container.bp3-overlay-inline{
      position:absolute; }
  .bp3-overlay.bp3-overlay-inline{
    display:inline;
    overflow:visible; }

.bp3-overlay-content{
  position:fixed;
  z-index:20; }
  .bp3-overlay-inline .bp3-overlay-content,
  .bp3-overlay-scroll-container .bp3-overlay-content{
    position:absolute; }

.bp3-overlay-backdrop{
  position:fixed;
  top:0;
  right:0;
  bottom:0;
  left:0;
  opacity:1;
  z-index:20;
  background-color:rgba(16, 22, 26, 0.7);
  overflow:auto;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-overlay-backdrop.bp3-overlay-enter, .bp3-overlay-backdrop.bp3-overlay-appear{
    opacity:0; }
  .bp3-overlay-backdrop.bp3-overlay-enter-active, .bp3-overlay-backdrop.bp3-overlay-appear-active{
    opacity:1;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-overlay-backdrop.bp3-overlay-exit{
    opacity:1; }
  .bp3-overlay-backdrop.bp3-overlay-exit-active{
    opacity:0;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-overlay-backdrop:focus{
    outline:none; }
  .bp3-overlay-inline .bp3-overlay-backdrop{
    position:absolute; }
.bp3-panel-stack{
  position:relative;
  overflow:hidden; }

.bp3-panel-stack-header{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -ms-flex-negative:0;
      flex-shrink:0;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  z-index:1;
  -webkit-box-shadow:0 1px rgba(16, 22, 26, 0.15);
          box-shadow:0 1px rgba(16, 22, 26, 0.15);
  height:30px; }
  .bp3-dark .bp3-panel-stack-header{
    -webkit-box-shadow:0 1px rgba(255, 255, 255, 0.15);
            box-shadow:0 1px rgba(255, 255, 255, 0.15); }
  .bp3-panel-stack-header > span{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-flex:1;
        -ms-flex:1;
            flex:1;
    -webkit-box-align:stretch;
        -ms-flex-align:stretch;
            align-items:stretch; }
  .bp3-panel-stack-header .bp3-heading{
    margin:0 5px; }

.bp3-button.bp3-panel-stack-header-back{
  margin-left:5px;
  padding-left:0;
  white-space:nowrap; }
  .bp3-button.bp3-panel-stack-header-back .bp3-icon{
    margin:0 2px; }

.bp3-panel-stack-view{
  position:absolute;
  top:0;
  right:0;
  bottom:0;
  left:0;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  margin-right:-1px;
  border-right:1px solid rgba(16, 22, 26, 0.15);
  background-color:#ffffff;
  overflow-y:auto; }
  .bp3-dark .bp3-panel-stack-view{
    background-color:#30404d; }

.bp3-panel-stack-push .bp3-panel-stack-enter, .bp3-panel-stack-push .bp3-panel-stack-appear{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0; }

.bp3-panel-stack-push .bp3-panel-stack-enter-active, .bp3-panel-stack-push .bp3-panel-stack-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease;
  -webkit-transition-delay:0;
          transition-delay:0; }

.bp3-panel-stack-push .bp3-panel-stack-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack-push .bp3-panel-stack-exit-active{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease;
  -webkit-transition-delay:0;
          transition-delay:0; }

.bp3-panel-stack-pop .bp3-panel-stack-enter, .bp3-panel-stack-pop .bp3-panel-stack-appear{
  -webkit-transform:translateX(-50%);
          transform:translateX(-50%);
  opacity:0; }

.bp3-panel-stack-pop .bp3-panel-stack-enter-active, .bp3-panel-stack-pop .bp3-panel-stack-appear-active{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease;
  -webkit-transition-delay:0;
          transition-delay:0; }

.bp3-panel-stack-pop .bp3-panel-stack-exit{
  -webkit-transform:translate(0%);
          transform:translate(0%);
  opacity:1; }

.bp3-panel-stack-pop .bp3-panel-stack-exit-active{
  -webkit-transform:translateX(100%);
          transform:translateX(100%);
  opacity:0;
  -webkit-transition-property:opacity, -webkit-transform;
  transition-property:opacity, -webkit-transform;
  transition-property:transform, opacity;
  transition-property:transform, opacity, -webkit-transform;
  -webkit-transition-duration:400ms;
          transition-duration:400ms;
  -webkit-transition-timing-function:ease;
          transition-timing-function:ease;
  -webkit-transition-delay:0;
          transition-delay:0; }
.bp3-popover{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  -webkit-transform:scale(1);
          transform:scale(1);
  display:inline-block;
  z-index:20;
  border-radius:3px; }
  .bp3-popover .bp3-popover-arrow{
    position:absolute;
    width:30px;
    height:30px; }
    .bp3-popover .bp3-popover-arrow::before{
      margin:5px;
      width:20px;
      height:20px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover{
    margin-top:-17px;
    margin-bottom:17px; }
    .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
      bottom:-11px; }
      .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(-90deg);
                transform:rotate(-90deg); }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover{
    margin-left:17px; }
    .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
      left:-11px; }
      .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(0);
                transform:rotate(0); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover{
    margin-top:17px; }
    .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
      top:-11px; }
      .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(90deg);
                transform:rotate(90deg); }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover{
    margin-right:17px;
    margin-left:-17px; }
    .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
      right:-11px; }
      .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow svg{
        -webkit-transform:rotate(180deg);
                transform:rotate(180deg); }
  .bp3-tether-element-attached-middle > .bp3-popover > .bp3-popover-arrow{
    top:50%;
    -webkit-transform:translateY(-50%);
            transform:translateY(-50%); }
  .bp3-tether-element-attached-center > .bp3-popover > .bp3-popover-arrow{
    right:50%;
    -webkit-transform:translateX(50%);
            transform:translateX(50%); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-popover > .bp3-popover-arrow{
    top:-0.3934px; }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-popover > .bp3-popover-arrow{
    right:-0.3934px; }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-popover > .bp3-popover-arrow{
    left:-0.3934px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-popover > .bp3-popover-arrow{
    bottom:-0.3934px; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:top left;
            transform-origin:top left; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:top center;
            transform-origin:top center; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:top right;
            transform-origin:top right; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:center left;
            transform-origin:center left; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:center center;
            transform-origin:center center; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:center right;
            transform-origin:center right; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-popover{
    -webkit-transform-origin:bottom left;
            transform-origin:bottom left; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-popover{
    -webkit-transform-origin:bottom center;
            transform-origin:bottom center; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-popover{
    -webkit-transform-origin:bottom right;
            transform-origin:bottom right; }
  .bp3-popover .bp3-popover-content{
    background:#ffffff;
    color:inherit; }
  .bp3-popover .bp3-popover-arrow::before{
    -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
            box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
  .bp3-popover .bp3-popover-arrow-border{
    fill:#10161a;
    fill-opacity:0.1; }
  .bp3-popover .bp3-popover-arrow-fill{
    fill:#ffffff; }
  .bp3-popover-enter > .bp3-popover, .bp3-popover-appear > .bp3-popover{
    -webkit-transform:scale(0.3);
            transform:scale(0.3); }
  .bp3-popover-enter-active > .bp3-popover, .bp3-popover-appear-active > .bp3-popover{
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-popover-exit > .bp3-popover{
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-popover-exit-active > .bp3-popover{
    -webkit-transform:scale(0.3);
            transform:scale(0.3);
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-popover .bp3-popover-content{
    position:relative;
    border-radius:3px; }
  .bp3-popover.bp3-popover-content-sizing .bp3-popover-content{
    max-width:350px;
    padding:20px; }
  .bp3-popover-target + .bp3-overlay .bp3-popover.bp3-popover-content-sizing{
    width:350px; }
  .bp3-popover.bp3-minimal{
    margin:0 !important; }
    .bp3-popover.bp3-minimal .bp3-popover-arrow{
      display:none; }
    .bp3-popover.bp3-minimal.bp3-popover{
      -webkit-transform:scale(1);
              transform:scale(1); }
      .bp3-popover-enter > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1); }
      .bp3-popover-enter-active > .bp3-popover.bp3-minimal.bp3-popover, .bp3-popover-appear-active > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1);
        -webkit-transition-property:-webkit-transform;
        transition-property:-webkit-transform;
        transition-property:transform;
        transition-property:transform, -webkit-transform;
        -webkit-transition-duration:100ms;
                transition-duration:100ms;
        -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
                transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
        -webkit-transition-delay:0;
                transition-delay:0; }
      .bp3-popover-exit > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1); }
      .bp3-popover-exit-active > .bp3-popover.bp3-minimal.bp3-popover{
        -webkit-transform:scale(1);
                transform:scale(1);
        -webkit-transition-property:-webkit-transform;
        transition-property:-webkit-transform;
        transition-property:transform;
        transition-property:transform, -webkit-transform;
        -webkit-transition-duration:100ms;
                transition-duration:100ms;
        -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
                transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
        -webkit-transition-delay:0;
                transition-delay:0; }
  .bp3-popover.bp3-dark,
  .bp3-dark .bp3-popover{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-popover.bp3-dark .bp3-popover-content,
    .bp3-dark .bp3-popover .bp3-popover-content{
      background:#30404d;
      color:inherit; }
    .bp3-popover.bp3-dark .bp3-popover-arrow::before,
    .bp3-dark .bp3-popover .bp3-popover-arrow::before{
      -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
              box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
    .bp3-popover.bp3-dark .bp3-popover-arrow-border,
    .bp3-dark .bp3-popover .bp3-popover-arrow-border{
      fill:#10161a;
      fill-opacity:0.2; }
    .bp3-popover.bp3-dark .bp3-popover-arrow-fill,
    .bp3-dark .bp3-popover .bp3-popover-arrow-fill{
      fill:#30404d; }

.bp3-popover-arrow::before{
  display:block;
  position:absolute;
  -webkit-transform:rotate(45deg);
          transform:rotate(45deg);
  border-radius:2px;
  content:""; }

.bp3-tether-pinned .bp3-popover-arrow{
  display:none; }

.bp3-popover-backdrop{
  background:rgba(255, 255, 255, 0); }

.bp3-transition-container{
  opacity:1;
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  z-index:20; }
  .bp3-transition-container.bp3-popover-enter, .bp3-transition-container.bp3-popover-appear{
    opacity:0; }
  .bp3-transition-container.bp3-popover-enter-active, .bp3-transition-container.bp3-popover-appear-active{
    opacity:1;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-transition-container.bp3-popover-exit{
    opacity:1; }
  .bp3-transition-container.bp3-popover-exit-active{
    opacity:0;
    -webkit-transition-property:opacity;
    transition-property:opacity;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-transition-container:focus{
    outline:none; }
  .bp3-transition-container.bp3-popover-leave .bp3-popover-content{
    pointer-events:none; }
  .bp3-transition-container[data-x-out-of-boundaries]{
    display:none; }

span.bp3-popover-target{
  display:inline-block; }

.bp3-popover-wrapper.bp3-fill{
  width:100%; }

.bp3-portal{
  position:absolute;
  top:0;
  right:0;
  left:0; }
@-webkit-keyframes linear-progress-bar-stripes{
  from{
    background-position:0 0; }
  to{
    background-position:30px 0; } }
@keyframes linear-progress-bar-stripes{
  from{
    background-position:0 0; }
  to{
    background-position:30px 0; } }

.bp3-progress-bar{
  display:block;
  position:relative;
  border-radius:40px;
  background:rgba(92, 112, 128, 0.2);
  width:100%;
  height:8px;
  overflow:hidden; }
  .bp3-progress-bar .bp3-progress-meter{
    position:absolute;
    border-radius:40px;
    background:linear-gradient(-45deg, rgba(255, 255, 255, 0.2) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.2) 50%, rgba(255, 255, 255, 0.2) 75%, transparent 75%);
    background-color:rgba(92, 112, 128, 0.8);
    background-size:30px 30px;
    width:100%;
    height:100%;
    -webkit-transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:width 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-progress-bar:not(.bp3-no-animation):not(.bp3-no-stripes) .bp3-progress-meter{
    animation:linear-progress-bar-stripes 300ms linear infinite reverse; }
  .bp3-progress-bar.bp3-no-stripes .bp3-progress-meter{
    background-image:none; }

.bp3-dark .bp3-progress-bar{
  background:rgba(16, 22, 26, 0.5); }
  .bp3-dark .bp3-progress-bar .bp3-progress-meter{
    background-color:#8a9ba8; }

.bp3-progress-bar.bp3-intent-primary .bp3-progress-meter{
  background-color:#137cbd; }

.bp3-progress-bar.bp3-intent-success .bp3-progress-meter{
  background-color:#0f9960; }

.bp3-progress-bar.bp3-intent-warning .bp3-progress-meter{
  background-color:#d9822b; }

.bp3-progress-bar.bp3-intent-danger .bp3-progress-meter{
  background-color:#db3737; }
@-webkit-keyframes skeleton-glow{
  from{
    border-color:rgba(206, 217, 224, 0.2);
    background:rgba(206, 217, 224, 0.2); }
  to{
    border-color:rgba(92, 112, 128, 0.2);
    background:rgba(92, 112, 128, 0.2); } }
@keyframes skeleton-glow{
  from{
    border-color:rgba(206, 217, 224, 0.2);
    background:rgba(206, 217, 224, 0.2); }
  to{
    border-color:rgba(92, 112, 128, 0.2);
    background:rgba(92, 112, 128, 0.2); } }
.bp3-skeleton{
  border-color:rgba(206, 217, 224, 0.2) !important;
  border-radius:2px;
  -webkit-box-shadow:none !important;
          box-shadow:none !important;
  background:rgba(206, 217, 224, 0.2);
  background-clip:padding-box !important;
  cursor:default;
  color:transparent !important;
  -webkit-animation:1000ms linear infinite alternate skeleton-glow;
          animation:1000ms linear infinite alternate skeleton-glow;
  pointer-events:none;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-skeleton::before, .bp3-skeleton::after,
  .bp3-skeleton *{
    visibility:hidden !important; }
.bp3-slider{
  width:100%;
  min-width:150px;
  height:40px;
  position:relative;
  outline:none;
  cursor:default;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-slider:hover{
    cursor:pointer; }
  .bp3-slider:active{
    cursor:-webkit-grabbing;
    cursor:grabbing; }
  .bp3-slider.bp3-disabled{
    opacity:0.5;
    cursor:not-allowed; }
  .bp3-slider.bp3-slider-unlabeled{
    height:16px; }

.bp3-slider-track,
.bp3-slider-progress{
  top:5px;
  right:0;
  left:0;
  height:6px;
  position:absolute; }

.bp3-slider-track{
  border-radius:3px;
  overflow:hidden; }

.bp3-slider-progress{
  background:rgba(92, 112, 128, 0.2); }
  .bp3-dark .bp3-slider-progress{
    background:rgba(16, 22, 26, 0.5); }
  .bp3-slider-progress.bp3-intent-primary{
    background-color:#137cbd; }
  .bp3-slider-progress.bp3-intent-success{
    background-color:#0f9960; }
  .bp3-slider-progress.bp3-intent-warning{
    background-color:#d9822b; }
  .bp3-slider-progress.bp3-intent-danger{
    background-color:#db3737; }

.bp3-slider-handle{
  -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
          box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
  background-color:#f5f8fa;
  background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.8)), to(rgba(255, 255, 255, 0)));
  background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.8), rgba(255, 255, 255, 0));
  color:#182026;
  position:absolute;
  top:0;
  left:0;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
  cursor:pointer;
  width:16px;
  height:16px; }
  .bp3-slider-handle:hover{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    background-clip:padding-box;
    background-color:#ebf1f5; }
  .bp3-slider-handle:active, .bp3-slider-handle.bp3-active{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background-color:#d8e1e8;
    background-image:none; }
  .bp3-slider-handle:disabled, .bp3-slider-handle.bp3-disabled{
    outline:none;
    -webkit-box-shadow:none;
            box-shadow:none;
    background-color:rgba(206, 217, 224, 0.5);
    background-image:none;
    cursor:not-allowed;
    color:rgba(92, 112, 128, 0.6); }
    .bp3-slider-handle:disabled.bp3-active, .bp3-slider-handle:disabled.bp3-active:hover, .bp3-slider-handle.bp3-disabled.bp3-active, .bp3-slider-handle.bp3-disabled.bp3-active:hover{
      background:rgba(206, 217, 224, 0.7); }
  .bp3-slider-handle:focus{
    z-index:1; }
  .bp3-slider-handle:hover{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 -1px 0 rgba(16, 22, 26, 0.1);
    background-clip:padding-box;
    background-color:#ebf1f5;
    z-index:2;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 1px 1px rgba(16, 22, 26, 0.2);
    cursor:-webkit-grab;
    cursor:grab; }
  .bp3-slider-handle.bp3-active{
    -webkit-box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
            box-shadow:inset 0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 2px rgba(16, 22, 26, 0.2);
    background-color:#d8e1e8;
    background-image:none;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), inset 0 1px 1px rgba(16, 22, 26, 0.1);
    cursor:-webkit-grabbing;
    cursor:grabbing; }
  .bp3-disabled .bp3-slider-handle{
    -webkit-box-shadow:none;
            box-shadow:none;
    background:#bfccd6;
    pointer-events:none; }
  .bp3-dark .bp3-slider-handle{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
    background-color:#394b59;
    background-image:-webkit-gradient(linear, left top, left bottom, from(rgba(255, 255, 255, 0.05)), to(rgba(255, 255, 255, 0)));
    background-image:linear-gradient(to bottom, rgba(255, 255, 255, 0.05), rgba(255, 255, 255, 0));
    color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle:hover, .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
      color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle:hover{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.4);
      background-color:#30404d; }
    .bp3-dark .bp3-slider-handle:active, .bp3-dark .bp3-slider-handle.bp3-active{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.6), inset 0 1px 2px rgba(16, 22, 26, 0.2);
      background-color:#202b33;
      background-image:none; }
    .bp3-dark .bp3-slider-handle:disabled, .bp3-dark .bp3-slider-handle.bp3-disabled{
      -webkit-box-shadow:none;
              box-shadow:none;
      background-color:rgba(57, 75, 89, 0.5);
      background-image:none;
      color:rgba(167, 182, 194, 0.6); }
      .bp3-dark .bp3-slider-handle:disabled.bp3-active, .bp3-dark .bp3-slider-handle.bp3-disabled.bp3-active{
        background:rgba(57, 75, 89, 0.7); }
    .bp3-dark .bp3-slider-handle .bp3-button-spinner .bp3-spinner-head{
      background:rgba(16, 22, 26, 0.5);
      stroke:#8a9ba8; }
    .bp3-dark .bp3-slider-handle, .bp3-dark .bp3-slider-handle:hover{
      background-color:#394b59; }
    .bp3-dark .bp3-slider-handle.bp3-active{
      background-color:#293742; }
  .bp3-dark .bp3-disabled .bp3-slider-handle{
    border-color:#5c7080;
    -webkit-box-shadow:none;
            box-shadow:none;
    background:#5c7080; }
  .bp3-slider-handle .bp3-slider-label{
    margin-left:8px;
    border-radius:3px;
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
    background:#394b59;
    color:#f5f8fa; }
    .bp3-dark .bp3-slider-handle .bp3-slider-label{
      -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
      background:#e1e8ed;
      color:#394b59; }
    .bp3-disabled .bp3-slider-handle .bp3-slider-label{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-slider-handle.bp3-start, .bp3-slider-handle.bp3-end{
    width:8px; }
  .bp3-slider-handle.bp3-start{
    border-top-right-radius:0;
    border-bottom-right-radius:0; }
  .bp3-slider-handle.bp3-end{
    margin-left:8px;
    border-top-left-radius:0;
    border-bottom-left-radius:0; }
    .bp3-slider-handle.bp3-end .bp3-slider-label{
      margin-left:0; }

.bp3-slider-label{
  -webkit-transform:translate(-50%, 20px);
          transform:translate(-50%, 20px);
  display:inline-block;
  position:absolute;
  padding:2px 5px;
  vertical-align:top;
  line-height:1;
  font-size:12px; }

.bp3-slider.bp3-vertical{
  width:40px;
  min-width:40px;
  height:150px; }
  .bp3-slider.bp3-vertical .bp3-slider-track,
  .bp3-slider.bp3-vertical .bp3-slider-progress{
    top:0;
    bottom:0;
    left:5px;
    width:6px;
    height:auto; }
  .bp3-slider.bp3-vertical .bp3-slider-progress{
    top:auto; }
  .bp3-slider.bp3-vertical .bp3-slider-label{
    -webkit-transform:translate(20px, 50%);
            transform:translate(20px, 50%); }
  .bp3-slider.bp3-vertical .bp3-slider-handle{
    top:auto; }
    .bp3-slider.bp3-vertical .bp3-slider-handle .bp3-slider-label{
      margin-top:-8px;
      margin-left:0; }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end, .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
      margin-left:0;
      width:16px;
      height:8px; }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start{
      border-top-left-radius:0;
      border-bottom-right-radius:3px; }
      .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-start .bp3-slider-label{
        -webkit-transform:translate(20px);
                transform:translate(20px); }
    .bp3-slider.bp3-vertical .bp3-slider-handle.bp3-end{
      margin-bottom:8px;
      border-top-left-radius:3px;
      border-bottom-left-radius:0;
      border-bottom-right-radius:0; }

@-webkit-keyframes pt-spinner-animation{
  from{
    -webkit-transform:rotate(0deg);
            transform:rotate(0deg); }
  to{
    -webkit-transform:rotate(360deg);
            transform:rotate(360deg); } }

@keyframes pt-spinner-animation{
  from{
    -webkit-transform:rotate(0deg);
            transform:rotate(0deg); }
  to{
    -webkit-transform:rotate(360deg);
            transform:rotate(360deg); } }

.bp3-spinner{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  -webkit-box-pack:center;
      -ms-flex-pack:center;
          justify-content:center;
  overflow:visible;
  vertical-align:middle; }
  .bp3-spinner svg{
    display:block; }
  .bp3-spinner path{
    fill-opacity:0; }
  .bp3-spinner .bp3-spinner-head{
    -webkit-transform-origin:center;
            transform-origin:center;
    -webkit-transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    transition:stroke-dashoffset 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
    stroke:rgba(92, 112, 128, 0.8);
    stroke-linecap:round; }
  .bp3-spinner .bp3-spinner-track{
    stroke:rgba(92, 112, 128, 0.2); }

.bp3-spinner-animation{
  -webkit-animation:pt-spinner-animation 500ms linear infinite;
          animation:pt-spinner-animation 500ms linear infinite; }
  .bp3-no-spin > .bp3-spinner-animation{
    -webkit-animation:none;
            animation:none; }

.bp3-dark .bp3-spinner .bp3-spinner-head{
  stroke:#8a9ba8; }

.bp3-dark .bp3-spinner .bp3-spinner-track{
  stroke:rgba(16, 22, 26, 0.5); }

.bp3-spinner.bp3-intent-primary .bp3-spinner-head{
  stroke:#137cbd; }

.bp3-spinner.bp3-intent-success .bp3-spinner-head{
  stroke:#0f9960; }

.bp3-spinner.bp3-intent-warning .bp3-spinner-head{
  stroke:#d9822b; }

.bp3-spinner.bp3-intent-danger .bp3-spinner-head{
  stroke:#db3737; }
.bp3-tabs.bp3-vertical{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex; }
  .bp3-tabs.bp3-vertical > .bp3-tab-list{
    -webkit-box-orient:vertical;
    -webkit-box-direction:normal;
        -ms-flex-direction:column;
            flex-direction:column;
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start; }
    .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab{
      border-radius:3px;
      width:100%;
      padding:0 10px; }
      .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab[aria-selected="true"]{
        -webkit-box-shadow:none;
                box-shadow:none;
        background-color:rgba(19, 124, 189, 0.2); }
    .bp3-tabs.bp3-vertical > .bp3-tab-list .bp3-tab-indicator-wrapper .bp3-tab-indicator{
      top:0;
      right:0;
      bottom:0;
      left:0;
      border-radius:3px;
      background-color:rgba(19, 124, 189, 0.2);
      height:auto; }
  .bp3-tabs.bp3-vertical > .bp3-tab-panel{
    margin-top:0;
    padding-left:20px; }

.bp3-tab-list{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  -webkit-box-align:end;
      -ms-flex-align:end;
          align-items:flex-end;
  position:relative;
  margin:0;
  border:none;
  padding:0;
  list-style:none; }
  .bp3-tab-list > *:not(:last-child){
    margin-right:20px; }

.bp3-tab{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  -webkit-box-flex:0;
      -ms-flex:0 0 auto;
          flex:0 0 auto;
  position:relative;
  cursor:pointer;
  max-width:100%;
  vertical-align:top;
  line-height:30px;
  color:#182026;
  font-size:14px; }
  .bp3-tab a{
    display:block;
    text-decoration:none;
    color:inherit; }
  .bp3-tab-indicator-wrapper ~ .bp3-tab{
    -webkit-box-shadow:none !important;
            box-shadow:none !important;
    background-color:transparent !important; }
  .bp3-tab[aria-disabled="true"]{
    cursor:not-allowed;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-tab[aria-selected="true"]{
    border-radius:0;
    -webkit-box-shadow:inset 0 -3px 0 #106ba3;
            box-shadow:inset 0 -3px 0 #106ba3; }
  .bp3-tab[aria-selected="true"], .bp3-tab:not([aria-disabled="true"]):hover{
    color:#106ba3; }
  .bp3-tab:focus{
    -moz-outline-radius:0; }
  .bp3-large > .bp3-tab{
    line-height:40px;
    font-size:16px; }

.bp3-tab-panel{
  margin-top:20px; }
  .bp3-tab-panel[aria-hidden="true"]{
    display:none; }

.bp3-tab-indicator-wrapper{
  position:absolute;
  top:0;
  left:0;
  -webkit-transform:translateX(0), translateY(0);
          transform:translateX(0), translateY(0);
  -webkit-transition:height, width, -webkit-transform;
  transition:height, width, -webkit-transform;
  transition:height, transform, width;
  transition:height, transform, width, -webkit-transform;
  -webkit-transition-duration:200ms;
          transition-duration:200ms;
  -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
          transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
  pointer-events:none; }
  .bp3-tab-indicator-wrapper .bp3-tab-indicator{
    position:absolute;
    right:0;
    bottom:0;
    left:0;
    background-color:#106ba3;
    height:3px; }
  .bp3-tab-indicator-wrapper.bp3-no-animation{
    -webkit-transition:none;
    transition:none; }

.bp3-dark .bp3-tab{
  color:#f5f8fa; }
  .bp3-dark .bp3-tab[aria-disabled="true"]{
    color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-tab[aria-selected="true"]{
    -webkit-box-shadow:inset 0 -3px 0 #48aff0;
            box-shadow:inset 0 -3px 0 #48aff0; }
  .bp3-dark .bp3-tab[aria-selected="true"], .bp3-dark .bp3-tab:not([aria-disabled="true"]):hover{
    color:#48aff0; }

.bp3-dark .bp3-tab-indicator{
  background-color:#48aff0; }

.bp3-flex-expander{
  -webkit-box-flex:1;
      -ms-flex:1 1;
          flex:1 1; }
.bp3-tag{
  display:-webkit-inline-box;
  display:-ms-inline-flexbox;
  display:inline-flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  position:relative;
  border:none;
  border-radius:3px;
  -webkit-box-shadow:none;
          box-shadow:none;
  background-color:#5c7080;
  min-width:20px;
  max-width:100%;
  min-height:20px;
  padding:2px 6px;
  line-height:16px;
  color:#f5f8fa;
  font-size:12px; }
  .bp3-tag.bp3-interactive{
    cursor:pointer; }
    .bp3-tag.bp3-interactive:hover{
      background-color:rgba(92, 112, 128, 0.85); }
    .bp3-tag.bp3-interactive.bp3-active, .bp3-tag.bp3-interactive:active{
      background-color:rgba(92, 112, 128, 0.7); }
  .bp3-tag > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-tag > .bp3-fill{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-tag::before,
  .bp3-tag > *{
    margin-right:4px; }
  .bp3-tag:empty::before,
  .bp3-tag > :last-child{
    margin-right:0; }
  .bp3-tag:focus{
    outline:rgba(19, 124, 189, 0.6) auto 2px;
    outline-offset:0;
    -moz-outline-radius:6px; }
  .bp3-tag.bp3-round{
    border-radius:30px;
    padding-right:8px;
    padding-left:8px; }
  .bp3-dark .bp3-tag{
    background-color:#bfccd6;
    color:#182026; }
    .bp3-dark .bp3-tag.bp3-interactive{
      cursor:pointer; }
      .bp3-dark .bp3-tag.bp3-interactive:hover{
        background-color:rgba(191, 204, 214, 0.85); }
      .bp3-dark .bp3-tag.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-interactive:active{
        background-color:rgba(191, 204, 214, 0.7); }
    .bp3-dark .bp3-tag > .bp3-icon, .bp3-dark .bp3-tag .bp3-icon-standard, .bp3-dark .bp3-tag .bp3-icon-large{
      fill:currentColor; }
  .bp3-tag > .bp3-icon, .bp3-tag .bp3-icon-standard, .bp3-tag .bp3-icon-large{
    fill:#ffffff; }
  .bp3-tag.bp3-large,
  .bp3-large .bp3-tag{
    min-width:30px;
    min-height:30px;
    padding:0 10px;
    line-height:20px;
    font-size:14px; }
    .bp3-tag.bp3-large::before,
    .bp3-tag.bp3-large > *,
    .bp3-large .bp3-tag::before,
    .bp3-large .bp3-tag > *{
      margin-right:7px; }
    .bp3-tag.bp3-large:empty::before,
    .bp3-tag.bp3-large > :last-child,
    .bp3-large .bp3-tag:empty::before,
    .bp3-large .bp3-tag > :last-child{
      margin-right:0; }
    .bp3-tag.bp3-large.bp3-round,
    .bp3-large .bp3-tag.bp3-round{
      padding-right:12px;
      padding-left:12px; }
  .bp3-tag.bp3-intent-primary{
    background:#137cbd;
    color:#ffffff; }
    .bp3-tag.bp3-intent-primary.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-primary.bp3-interactive:hover{
        background-color:rgba(19, 124, 189, 0.85); }
      .bp3-tag.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-primary.bp3-interactive:active{
        background-color:rgba(19, 124, 189, 0.7); }
  .bp3-tag.bp3-intent-success{
    background:#0f9960;
    color:#ffffff; }
    .bp3-tag.bp3-intent-success.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-success.bp3-interactive:hover{
        background-color:rgba(15, 153, 96, 0.85); }
      .bp3-tag.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-success.bp3-interactive:active{
        background-color:rgba(15, 153, 96, 0.7); }
  .bp3-tag.bp3-intent-warning{
    background:#d9822b;
    color:#ffffff; }
    .bp3-tag.bp3-intent-warning.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-warning.bp3-interactive:hover{
        background-color:rgba(217, 130, 43, 0.85); }
      .bp3-tag.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-warning.bp3-interactive:active{
        background-color:rgba(217, 130, 43, 0.7); }
  .bp3-tag.bp3-intent-danger{
    background:#db3737;
    color:#ffffff; }
    .bp3-tag.bp3-intent-danger.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-intent-danger.bp3-interactive:hover{
        background-color:rgba(219, 55, 55, 0.85); }
      .bp3-tag.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-intent-danger.bp3-interactive:active{
        background-color:rgba(219, 55, 55, 0.7); }
  .bp3-tag.bp3-fill{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    width:100%; }
  .bp3-tag.bp3-minimal > .bp3-icon, .bp3-tag.bp3-minimal .bp3-icon-standard, .bp3-tag.bp3-minimal .bp3-icon-large{
    fill:#5c7080; }
  .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]){
    background-color:rgba(138, 155, 168, 0.2);
    color:#182026; }
    .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:hover{
        background-color:rgba(92, 112, 128, 0.3); }
      .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:active{
        background-color:rgba(92, 112, 128, 0.4); }
    .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]){
      color:#f5f8fa; }
      .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:hover{
          background-color:rgba(191, 204, 214, 0.3); }
        .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]).bp3-interactive:active{
          background-color:rgba(191, 204, 214, 0.4); }
      .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) > .bp3-icon, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) .bp3-icon-standard, .bp3-dark .bp3-tag.bp3-minimal:not([class*="bp3-intent-"]) .bp3-icon-large{
        fill:#a7b6c2; }
  .bp3-tag.bp3-minimal.bp3-intent-primary{
    background-color:rgba(19, 124, 189, 0.15);
    color:#106ba3; }
    .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
        background-color:rgba(19, 124, 189, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
        background-color:rgba(19, 124, 189, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-primary > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-primary .bp3-icon-large{
      fill:#137cbd; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary{
      background-color:rgba(19, 124, 189, 0.25);
      color:#48aff0; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:hover{
          background-color:rgba(19, 124, 189, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-primary.bp3-interactive:active{
          background-color:rgba(19, 124, 189, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-success{
    background-color:rgba(15, 153, 96, 0.15);
    color:#0d8050; }
    .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
        background-color:rgba(15, 153, 96, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
        background-color:rgba(15, 153, 96, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-success > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-success .bp3-icon-large{
      fill:#0f9960; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success{
      background-color:rgba(15, 153, 96, 0.25);
      color:#3dcc91; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:hover{
          background-color:rgba(15, 153, 96, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-success.bp3-interactive:active{
          background-color:rgba(15, 153, 96, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-warning{
    background-color:rgba(217, 130, 43, 0.15);
    color:#bf7326; }
    .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
        background-color:rgba(217, 130, 43, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
        background-color:rgba(217, 130, 43, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-warning > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-warning .bp3-icon-large{
      fill:#d9822b; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning{
      background-color:rgba(217, 130, 43, 0.25);
      color:#ffb366; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:hover{
          background-color:rgba(217, 130, 43, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-warning.bp3-interactive:active{
          background-color:rgba(217, 130, 43, 0.45); }
  .bp3-tag.bp3-minimal.bp3-intent-danger{
    background-color:rgba(219, 55, 55, 0.15);
    color:#c23030; }
    .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
      cursor:pointer; }
      .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
        background-color:rgba(219, 55, 55, 0.25); }
      .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
        background-color:rgba(219, 55, 55, 0.35); }
    .bp3-tag.bp3-minimal.bp3-intent-danger > .bp3-icon, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-standard, .bp3-tag.bp3-minimal.bp3-intent-danger .bp3-icon-large{
      fill:#db3737; }
    .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger{
      background-color:rgba(219, 55, 55, 0.25);
      color:#ff7373; }
      .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive{
        cursor:pointer; }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:hover{
          background-color:rgba(219, 55, 55, 0.35); }
        .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive.bp3-active, .bp3-dark .bp3-tag.bp3-minimal.bp3-intent-danger.bp3-interactive:active{
          background-color:rgba(219, 55, 55, 0.45); }

.bp3-tag-remove{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  opacity:0.5;
  margin-top:-2px;
  margin-right:-6px !important;
  margin-bottom:-2px;
  border:none;
  background:none;
  cursor:pointer;
  padding:2px;
  padding-left:0;
  color:inherit; }
  .bp3-tag-remove:hover{
    opacity:0.8;
    background:none;
    text-decoration:none; }
  .bp3-tag-remove:active{
    opacity:1; }
  .bp3-tag-remove:empty::before{
    line-height:1;
    font-family:"Icons16", sans-serif;
    font-size:16px;
    font-weight:400;
    font-style:normal;
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased;
    content:""; }
  .bp3-large .bp3-tag-remove{
    margin-right:-10px !important;
    padding:5px;
    padding-left:0; }
    .bp3-large .bp3-tag-remove:empty::before{
      line-height:1;
      font-family:"Icons20", sans-serif;
      font-size:20px;
      font-weight:400;
      font-style:normal; }
.bp3-tag-input{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-orient:horizontal;
  -webkit-box-direction:normal;
      -ms-flex-direction:row;
          flex-direction:row;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  cursor:text;
  height:auto;
  min-height:30px;
  padding-right:0;
  padding-left:5px;
  line-height:inherit; }
  .bp3-tag-input > *{
    -webkit-box-flex:0;
        -ms-flex-positive:0;
            flex-grow:0;
    -ms-flex-negative:0;
        flex-shrink:0; }
  .bp3-tag-input > .bp3-tag-input-values{
    -webkit-box-flex:1;
        -ms-flex-positive:1;
            flex-grow:1;
    -ms-flex-negative:1;
        flex-shrink:1; }
  .bp3-tag-input .bp3-tag-input-icon{
    margin-top:7px;
    margin-right:7px;
    margin-left:2px;
    color:#5c7080; }
  .bp3-tag-input .bp3-tag-input-values{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-orient:horizontal;
    -webkit-box-direction:normal;
        -ms-flex-direction:row;
            flex-direction:row;
    -ms-flex-wrap:wrap;
        flex-wrap:wrap;
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center;
    -ms-flex-item-align:stretch;
        align-self:stretch;
    margin-top:5px;
    margin-right:7px;
    min-width:0; }
    .bp3-tag-input .bp3-tag-input-values > *{
      -webkit-box-flex:0;
          -ms-flex-positive:0;
              flex-grow:0;
      -ms-flex-negative:0;
          flex-shrink:0; }
    .bp3-tag-input .bp3-tag-input-values > .bp3-fill{
      -webkit-box-flex:1;
          -ms-flex-positive:1;
              flex-grow:1;
      -ms-flex-negative:1;
          flex-shrink:1; }
    .bp3-tag-input .bp3-tag-input-values::before,
    .bp3-tag-input .bp3-tag-input-values > *{
      margin-right:5px; }
    .bp3-tag-input .bp3-tag-input-values:empty::before,
    .bp3-tag-input .bp3-tag-input-values > :last-child{
      margin-right:0; }
    .bp3-tag-input .bp3-tag-input-values:first-child .bp3-input-ghost:first-child{
      padding-left:5px; }
    .bp3-tag-input .bp3-tag-input-values > *{
      margin-bottom:5px; }
  .bp3-tag-input .bp3-tag{
    overflow-wrap:break-word; }
    .bp3-tag-input .bp3-tag.bp3-active{
      outline:rgba(19, 124, 189, 0.6) auto 2px;
      outline-offset:0;
      -moz-outline-radius:6px; }
  .bp3-tag-input .bp3-input-ghost{
    -webkit-box-flex:1;
        -ms-flex:1 1 auto;
            flex:1 1 auto;
    width:80px;
    line-height:20px; }
    .bp3-tag-input .bp3-input-ghost:disabled, .bp3-tag-input .bp3-input-ghost.bp3-disabled{
      cursor:not-allowed; }
  .bp3-tag-input .bp3-button,
  .bp3-tag-input .bp3-spinner{
    margin:3px;
    margin-left:0; }
  .bp3-tag-input .bp3-button{
    min-width:24px;
    min-height:24px;
    padding:0 7px; }
  .bp3-tag-input.bp3-large{
    height:auto;
    min-height:40px; }
    .bp3-tag-input.bp3-large::before,
    .bp3-tag-input.bp3-large > *{
      margin-right:10px; }
    .bp3-tag-input.bp3-large:empty::before,
    .bp3-tag-input.bp3-large > :last-child{
      margin-right:0; }
    .bp3-tag-input.bp3-large .bp3-tag-input-icon{
      margin-top:10px;
      margin-left:5px; }
    .bp3-tag-input.bp3-large .bp3-input-ghost{
      line-height:30px; }
    .bp3-tag-input.bp3-large .bp3-button{
      min-width:30px;
      min-height:30px;
      padding:5px 10px;
      margin:5px;
      margin-left:0; }
    .bp3-tag-input.bp3-large .bp3-spinner{
      margin:8px;
      margin-left:0; }
  .bp3-tag-input.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
    background-color:#ffffff; }
    .bp3-tag-input.bp3-active.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-success{
      -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
    .bp3-tag-input.bp3-active.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2);
              box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.2); }
  .bp3-dark .bp3-tag-input .bp3-tag-input-icon, .bp3-tag-input.bp3-dark .bp3-tag-input-icon{
    color:#a7b6c2; }
  .bp3-dark .bp3-tag-input .bp3-input-ghost, .bp3-tag-input.bp3-dark .bp3-input-ghost{
    color:#f5f8fa; }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-webkit-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-webkit-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-moz-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-moz-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost:-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost:-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::-ms-input-placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::-ms-input-placeholder{
      color:rgba(167, 182, 194, 0.6); }
    .bp3-dark .bp3-tag-input .bp3-input-ghost::placeholder, .bp3-tag-input.bp3-dark .bp3-input-ghost::placeholder{
      color:rgba(167, 182, 194, 0.6); }
  .bp3-dark .bp3-tag-input.bp3-active, .bp3-tag-input.bp3-dark.bp3-active{
    -webkit-box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px #137cbd, 0 0 0 1px #137cbd, 0 0 0 3px rgba(19, 124, 189, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
    background-color:rgba(16, 22, 26, 0.3); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-primary, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-primary{
      -webkit-box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #106ba3, 0 0 0 3px rgba(16, 107, 163, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-success, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-success{
      -webkit-box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #0d8050, 0 0 0 3px rgba(13, 128, 80, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-warning, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-warning{
      -webkit-box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #bf7326, 0 0 0 3px rgba(191, 115, 38, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }
    .bp3-dark .bp3-tag-input.bp3-active.bp3-intent-danger, .bp3-tag-input.bp3-dark.bp3-active.bp3-intent-danger{
      -webkit-box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4);
              box-shadow:0 0 0 1px #c23030, 0 0 0 3px rgba(194, 48, 48, 0.3), inset 0 0 0 1px rgba(16, 22, 26, 0.3), inset 0 1px 1px rgba(16, 22, 26, 0.4); }

.bp3-input-ghost{
  border:none;
  -webkit-box-shadow:none;
          box-shadow:none;
  background:none;
  padding:0; }
  .bp3-input-ghost::-webkit-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input-ghost::-moz-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input-ghost:-ms-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input-ghost::-ms-input-placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input-ghost::placeholder{
    opacity:1;
    color:rgba(92, 112, 128, 0.6); }
  .bp3-input-ghost:focus{
    outline:none !important; }
.bp3-toast{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-align:start;
      -ms-flex-align:start;
          align-items:flex-start;
  position:relative !important;
  margin:20px 0 0;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  background-color:#ffffff;
  min-width:300px;
  max-width:500px;
  pointer-events:all; }
  .bp3-toast.bp3-toast-enter, .bp3-toast.bp3-toast-appear{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px); }
  .bp3-toast.bp3-toast-enter-active, .bp3-toast.bp3-toast-appear-active{
    -webkit-transform:translateY(0);
            transform:translateY(0);
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-toast.bp3-toast-enter ~ .bp3-toast, .bp3-toast.bp3-toast-appear ~ .bp3-toast{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px); }
  .bp3-toast.bp3-toast-enter-active ~ .bp3-toast, .bp3-toast.bp3-toast-appear-active ~ .bp3-toast{
    -webkit-transform:translateY(0);
            transform:translateY(0);
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
            transition-timing-function:cubic-bezier(0.54, 1.12, 0.38, 1.11);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-toast.bp3-toast-exit{
    opacity:1;
    -webkit-filter:blur(0);
            filter:blur(0); }
  .bp3-toast.bp3-toast-exit-active{
    opacity:0;
    -webkit-filter:blur(10px);
            filter:blur(10px);
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:opacity, filter;
    transition-property:opacity, filter, -webkit-filter;
    -webkit-transition-duration:300ms;
            transition-duration:300ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-toast.bp3-toast-exit ~ .bp3-toast{
    -webkit-transform:translateY(0);
            transform:translateY(0); }
  .bp3-toast.bp3-toast-exit-active ~ .bp3-toast{
    -webkit-transform:translateY(-40px);
            transform:translateY(-40px);
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:50ms;
            transition-delay:50ms; }
  .bp3-toast .bp3-button-group{
    -webkit-box-flex:0;
        -ms-flex:0 0 auto;
            flex:0 0 auto;
    padding:5px;
    padding-left:0; }
  .bp3-toast > .bp3-icon{
    margin:12px;
    margin-right:0;
    color:#5c7080; }
  .bp3-toast.bp3-dark,
  .bp3-dark .bp3-toast{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
    background-color:#394b59; }
    .bp3-toast.bp3-dark > .bp3-icon,
    .bp3-dark .bp3-toast > .bp3-icon{
      color:#a7b6c2; }
  .bp3-toast[class*="bp3-intent-"] a{
    color:rgba(255, 255, 255, 0.7); }
    .bp3-toast[class*="bp3-intent-"] a:hover{
      color:#ffffff; }
  .bp3-toast[class*="bp3-intent-"] > .bp3-icon{
    color:#ffffff; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button, .bp3-toast[class*="bp3-intent-"] .bp3-button::before,
  .bp3-toast[class*="bp3-intent-"] .bp3-button .bp3-icon, .bp3-toast[class*="bp3-intent-"] .bp3-button:active{
    color:rgba(255, 255, 255, 0.7) !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:focus{
    outline-color:rgba(255, 255, 255, 0.5); }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:hover{
    background-color:rgba(255, 255, 255, 0.15) !important;
    color:#ffffff !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button:active{
    background-color:rgba(255, 255, 255, 0.3) !important;
    color:#ffffff !important; }
  .bp3-toast[class*="bp3-intent-"] .bp3-button::after{
    background:rgba(255, 255, 255, 0.3) !important; }
  .bp3-toast.bp3-intent-primary{
    background-color:#137cbd;
    color:#ffffff; }
  .bp3-toast.bp3-intent-success{
    background-color:#0f9960;
    color:#ffffff; }
  .bp3-toast.bp3-intent-warning{
    background-color:#d9822b;
    color:#ffffff; }
  .bp3-toast.bp3-intent-danger{
    background-color:#db3737;
    color:#ffffff; }

.bp3-toast-message{
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  padding:11px;
  word-break:break-word; }

.bp3-toast-container{
  display:-webkit-box !important;
  display:-ms-flexbox !important;
  display:flex !important;
  -webkit-box-orient:vertical;
  -webkit-box-direction:normal;
      -ms-flex-direction:column;
          flex-direction:column;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  position:fixed;
  right:0;
  left:0;
  z-index:40;
  overflow:hidden;
  padding:0 20px 20px;
  pointer-events:none; }
  .bp3-toast-container.bp3-toast-container-top{
    top:0;
    bottom:auto; }
  .bp3-toast-container.bp3-toast-container-bottom{
    -webkit-box-orient:vertical;
    -webkit-box-direction:reverse;
        -ms-flex-direction:column-reverse;
            flex-direction:column-reverse;
    top:auto;
    bottom:0; }
  .bp3-toast-container.bp3-toast-container-left{
    -webkit-box-align:start;
        -ms-flex-align:start;
            align-items:flex-start; }
  .bp3-toast-container.bp3-toast-container-right{
    -webkit-box-align:end;
        -ms-flex-align:end;
            align-items:flex-end; }

.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-enter:not(.bp3-toast-enter-active) ~ .bp3-toast, .bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active),
.bp3-toast-container-bottom .bp3-toast.bp3-toast-appear:not(.bp3-toast-appear-active) ~ .bp3-toast,
.bp3-toast-container-bottom .bp3-toast.bp3-toast-leave-active ~ .bp3-toast{
  -webkit-transform:translateY(60px);
          transform:translateY(60px); }
.bp3-tooltip{
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 2px 4px rgba(16, 22, 26, 0.2), 0 8px 24px rgba(16, 22, 26, 0.2);
  -webkit-transform:scale(1);
          transform:scale(1); }
  .bp3-tooltip .bp3-popover-arrow{
    position:absolute;
    width:22px;
    height:22px; }
    .bp3-tooltip .bp3-popover-arrow::before{
      margin:4px;
      width:14px;
      height:14px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip{
    margin-top:-11px;
    margin-bottom:11px; }
    .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
      bottom:-8px; }
      .bp3-tether-element-attached-bottom.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(-90deg);
                transform:rotate(-90deg); }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip{
    margin-left:11px; }
    .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
      left:-8px; }
      .bp3-tether-element-attached-left.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(0);
                transform:rotate(0); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip{
    margin-top:11px; }
    .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
      top:-8px; }
      .bp3-tether-element-attached-top.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(90deg);
                transform:rotate(90deg); }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip{
    margin-right:11px;
    margin-left:-11px; }
    .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
      right:-8px; }
      .bp3-tether-element-attached-right.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow svg{
        -webkit-transform:rotate(180deg);
                transform:rotate(180deg); }
  .bp3-tether-element-attached-middle > .bp3-tooltip > .bp3-popover-arrow{
    top:50%;
    -webkit-transform:translateY(-50%);
            transform:translateY(-50%); }
  .bp3-tether-element-attached-center > .bp3-tooltip > .bp3-popover-arrow{
    right:50%;
    -webkit-transform:translateX(50%);
            transform:translateX(50%); }
  .bp3-tether-element-attached-top.bp3-tether-target-attached-top > .bp3-tooltip > .bp3-popover-arrow{
    top:-0.22183px; }
  .bp3-tether-element-attached-right.bp3-tether-target-attached-right > .bp3-tooltip > .bp3-popover-arrow{
    right:-0.22183px; }
  .bp3-tether-element-attached-left.bp3-tether-target-attached-left > .bp3-tooltip > .bp3-popover-arrow{
    left:-0.22183px; }
  .bp3-tether-element-attached-bottom.bp3-tether-target-attached-bottom > .bp3-tooltip > .bp3-popover-arrow{
    bottom:-0.22183px; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:top left;
            transform-origin:top left; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:top center;
            transform-origin:top center; }
  .bp3-tether-element-attached-top.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:top right;
            transform-origin:top right; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:center left;
            transform-origin:center left; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:center center;
            transform-origin:center center; }
  .bp3-tether-element-attached-middle.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:center right;
            transform-origin:center right; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-left > .bp3-tooltip{
    -webkit-transform-origin:bottom left;
            transform-origin:bottom left; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-center > .bp3-tooltip{
    -webkit-transform-origin:bottom center;
            transform-origin:bottom center; }
  .bp3-tether-element-attached-bottom.bp3-tether-element-attached-right > .bp3-tooltip{
    -webkit-transform-origin:bottom right;
            transform-origin:bottom right; }
  .bp3-tooltip .bp3-popover-content{
    background:#394b59;
    color:#f5f8fa; }
  .bp3-tooltip .bp3-popover-arrow::before{
    -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2);
            box-shadow:1px 1px 6px rgba(16, 22, 26, 0.2); }
  .bp3-tooltip .bp3-popover-arrow-border{
    fill:#10161a;
    fill-opacity:0.1; }
  .bp3-tooltip .bp3-popover-arrow-fill{
    fill:#394b59; }
  .bp3-popover-enter > .bp3-tooltip, .bp3-popover-appear > .bp3-tooltip{
    -webkit-transform:scale(0.8);
            transform:scale(0.8); }
  .bp3-popover-enter-active > .bp3-tooltip, .bp3-popover-appear-active > .bp3-tooltip{
    -webkit-transform:scale(1);
            transform:scale(1);
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-popover-exit > .bp3-tooltip{
    -webkit-transform:scale(1);
            transform:scale(1); }
  .bp3-popover-exit-active > .bp3-tooltip{
    -webkit-transform:scale(0.8);
            transform:scale(0.8);
    -webkit-transition-property:-webkit-transform;
    transition-property:-webkit-transform;
    transition-property:transform;
    transition-property:transform, -webkit-transform;
    -webkit-transition-duration:100ms;
            transition-duration:100ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-tooltip .bp3-popover-content{
    padding:10px 12px; }
  .bp3-tooltip.bp3-dark,
  .bp3-dark .bp3-tooltip{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 2px 4px rgba(16, 22, 26, 0.4), 0 8px 24px rgba(16, 22, 26, 0.4); }
    .bp3-tooltip.bp3-dark .bp3-popover-content,
    .bp3-dark .bp3-tooltip .bp3-popover-content{
      background:#e1e8ed;
      color:#394b59; }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow::before,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow::before{
      -webkit-box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4);
              box-shadow:1px 1px 6px rgba(16, 22, 26, 0.4); }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow-border,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow-border{
      fill:#10161a;
      fill-opacity:0.2; }
    .bp3-tooltip.bp3-dark .bp3-popover-arrow-fill,
    .bp3-dark .bp3-tooltip .bp3-popover-arrow-fill{
      fill:#e1e8ed; }
  .bp3-tooltip.bp3-intent-primary .bp3-popover-content{
    background:#137cbd;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-primary .bp3-popover-arrow-fill{
    fill:#137cbd; }
  .bp3-tooltip.bp3-intent-success .bp3-popover-content{
    background:#0f9960;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-success .bp3-popover-arrow-fill{
    fill:#0f9960; }
  .bp3-tooltip.bp3-intent-warning .bp3-popover-content{
    background:#d9822b;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-warning .bp3-popover-arrow-fill{
    fill:#d9822b; }
  .bp3-tooltip.bp3-intent-danger .bp3-popover-content{
    background:#db3737;
    color:#ffffff; }
  .bp3-tooltip.bp3-intent-danger .bp3-popover-arrow-fill{
    fill:#db3737; }

.bp3-tooltip-indicator{
  border-bottom:dotted 1px;
  cursor:help; }
.bp3-tree .bp3-icon, .bp3-tree .bp3-icon-standard, .bp3-tree .bp3-icon-large{
  color:#5c7080; }
  .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-tree .bp3-icon-large.bp3-intent-primary{
    color:#137cbd; }
  .bp3-tree .bp3-icon.bp3-intent-success, .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-tree .bp3-icon-large.bp3-intent-success{
    color:#0f9960; }
  .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-tree .bp3-icon-large.bp3-intent-warning{
    color:#d9822b; }
  .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-tree .bp3-icon-large.bp3-intent-danger{
    color:#db3737; }

.bp3-tree-node-list{
  margin:0;
  padding-left:0;
  list-style:none; }

.bp3-tree-root{
  position:relative;
  background-color:transparent;
  cursor:default;
  padding-left:0; }

.bp3-tree-node-content-0{
  padding-left:0px; }

.bp3-tree-node-content-1{
  padding-left:23px; }

.bp3-tree-node-content-2{
  padding-left:46px; }

.bp3-tree-node-content-3{
  padding-left:69px; }

.bp3-tree-node-content-4{
  padding-left:92px; }

.bp3-tree-node-content-5{
  padding-left:115px; }

.bp3-tree-node-content-6{
  padding-left:138px; }

.bp3-tree-node-content-7{
  padding-left:161px; }

.bp3-tree-node-content-8{
  padding-left:184px; }

.bp3-tree-node-content-9{
  padding-left:207px; }

.bp3-tree-node-content-10{
  padding-left:230px; }

.bp3-tree-node-content-11{
  padding-left:253px; }

.bp3-tree-node-content-12{
  padding-left:276px; }

.bp3-tree-node-content-13{
  padding-left:299px; }

.bp3-tree-node-content-14{
  padding-left:322px; }

.bp3-tree-node-content-15{
  padding-left:345px; }

.bp3-tree-node-content-16{
  padding-left:368px; }

.bp3-tree-node-content-17{
  padding-left:391px; }

.bp3-tree-node-content-18{
  padding-left:414px; }

.bp3-tree-node-content-19{
  padding-left:437px; }

.bp3-tree-node-content-20{
  padding-left:460px; }

.bp3-tree-node-content{
  display:-webkit-box;
  display:-ms-flexbox;
  display:flex;
  -webkit-box-align:center;
      -ms-flex-align:center;
          align-items:center;
  width:100%;
  height:30px;
  padding-right:5px; }
  .bp3-tree-node-content:hover{
    background-color:rgba(191, 204, 214, 0.4); }

.bp3-tree-node-caret,
.bp3-tree-node-caret-none{
  min-width:30px; }

.bp3-tree-node-caret{
  color:#5c7080;
  -webkit-transform:rotate(0deg);
          transform:rotate(0deg);
  cursor:pointer;
  padding:7px;
  -webkit-transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:-webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9);
  transition:transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9), -webkit-transform 200ms cubic-bezier(0.4, 1, 0.75, 0.9); }
  .bp3-tree-node-caret:hover{
    color:#182026; }
  .bp3-dark .bp3-tree-node-caret{
    color:#a7b6c2; }
    .bp3-dark .bp3-tree-node-caret:hover{
      color:#f5f8fa; }
  .bp3-tree-node-caret.bp3-tree-node-caret-open{
    -webkit-transform:rotate(90deg);
            transform:rotate(90deg); }
  .bp3-tree-node-caret.bp3-icon-standard::before{
    content:""; }

.bp3-tree-node-icon{
  position:relative;
  margin-right:7px; }

.bp3-tree-node-label{
  overflow:hidden;
  text-overflow:ellipsis;
  white-space:nowrap;
  word-wrap:normal;
  -webkit-box-flex:1;
      -ms-flex:1 1 auto;
          flex:1 1 auto;
  position:relative;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-tree-node-label span{
    display:inline; }

.bp3-tree-node-secondary-label{
  padding:0 5px;
  -webkit-user-select:none;
     -moz-user-select:none;
      -ms-user-select:none;
          user-select:none; }
  .bp3-tree-node-secondary-label .bp3-popover-wrapper,
  .bp3-tree-node-secondary-label .bp3-popover-target{
    display:-webkit-box;
    display:-ms-flexbox;
    display:flex;
    -webkit-box-align:center;
        -ms-flex-align:center;
            align-items:center; }

.bp3-tree-node.bp3-disabled .bp3-tree-node-content{
  background-color:inherit;
  cursor:not-allowed;
  color:rgba(92, 112, 128, 0.6); }

.bp3-tree-node.bp3-disabled .bp3-tree-node-caret,
.bp3-tree-node.bp3-disabled .bp3-tree-node-icon{
  cursor:not-allowed;
  color:rgba(92, 112, 128, 0.6); }

.bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
  background-color:#137cbd; }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content,
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-standard, .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-icon-large{
    color:#ffffff; }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret::before{
    color:rgba(255, 255, 255, 0.7); }
  .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content .bp3-tree-node-caret:hover::before{
    color:#ffffff; }

.bp3-dark .bp3-tree-node-content:hover{
  background-color:rgba(92, 112, 128, 0.3); }

.bp3-dark .bp3-tree .bp3-icon, .bp3-dark .bp3-tree .bp3-icon-standard, .bp3-dark .bp3-tree .bp3-icon-large{
  color:#a7b6c2; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-primary, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-primary{
    color:#137cbd; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-success, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-success{
    color:#0f9960; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-warning, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-warning{
    color:#d9822b; }
  .bp3-dark .bp3-tree .bp3-icon.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-standard.bp3-intent-danger, .bp3-dark .bp3-tree .bp3-icon-large.bp3-intent-danger{
    color:#db3737; }

.bp3-dark .bp3-tree-node.bp3-tree-node-selected > .bp3-tree-node-content{
  background-color:#137cbd; }
/*!

Copyright 2017-present Palantir Technologies, Inc. All rights reserved.
Licensed under the Apache License, Version 2.0.

*/
.bp3-omnibar{
  -webkit-filter:blur(0);
          filter:blur(0);
  opacity:1;
  top:20vh;
  left:calc(50% - 250px);
  z-index:21;
  border-radius:3px;
  -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
          box-shadow:0 0 0 1px rgba(16, 22, 26, 0.1), 0 4px 8px rgba(16, 22, 26, 0.2), 0 18px 46px 6px rgba(16, 22, 26, 0.2);
  background-color:#ffffff;
  width:500px; }
  .bp3-omnibar.bp3-overlay-enter, .bp3-omnibar.bp3-overlay-appear{
    -webkit-filter:blur(20px);
            filter:blur(20px);
    opacity:0.2; }
  .bp3-omnibar.bp3-overlay-enter-active, .bp3-omnibar.bp3-overlay-appear-active{
    -webkit-filter:blur(0);
            filter:blur(0);
    opacity:1;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:filter, opacity;
    transition-property:filter, opacity, -webkit-filter;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-omnibar.bp3-overlay-exit{
    -webkit-filter:blur(0);
            filter:blur(0);
    opacity:1; }
  .bp3-omnibar.bp3-overlay-exit-active{
    -webkit-filter:blur(20px);
            filter:blur(20px);
    opacity:0.2;
    -webkit-transition-property:opacity, -webkit-filter;
    transition-property:opacity, -webkit-filter;
    transition-property:filter, opacity;
    transition-property:filter, opacity, -webkit-filter;
    -webkit-transition-duration:200ms;
            transition-duration:200ms;
    -webkit-transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
            transition-timing-function:cubic-bezier(0.4, 1, 0.75, 0.9);
    -webkit-transition-delay:0;
            transition-delay:0; }
  .bp3-omnibar .bp3-input{
    border-radius:0;
    background-color:transparent; }
    .bp3-omnibar .bp3-input, .bp3-omnibar .bp3-input:focus{
      -webkit-box-shadow:none;
              box-shadow:none; }
  .bp3-omnibar .bp3-menu{
    border-radius:0;
    -webkit-box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
            box-shadow:inset 0 1px 0 rgba(16, 22, 26, 0.15);
    background-color:transparent;
    max-height:calc(60vh - 40px);
    overflow:auto; }
    .bp3-omnibar .bp3-menu:empty{
      display:none; }
  .bp3-dark .bp3-omnibar, .bp3-omnibar.bp3-dark{
    -webkit-box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
            box-shadow:0 0 0 1px rgba(16, 22, 26, 0.2), 0 4px 8px rgba(16, 22, 26, 0.4), 0 18px 46px 6px rgba(16, 22, 26, 0.4);
    background-color:#30404d; }

.bp3-omnibar-overlay .bp3-overlay-backdrop{
  background-color:rgba(16, 22, 26, 0.2); }

.bp3-select-popover .bp3-popover-content{
  padding:5px; }

.bp3-select-popover .bp3-input-group{
  margin-bottom:0; }

.bp3-select-popover .bp3-menu{
  max-width:400px;
  max-height:300px;
  overflow:auto;
  padding:0; }
  .bp3-select-popover .bp3-menu:not(:first-child){
    padding-top:5px; }

.bp3-multi-select{
  min-width:150px; }

.bp3-multi-select-popover .bp3-menu{
  max-width:400px;
  max-height:300px;
  overflow:auto; }

.bp3-select-popover .bp3-popover-content{
  padding:5px; }

.bp3-select-popover .bp3-input-group{
  margin-bottom:0; }

.bp3-select-popover .bp3-menu{
  max-width:400px;
  max-height:300px;
  overflow:auto;
  padding:0; }
  .bp3-select-popover .bp3-menu:not(:first-child){
    padding-top:5px; }
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensureUiComponents() in @jupyterlab/buildutils */

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

/* Icons urls */

:root {
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDhoLTIuODFjLS40NS0uNzgtMS4wNy0xLjQ1LTEuODItMS45NkwxNyA0LjQxIDE1LjU5IDNsLTIuMTcgMi4xN0MxMi45NiA1LjA2IDEyLjQ5IDUgMTIgNWMtLjQ5IDAtLjk2LjA2LTEuNDEuMTdMOC40MSAzIDcgNC40MWwxLjYyIDEuNjNDNy44OCA2LjU1IDcuMjYgNy4yMiA2LjgxIDhINHYyaDIuMDljLS4wNS4zMy0uMDkuNjYtLjA5IDF2MUg0djJoMnYxYzAgLjM0LjA0LjY3LjA5IDFINHYyaDIuODFjMS4wNCAxLjc5IDIuOTcgMyA1LjE5IDNzNC4xNS0xLjIxIDUuMTktM0gyMHYtMmgtMi4wOWMuMDUtLjMzLjA5LS42Ni4wOS0xdi0xaDJ2LTJoLTJ2LTFjMC0uMzQtLjA0LS42Ny0uMDktMUgyMFY4em0tNiA4aC00di0yaDR2MnptMC00aC00di0yaDR2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTYuMTdMNC44MyAxMmwtMS40MiAxLjQxTDkgMTkgMjEgN2wtMS40MS0xLjQxeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1pY29uLWJyYW5kMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNmZmYiPgogICAgPHBhdGggZD0iTTEwNSAxMjcuM2g0MHYxMi44aC00MHpNNTEuMSA3N0w3NCA5OS45bC0yMy4zIDIzLjMgMTAuNSAxMC41IDIzLjMtMjMuM0w5NSA5OS45IDg0LjUgODkuNCA2MS42IDY2LjV6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMSBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNGOUE4MjUiPgogICAgPHBhdGggZD0iTTIwLjIgMTEuOGMtMS42IDAtMS43LjUtMS43IDEgMCAuNC4xLjkuMSAxLjMuMS41LjEuOS4xIDEuMyAwIDEuNy0xLjQgMi4zLTMuNSAyLjNoLS45di0xLjloLjVjMS4xIDAgMS40IDAgMS40LS44IDAtLjMgMC0uNi0uMS0xIDAtLjQtLjEtLjgtLjEtMS4yIDAtMS4zIDAtMS44IDEuMy0yLTEuMy0uMi0xLjMtLjctMS4zLTIgMC0uNC4xLS44LjEtMS4yLjEtLjQuMS0uNy4xLTEgMC0uOC0uNC0uNy0xLjQtLjhoLS41VjQuMWguOWMyLjIgMCAzLjUuNyAzLjUgMi4zIDAgLjQtLjEuOS0uMSAxLjMtLjEuNS0uMS45LS4xIDEuMyAwIC41LjIgMSAxLjcgMXYxLjh6TTEuOCAxMC4xYzEuNiAwIDEuNy0uNSAxLjctMSAwLS40LS4xLS45LS4xLTEuMy0uMS0uNS0uMS0uOS0uMS0xLjMgMC0xLjYgMS40LTIuMyAzLjUtMi4zaC45djEuOWgtLjVjLTEgMC0xLjQgMC0xLjQuOCAwIC4zIDAgLjYuMSAxIDAgLjIuMS42LjEgMSAwIDEuMyAwIDEuOC0xLjMgMkM2IDExLjIgNiAxMS43IDYgMTNjMCAuNC0uMS44LS4xIDEuMi0uMS4zLS4xLjctLjEgMSAwIC44LjMuOCAxLjQuOGguNXYxLjloLS45Yy0yLjEgMC0zLjUtLjYtMy41LTIuMyAwLS40LjEtLjkuMS0xLjMuMS0uNS4xLS45LjEtMS4zIDAtLjUtLjItMS0xLjctMXYtMS45eiIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSIxMy44IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY3g9IjExIiBjeT0iOC4yIiByPSIyLjEiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgPGcgY2xhc3M9ImpwLWljb24td2FybjAiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4=);
  --jp-icon-listings-info: url(data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iaXNvLTg4NTktMSI/Pg0KPHN2ZyB2ZXJzaW9uPSIxLjEiIGlkPSJDYXBhXzEiIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHg9IjBweCIgeT0iMHB4Ig0KCSB2aWV3Qm94PSIwIDAgNTAuOTc4IDUwLjk3OCIgc3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgNTAuOTc4IDUwLjk3ODsiIHhtbDpzcGFjZT0icHJlc2VydmUiPg0KPGc+DQoJPGc+DQoJCTxnPg0KCQkJPHBhdGggc3R5bGU9ImZpbGw6IzAxMDAwMjsiIGQ9Ik00My41Miw3LjQ1OEMzOC43MTEsMi42NDgsMzIuMzA3LDAsMjUuNDg5LDBDMTguNjcsMCwxMi4yNjYsMi42NDgsNy40NTgsNy40NTgNCgkJCQljLTkuOTQzLDkuOTQxLTkuOTQzLDI2LjExOSwwLDM2LjA2MmM0LjgwOSw0LjgwOSwxMS4yMTIsNy40NTYsMTguMDMxLDcuNDU4YzAsMCwwLjAwMSwwLDAuMDAyLDANCgkJCQljNi44MTYsMCwxMy4yMjEtMi42NDgsMTguMDI5LTcuNDU4YzQuODA5LTQuODA5LDcuNDU3LTExLjIxMiw3LjQ1Ny0xOC4wM0M1MC45NzcsMTguNjcsNDguMzI4LDEyLjI2Niw0My41Miw3LjQ1OHoNCgkJCQkgTTQyLjEwNiw0Mi4xMDVjLTQuNDMyLDQuNDMxLTEwLjMzMiw2Ljg3Mi0xNi42MTUsNi44NzJoLTAuMDAyYy02LjI4NS0wLjAwMS0xMi4xODctMi40NDEtMTYuNjE3LTYuODcyDQoJCQkJYy05LjE2Mi05LjE2My05LjE2Mi0yNC4wNzEsMC0zMy4yMzNDMTMuMzAzLDQuNDQsMTkuMjA0LDIsMjUuNDg5LDJjNi4yODQsMCwxMi4xODYsMi40NCwxNi42MTcsNi44NzINCgkJCQljNC40MzEsNC40MzEsNi44NzEsMTAuMzMyLDYuODcxLDE2LjYxN0M0OC45NzcsMzEuNzcyLDQ2LjUzNiwzNy42NzUsNDIuMTA2LDQyLjEwNXoiLz4NCgkJPC9nPg0KCQk8Zz4NCgkJCTxwYXRoIHN0eWxlPSJmaWxsOiMwMTAwMDI7IiBkPSJNMjMuNTc4LDMyLjIxOGMtMC4wMjMtMS43MzQsMC4xNDMtMy4wNTksMC40OTYtMy45NzJjMC4zNTMtMC45MTMsMS4xMS0xLjk5NywyLjI3Mi0zLjI1Mw0KCQkJCWMwLjQ2OC0wLjUzNiwwLjkyMy0xLjA2MiwxLjM2Ny0xLjU3NWMwLjYyNi0wLjc1MywxLjEwNC0xLjQ3OCwxLjQzNi0yLjE3NWMwLjMzMS0wLjcwNywwLjQ5NS0xLjU0MSwwLjQ5NS0yLjUNCgkJCQljMC0xLjA5Ni0wLjI2LTIuMDg4LTAuNzc5LTIuOTc5Yy0wLjU2NS0wLjg3OS0xLjUwMS0xLjMzNi0yLjgwNi0xLjM2OWMtMS44MDIsMC4wNTctMi45ODUsMC42NjctMy41NSwxLjgzMg0KCQkJCWMtMC4zMDEsMC41MzUtMC41MDMsMS4xNDEtMC42MDcsMS44MTRjLTAuMTM5LDAuNzA3LTAuMjA3LDEuNDMyLTAuMjA3LDIuMTc0aC0yLjkzN2MtMC4wOTEtMi4yMDgsMC40MDctNC4xMTQsMS40OTMtNS43MTkNCgkJCQljMS4wNjItMS42NCwyLjg1NS0yLjQ4MSw1LjM3OC0yLjUyN2MyLjE2LDAuMDIzLDMuODc0LDAuNjA4LDUuMTQxLDEuNzU4YzEuMjc4LDEuMTYsMS45MjksMi43NjQsMS45NSw0LjgxMQ0KCQkJCWMwLDEuMTQyLTAuMTM3LDIuMTExLTAuNDEsMi45MTFjLTAuMzA5LDAuODQ1LTAuNzMxLDEuNTkzLTEuMjY4LDIuMjQzYy0wLjQ5MiwwLjY1LTEuMDY4LDEuMzE4LTEuNzMsMi4wMDINCgkJCQljLTAuNjUsMC42OTctMS4zMTMsMS40NzktMS45ODcsMi4zNDZjLTAuMjM5LDAuMzc3LTAuNDI5LDAuNzc3LTAuNTY1LDEuMTk5Yy0wLjE2LDAuOTU5LTAuMjE3LDEuOTUxLTAuMTcxLDIuOTc5DQoJCQkJQzI2LjU4OSwzMi4yMTgsMjMuNTc4LDMyLjIxOCwyMy41NzgsMzIuMjE4eiBNMjMuNTc4LDM4LjIydi0zLjQ4NGgzLjA3NnYzLjQ4NEgyMy41Nzh6Ii8+DQoJCTwvZz4NCgk8L2c+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8Zz4NCjwvZz4NCjxnPg0KPC9nPg0KPGc+DQo8L2c+DQo8L3N2Zz4NCg==);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMEQ0N0ExIj4KICAgIDxwYXRoIGQ9Ik0xMS4xIDYuOVY1LjhINi45YzAtLjUgMC0xLjMuMi0xLjYuNC0uNy44LTEuMSAxLjctMS40IDEuNy0uMyAyLjUtLjMgMy45LS4xIDEgLjEgMS45LjkgMS45IDEuOXY0LjJjMCAuNS0uOSAxLjYtMiAxLjZIOC44Yy0xLjUgMC0yLjQgMS40LTIuNCAyLjh2Mi4ySDQuN0MzLjUgMTUuMSAzIDE0IDMgMTMuMVY5Yy0uMS0xIC42LTIgMS44LTIgMS41LS4xIDYuMy0uMSA2LjMtLjF6Ii8+CiAgICA8cGF0aCBkPSJNMTAuOSAxNS4xdjEuMWg0LjJjMCAuNSAwIDEuMy0uMiAxLjYtLjQuNy0uOCAxLjEtMS43IDEuNC0xLjcuMy0yLjUuMy0zLjkuMS0xLS4xLTEuOS0uOS0xLjktMS45di00LjJjMC0uNS45LTEuNiAyLTEuNmgzLjhjMS41IDAgMi40LTEuNCAyLjQtMi44VjYuNmgxLjdDMTguNSA2LjkgMTkgOCAxOSA4LjlWMTNjMCAxLS43IDIuMS0xLjkgMi4xaC02LjJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
  --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiB3aWR0aD0iMjAiIGhlaWdodD0iMjAiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMikiIGZpbGw9IiMzMzMzMzMiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uLWFjY2VudDIganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGQ9Ik01LjA1NjY0IDguNzYxNzJDNS4wNTY2NCA4LjU5NzY2IDUuMDMxMjUgOC40NTMxMiA0Ljk4MDQ3IDguMzI4MTJDNC45MzM1OSA4LjE5OTIyIDQuODU1NDcgOC4wODIwMyA0Ljc0NjA5IDcuOTc2NTZDNC42NDA2MiA3Ljg3MTA5IDQuNSA3Ljc3NTM5IDQuMzI0MjIgNy42ODk0NUM0LjE1MjM0IDcuNTk5NjEgMy45NDMzNiA3LjUxMTcyIDMuNjk3MjcgNy40MjU3OEMzLjMwMjczIDcuMjg1MTYgMi45NDMzNiA3LjEzNjcyIDIuNjE5MTQgNi45ODA0N0MyLjI5NDkyIDYuODI0MjIgMi4wMTc1OCA2LjY0MjU4IDEuNzg3MTEgNi40MzU1NUMxLjU2MDU1IDYuMjI4NTIgMS4zODQ3NyA1Ljk4ODI4IDEuMjU5NzcgNS43MTQ4NEMxLjEzNDc3IDUuNDM3NSAxLjA3MjI3IDUuMTA5MzggMS4wNzIyNyA0LjczMDQ3QzEuMDcyMjcgNC4zOTg0NCAxLjEyODkxIDQuMDk1NyAxLjI0MjE5IDMuODIyMjdDMS4zNTU0NyAzLjU0NDkyIDEuNTE1NjIgMy4zMDQ2OSAxLjcyMjY2IDMuMTAxNTZDMS45Mjk2OSAyLjg5ODQ0IDIuMTc5NjkgMi43MzQzNyAyLjQ3MjY2IDIuNjA5MzhDMi43NjU2MiAyLjQ4NDM4IDMuMDkxOCAyLjQwNDMgMy40NTExNyAyLjM2OTE0VjEuMTA5MzhINC4zODg2N1YyLjM4MDg2QzQuNzQwMjMgMi40Mjc3MyA1LjA1NjY0IDIuNTIzNDQgNS4zMzc4OSAyLjY2Nzk3QzUuNjE5MTQgMi44MTI1IDUuODU3NDIgMy4wMDE5NSA2LjA1MjczIDMuMjM2MzNDNi4yNTE5NSAzLjQ2NjggNi40MDQzIDMuNzQwMjMgNi41MDk3NyA0LjA1NjY0QzYuNjE5MTQgNC4zNjkxNCA2LjY3MzgzIDQuNzIwNyA2LjY3MzgzIDUuMTExMzNINS4wNDQ5MkM1LjA0NDkyIDQuNjM4NjcgNC45Mzc1IDQuMjgxMjUgNC43MjI2NiA0LjAzOTA2QzQuNTA3ODEgMy43OTI5NyA0LjIxNjggMy42Njk5MiAzLjg0OTYxIDMuNjY5OTJDMy42NTAzOSAzLjY2OTkyIDMuNDc2NTYgMy42OTcyNyAzLjMyODEyIDMuNzUxOTVDMy4xODM1OSAzLjgwMjczIDMuMDY0NDUgMy44NzY5NSAyLjk3MDcgMy45NzQ2MUMyLjg3Njk1IDQuMDY4MzYgMi44MDY2NCA0LjE3OTY5IDIuNzU5NzcgNC4zMDg1OUMyLjcxNjggNC40Mzc1IDIuNjk1MzEgNC41NzgxMiAyLjY5NTMxIDQuNzMwNDdDMi42OTUzMSA0Ljg4MjgxIDIuNzE2OCA1LjAxOTUzIDIuNzU5NzcgNS4xNDA2MkMyLjgwNjY0IDUuMjU3ODEgMi44ODI4MSA1LjM2NzE5IDIuOTg4MjggNS40Njg3NUMzLjA5NzY2IDUuNTcwMzEgMy4yNDAyMyA1LjY2Nzk3IDMuNDE2MDIgNS43NjE3MkMzLjU5MTggNS44NTE1NiAzLjgxMDU1IDUuOTQzMzYgNC4wNzIyNyA2LjAzNzExQzQuNDY2OCA2LjE4NTU1IDQuODI0MjIgNi4zMzk4NCA1LjE0NDUzIDYuNUM1LjQ2NDg0IDYuNjU2MjUgNS43MzgyOCA2LjgzOTg0IDUuOTY0ODQgNy4wNTA3OEM2LjE5NTMxIDcuMjU3ODEgNi4zNzEwOSA3LjUgNi40OTIxOSA3Ljc3NzM0QzYuNjE3MTkgOC4wNTA3OCA2LjY3OTY5IDguMzc1IDYuNjc5NjkgOC43NUM2LjY3OTY5IDkuMDkzNzUgNi42MjMwNSA5LjQwNDMgNi41MDk3NyA5LjY4MTY0QzYuMzk2NDggOS45NTUwOCA2LjIzNDM4IDEwLjE5MTQgNi4wMjM0NCAxMC4zOTA2QzUuODEyNSAxMC41ODk4IDUuNTU4NTkgMTAuNzUgNS4yNjE3MiAxMC44NzExQzQuOTY0ODQgMTAuOTg4MyA0LjYzMjgxIDExLjA2NDUgNC4yNjU2MiAxMS4wOTk2VjEyLjI0OEgzLjMzMzk4VjExLjA5OTZDMy4wMDE5NSAxMS4wNjg0IDIuNjc5NjkgMTAuOTk2MSAyLjM2NzE5IDEwLjg4MjhDMi4wNTQ2OSAxMC43NjU2IDEuNzc3MzQgMTAuNTk3NyAxLjUzNTE2IDEwLjM3ODlDMS4yOTY4OCAxMC4xNjAyIDEuMTA1NDcgOS44ODQ3NyAwLjk2MDkzOCA5LjU1MjczQzAuODE2NDA2IDkuMjE2OCAwLjc0NDE0MSA4LjgxNDQ1IDAuNzQ0MTQxIDguMzQ1N0gyLjM3ODkxQzIuMzc4OTEgOC42MjY5NSAyLjQxOTkyIDguODYzMjggMi41MDE5NSA5LjA1NDY5QzIuNTgzOTggOS4yNDIxOSAyLjY4OTQ1IDkuMzkyNTggMi44MTgzNiA5LjUwNTg2QzIuOTUxMTcgOS42MTUyMyAzLjEwMTU2IDkuNjkzMzYgMy4yNjk1MyA5Ljc0MDIzQzMuNDM3NSA5Ljc4NzExIDMuNjA5MzggOS44MTA1NSAzLjc4NTE2IDkuODEwNTVDNC4yMDMxMiA5LjgxMDU1IDQuNTE5NTMgOS43MTI4OSA0LjczNDM4IDkuNTE3NThDNC45NDkyMiA5LjMyMjI3IDUuMDU2NjQgOS4wNzAzMSA1LjA1NjY0IDguNzYxNzJaTTEzLjQxOCAxMi4yNzE1SDguMDc0MjJWMTFIMTMuNDE4VjEyLjI3MTVaIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzLjk1MjY0IDYpIiBmaWxsPSJ3aGl0ZSIvPgo8L3N2Zz4K);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTUgMTVIM3YyaDEydi0yem0wLThIM3YyaDEyVjd6TTMgMTNoMTh2LTJIM3Yyem0wIDhoMTh2LTJIM3Yyek0zIDN2MmgxOFYzSDN6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}
.jp-BugIcon {
  background-image: var(--jp-icon-bug);
}
.jp-BuildIcon {
  background-image: var(--jp-icon-build);
}
.jp-CaretDownEmptyIcon {
  background-image: var(--jp-icon-caret-down-empty);
}
.jp-CaretDownEmptyThinIcon {
  background-image: var(--jp-icon-caret-down-empty-thin);
}
.jp-CaretDownIcon {
  background-image: var(--jp-icon-caret-down);
}
.jp-CaretLeftIcon {
  background-image: var(--jp-icon-caret-left);
}
.jp-CaretRightIcon {
  background-image: var(--jp-icon-caret-right);
}
.jp-CaretUpEmptyThinIcon {
  background-image: var(--jp-icon-caret-up-empty-thin);
}
.jp-CaretUpIcon {
  background-image: var(--jp-icon-caret-up);
}
.jp-CaseSensitiveIcon {
  background-image: var(--jp-icon-case-sensitive);
}
.jp-CheckIcon {
  background-image: var(--jp-icon-check);
}
.jp-CircleEmptyIcon {
  background-image: var(--jp-icon-circle-empty);
}
.jp-CircleIcon {
  background-image: var(--jp-icon-circle);
}
.jp-ClearIcon {
  background-image: var(--jp-icon-clear);
}
.jp-CloseIcon {
  background-image: var(--jp-icon-close);
}
.jp-ConsoleIcon {
  background-image: var(--jp-icon-console);
}
.jp-CopyIcon {
  background-image: var(--jp-icon-copy);
}
.jp-CutIcon {
  background-image: var(--jp-icon-cut);
}
.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}
.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}
.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}
.jp-ExtensionIcon {
  background-image: var(--jp-icon-extension);
}
.jp-FastForwardIcon {
  background-image: var(--jp-icon-fast-forward);
}
.jp-FileIcon {
  background-image: var(--jp-icon-file);
}
.jp-FileUploadIcon {
  background-image: var(--jp-icon-file-upload);
}
.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}
.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}
.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}
.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}
.jp-InspectorIcon {
  background-image: var(--jp-icon-inspector);
}
.jp-JsonIcon {
  background-image: var(--jp-icon-json);
}
.jp-JupyterFaviconIcon {
  background-image: var(--jp-icon-jupyter-favicon);
}
.jp-JupyterIcon {
  background-image: var(--jp-icon-jupyter);
}
.jp-JupyterlabWordmarkIcon {
  background-image: var(--jp-icon-jupyterlab-wordmark);
}
.jp-KernelIcon {
  background-image: var(--jp-icon-kernel);
}
.jp-KeyboardIcon {
  background-image: var(--jp-icon-keyboard);
}
.jp-LauncherIcon {
  background-image: var(--jp-icon-launcher);
}
.jp-LineFormIcon {
  background-image: var(--jp-icon-line-form);
}
.jp-LinkIcon {
  background-image: var(--jp-icon-link);
}
.jp-ListIcon {
  background-image: var(--jp-icon-list);
}
.jp-ListingsInfoIcon {
  background-image: var(--jp-icon-listings-info);
}
.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}
.jp-NewFolderIcon {
  background-image: var(--jp-icon-new-folder);
}
.jp-NotTrustedIcon {
  background-image: var(--jp-icon-not-trusted);
}
.jp-NotebookIcon {
  background-image: var(--jp-icon-notebook);
}
.jp-PaletteIcon {
  background-image: var(--jp-icon-palette);
}
.jp-PasteIcon {
  background-image: var(--jp-icon-paste);
}
.jp-PythonIcon {
  background-image: var(--jp-icon-python);
}
.jp-RKernelIcon {
  background-image: var(--jp-icon-r-kernel);
}
.jp-ReactIcon {
  background-image: var(--jp-icon-react);
}
.jp-RefreshIcon {
  background-image: var(--jp-icon-refresh);
}
.jp-RegexIcon {
  background-image: var(--jp-icon-regex);
}
.jp-RunIcon {
  background-image: var(--jp-icon-run);
}
.jp-RunningIcon {
  background-image: var(--jp-icon-running);
}
.jp-SaveIcon {
  background-image: var(--jp-icon-save);
}
.jp-SearchIcon {
  background-image: var(--jp-icon-search);
}
.jp-SettingsIcon {
  background-image: var(--jp-icon-settings);
}
.jp-SpreadsheetIcon {
  background-image: var(--jp-icon-spreadsheet);
}
.jp-StopIcon {
  background-image: var(--jp-icon-stop);
}
.jp-TabIcon {
  background-image: var(--jp-icon-tab);
}
.jp-TerminalIcon {
  background-image: var(--jp-icon-terminal);
}
.jp-TextEditorIcon {
  background-image: var(--jp-icon-text-editor);
}
.jp-TrustedIcon {
  background-image: var(--jp-icon-trusted);
}
.jp-UndoIcon {
  background-image: var(--jp-icon-undo);
}
.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}
.jp-YamlIcon {
  background-image: var(--jp-icon-yaml);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * (DEPRECATED) Support for consuming icons as CSS background images
 */

:root {
  --jp-icon-search-white: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
}

.jp-Icon,
.jp-MaterialIcon {
  background-position: center;
  background-repeat: no-repeat;
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-cover {
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
}

/**
 * (DEPRECATED) Support for specific CSS icon sizes
 */

.jp-Icon-16 {
  background-size: 16px;
  min-width: 16px;
  min-height: 16px;
}

.jp-Icon-18 {
  background-size: 18px;
  min-width: 18px;
  min-height: 18px;
}

.jp-Icon-20 {
  background-size: 20px;
  min-width: 20px;
  min-height: 20px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for icons as inline SVG HTMLElements
 */

/* recolor the primary elements of an icon */
.jp-icon0[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon1[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon2[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon3[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}
/* recolor the accent elements of an icon */
.jp-icon-accent0[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-accent1[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-accent2[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-accent3[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-accent4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-accent0[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-accent1[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-accent2[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-accent3[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-accent4[stroke] {
  stroke: var(--jp-layout-color4);
}
/* set the color of an icon to transparent */
.jp-icon-none[fill] {
  fill: none;
}

.jp-icon-none[stroke] {
  stroke: none;
}
/* brand icon colors. Same for light and dark */
.jp-icon-brand0[fill] {
  fill: var(--jp-brand-color0);
}
.jp-icon-brand1[fill] {
  fill: var(--jp-brand-color1);
}
.jp-icon-brand2[fill] {
  fill: var(--jp-brand-color2);
}
.jp-icon-brand3[fill] {
  fill: var(--jp-brand-color3);
}
.jp-icon-brand4[fill] {
  fill: var(--jp-brand-color4);
}

.jp-icon-brand0[stroke] {
  stroke: var(--jp-brand-color0);
}
.jp-icon-brand1[stroke] {
  stroke: var(--jp-brand-color1);
}
.jp-icon-brand2[stroke] {
  stroke: var(--jp-brand-color2);
}
.jp-icon-brand3[stroke] {
  stroke: var(--jp-brand-color3);
}
.jp-icon-brand4[stroke] {
  stroke: var(--jp-brand-color4);
}
/* warn icon colors. Same for light and dark */
.jp-icon-warn0[fill] {
  fill: var(--jp-warn-color0);
}
.jp-icon-warn1[fill] {
  fill: var(--jp-warn-color1);
}
.jp-icon-warn2[fill] {
  fill: var(--jp-warn-color2);
}
.jp-icon-warn3[fill] {
  fill: var(--jp-warn-color3);
}

.jp-icon-warn0[stroke] {
  stroke: var(--jp-warn-color0);
}
.jp-icon-warn1[stroke] {
  stroke: var(--jp-warn-color1);
}
.jp-icon-warn2[stroke] {
  stroke: var(--jp-warn-color2);
}
.jp-icon-warn3[stroke] {
  stroke: var(--jp-warn-color3);
}
/* icon colors that contrast well with each other and most backgrounds */
.jp-icon-contrast0[fill] {
  fill: var(--jp-icon-contrast-color0);
}
.jp-icon-contrast1[fill] {
  fill: var(--jp-icon-contrast-color1);
}
.jp-icon-contrast2[fill] {
  fill: var(--jp-icon-contrast-color2);
}
.jp-icon-contrast3[fill] {
  fill: var(--jp-icon-contrast-color3);
}

.jp-icon-contrast0[stroke] {
  stroke: var(--jp-icon-contrast-color0);
}
.jp-icon-contrast1[stroke] {
  stroke: var(--jp-icon-contrast-color1);
}
.jp-icon-contrast2[stroke] {
  stroke: var(--jp-icon-contrast-color2);
}
.jp-icon-contrast3[stroke] {
  stroke: var(--jp-icon-contrast-color3);
}

/* CSS for icons in selected items in the settings editor */
#setting-editor .jp-PluginList .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}
#setting-editor
  .jp-PluginList
  .jp-mod-selected
  .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* CSS for icons in selected tabs in the sidebar tab manager */
#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable[fill] {
  fill: #fff;
}

#tab-manager .lm-TabBar-tab.jp-mod-active .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}
#tab-manager
  .lm-TabBar-tab.jp-mod-active
  .jp-icon-hover
  :hover
  .jp-icon-selectable[fill] {
  fill: var(--jp-brand-color1);
}

#tab-manager
  .lm-TabBar-tab.jp-mod-active
  .jp-icon-hover
  :hover
  .jp-icon-selectable-inverse[fill] {
  fill: #fff;
}

/**
 * TODO: come up with non css-hack solution for showing the busy icon on top
 *  of the close icon
 * CSS for complex behavior of close icon of tabs in the sidebar tab manager
 */
#tab-manager
  .lm-TabBar-tab.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}
#tab-manager
  .lm-TabBar-tab.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

#tab-manager
  .lm-TabBar-tab.jp-mod-dirty.jp-mod-active
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: #fff;
}

/**
* TODO: come up with non css-hack solution for showing the busy icon on top
*  of the close icon
* CSS for complex behavior of close icon of tabs in the main area tabbar
*/
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon3[fill] {
  fill: none;
}
.lm-DockPanel-tabBar
  .lm-TabBar-tab.lm-mod-closable.jp-mod-dirty
  > .lm-TabBar-tabCloseIcon
  > :not(:hover)
  > .jp-icon-busy[fill] {
  fill: var(--jp-inverse-layout-color3);
}

/* CSS for icons in status bar */
#jp-main-statusbar .jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

#jp-main-statusbar .jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}
/* special handling for splash icon CSS. While the theme CSS reloads during
   splash, the splash icon can loose theming. To prevent that, we set a
   default for its color variable */
:root {
  --jp-warn-color0: var(--md-orange-700);
}

/* not sure what to do with this one, used in filebrowser listing */
.jp-DragIcon {
  margin-right: 4px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/**
 * Support for alt colors for icons as inline SVG HTMLElements
 */

/* alt recolor the primary elements of an icon */
.jp-icon-alt .jp-icon0[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-alt .jp-icon1[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-alt .jp-icon2[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-alt .jp-icon3[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-alt .jp-icon4[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-alt .jp-icon0[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-alt .jp-icon1[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-alt .jp-icon2[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-alt .jp-icon3[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-alt .jp-icon4[stroke] {
  stroke: var(--jp-layout-color4);
}

/* alt recolor the accent elements of an icon */
.jp-icon-alt .jp-icon-accent0[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-alt .jp-icon-accent1[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-alt .jp-icon-accent2[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-alt .jp-icon-accent3[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-alt .jp-icon-accent4[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-alt .jp-icon-accent0[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-alt .jp-icon-accent1[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-alt .jp-icon-accent2[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-alt .jp-icon-accent3[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-alt .jp-icon-accent4[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-icon-hoverShow:not(:hover) svg {
  display: none !important;
}

/**
 * Support for hover colors for icons as inline SVG HTMLElements
 */

/**
 * regular colors
 */

/* recolor the primary elements of an icon */
.jp-icon-hover :hover .jp-icon0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-hover :hover .jp-icon1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-hover :hover .jp-icon2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-hover :hover .jp-icon3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-hover :hover .jp-icon4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-hover :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-hover :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-hover :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-hover :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/* recolor the accent elements of an icon */
.jp-icon-hover :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-hover :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-hover :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-hover :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-hover :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-hover :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-hover :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-hover :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-hover :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* set the color of an icon to transparent */
.jp-icon-hover :hover .jp-icon-none-hover[fill] {
  fill: none;
}

.jp-icon-hover :hover .jp-icon-none-hover[stroke] {
  stroke: none;
}

/**
 * inverse colors
 */

/* inverse recolor the primary elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[fill] {
  fill: var(--jp-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[fill] {
  fill: var(--jp-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[fill] {
  fill: var(--jp-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[fill] {
  fill: var(--jp-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[fill] {
  fill: var(--jp-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon0-hover[stroke] {
  stroke: var(--jp-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon1-hover[stroke] {
  stroke: var(--jp-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon2-hover[stroke] {
  stroke: var(--jp-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon3-hover[stroke] {
  stroke: var(--jp-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon4-hover[stroke] {
  stroke: var(--jp-layout-color4);
}

/* inverse recolor the accent elements of an icon */
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[fill] {
  fill: var(--jp-inverse-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[fill] {
  fill: var(--jp-inverse-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[fill] {
  fill: var(--jp-inverse-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[fill] {
  fill: var(--jp-inverse-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[fill] {
  fill: var(--jp-inverse-layout-color4);
}

.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent0-hover[stroke] {
  stroke: var(--jp-inverse-layout-color0);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent1-hover[stroke] {
  stroke: var(--jp-inverse-layout-color1);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent2-hover[stroke] {
  stroke: var(--jp-inverse-layout-color2);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent3-hover[stroke] {
  stroke: var(--jp-inverse-layout-color3);
}
.jp-icon-hover.jp-icon-alt :hover .jp-icon-accent4-hover[stroke] {
  stroke: var(--jp-inverse-layout-color4);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

/* Override Blueprint's _reset.scss styles */
html {
  box-sizing: unset;
}

*,
*::before,
*::after {
  box-sizing: unset;
}

body {
  color: unset;
  font-family: var(--jp-ui-font-family);
}

p {
  margin-top: unset;
  margin-bottom: unset;
}

small {
  font-size: unset;
}

strong {
  font-weight: unset;
}

/* Override Blueprint's _typography.scss styles */
a {
  text-decoration: unset;
  color: unset;
}
a:hover {
  text-decoration: unset;
  color: unset;
}

/* Override Blueprint's _accessibility.scss styles */
:focus {
  outline: unset;
  outline-offset: unset;
  -moz-outline-radius: unset;
}

/* Styles for ui-components */
.jp-Button {
  border-radius: var(--jp-border-radius);
  padding: 0px 12px;
  font-size: var(--jp-ui-font-size1);
}

/* Use our own theme for hover styles */
button.jp-Button.bp3-button.bp3-minimal:hover {
  background-color: var(--jp-layout-color2);
}
.jp-Button.minimal {
  color: unset !important;
}

.jp-Button.jp-ToolbarButtonComponent {
  text-transform: none;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color3);
}

.jp-BPIcon {
  display: inline-block;
  vertical-align: middle;
  margin: auto;
}

/* Stop blueprint futzing with our icon fills */
.bp3-icon.jp-BPIcon > svg:not([fill]) {
  fill: var(--jp-inverse-layout-color3);
}

.jp-InputGroupAction {
  padding: 6px;
}

.jp-HTMLSelect.jp-DefaultStyle select {
  background-color: initial;
  border: none;
  border-radius: 0;
  box-shadow: none;
  color: var(--jp-ui-font-color0);
  display: block;
  font-size: var(--jp-ui-font-size1);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

/* Use our own theme for hover and option styles */
.jp-HTMLSelect.jp-DefaultStyle select:hover,
.jp-HTMLSelect.jp-DefaultStyle select > option {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color0);
}
select {
  box-sizing: border-box;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-top: 1px solid var(--jp-border-color2);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-Collapse-header {
  padding: 1px 12px;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size2);
}

.jp-Collapse-header:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Collapse-contents {
  padding: 0px 12px 0px 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-commandpalette-search-height: 28px;
}

/*-----------------------------------------------------------------------------
| Overall styles
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  padding-bottom: 0px;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Search
|----------------------------------------------------------------------------*/

.lm-CommandPalette-search {
  padding: 4px;
  background-color: var(--jp-layout-color1);
  z-index: 2;
}

.lm-CommandPalette-wrapper {
  overflow: overlay;
  padding: 0px 9px;
  background-color: var(--jp-input-active-background);
  height: 30px;
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
  box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.lm-CommandPalette-wrapper::after {
  content: ' ';
  color: white;
  background-color: var(--jp-brand-color1);
  position: absolute;
  top: 4px;
  right: 4px;
  height: 30px;
  width: 10px;
  padding: 0px 10px;
  background-image: var(--jp-icon-search-white);
  background-size: 20px;
  background-repeat: no-repeat;
  background-position: center;
}

.lm-CommandPalette-input {
  background: transparent;
  width: calc(100% - 18px);
  float: left;
  border: none;
  outline: none;
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  line-height: var(--jp-private-commandpalette-search-height);
}

.lm-CommandPalette-input::-webkit-input-placeholder,
.lm-CommandPalette-input::-moz-placeholder,
.lm-CommandPalette-input:-ms-input-placeholder {
  color: var(--jp-ui-font-color3);
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------*/

.lm-CommandPalette-header:first-child {
  margin-top: 0px;
}

.lm-CommandPalette-header {
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin-top: 8px;
  padding: 8px 0 8px 12px;
  text-transform: uppercase;
}

.lm-CommandPalette-header.lm-mod-active {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-header > mark {
  background-color: transparent;
  font-weight: bold;
  color: var(--jp-ui-font-color1);
}

.lm-CommandPalette-item {
  padding: 4px 12px 4px 4px;
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  font-weight: 400;
  display: flex;
}

.lm-CommandPalette-item.lm-mod-disabled {
  color: var(--jp-ui-font-color3);
}

.lm-CommandPalette-item.lm-mod-active {
  background: var(--jp-layout-color3);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
  background: var(--jp-layout-color4);
}

.lm-CommandPalette-item:hover:not(.lm-mod-active):not(.lm-mod-disabled) {
  background: var(--jp-layout-color2);
}

.lm-CommandPalette-itemContent {
  overflow: hidden;
}

.lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.lm-CommandPalette-item.lm-mod-disabled mark {
  color: var(--jp-ui-font-color3);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
  margin: 0 4px 0 0;
  position: relative;
  width: 16px;
  top: 2px;
  flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
  opacity: 0.4;
}

.lm-CommandPalette-item .lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemCaption {
  display: none;
}

.lm-CommandPalette-content {
  background-color: var(--jp-layout-color1);
}

.lm-CommandPalette-content:empty:after {
  content: 'No results';
  margin: auto;
  margin-top: 20px;
  width: 100px;
  display: block;
  font-size: var(--jp-ui-font-size2);
  font-family: var(--jp-ui-font-family);
  font-weight: lighter;
}

.lm-CommandPalette-emptyMessage {
  text-align: center;
  margin-top: 24px;
  line-height: 1.32;
  padding: 0px 8px;
  color: var(--jp-content-font-color3);
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Dialog {
  position: absolute;
  z-index: 10000;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  top: 0px;
  left: 0px;
  margin: 0;
  padding: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-dialog-background);
}

.jp-Dialog-content {
  display: flex;
  flex-direction: column;
  margin-left: auto;
  margin-right: auto;
  background: var(--jp-layout-color1);
  padding: 24px;
  padding-bottom: 12px;
  min-width: 300px;
  min-height: 150px;
  max-width: 1000px;
  max-height: 500px;
  box-sizing: border-box;
  box-shadow: var(--jp-elevation-z20);
  word-wrap: break-word;
  border-radius: var(--jp-border-radius);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color1);
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0px;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

.jp-Dialog-header {
  flex: 0 0 auto;
  padding-bottom: 12px;
  font-size: var(--jp-ui-font-size3);
  font-weight: 400;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-title {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.jp-Dialog-body > .jp-select-wrapper {
  width: 100%;
}

.jp-Dialog-body > button {
  padding: 0px 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-HoverBox {
  position: fixed;
}

.jp-HoverBox.jp-mod-outofview {
  display: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MainAreaWidget > :focus {
  outline: none;
}

/**
 * google-material-color v1.2.6
 * https://github.com/danlevan/google-material-color
 */
:root {
  --md-red-50: #ffebee;
  --md-red-100: #ffcdd2;
  --md-red-200: #ef9a9a;
  --md-red-300: #e57373;
  --md-red-400: #ef5350;
  --md-red-500: #f44336;
  --md-red-600: #e53935;
  --md-red-700: #d32f2f;
  --md-red-800: #c62828;
  --md-red-900: #b71c1c;
  --md-red-A100: #ff8a80;
  --md-red-A200: #ff5252;
  --md-red-A400: #ff1744;
  --md-red-A700: #d50000;

  --md-pink-50: #fce4ec;
  --md-pink-100: #f8bbd0;
  --md-pink-200: #f48fb1;
  --md-pink-300: #f06292;
  --md-pink-400: #ec407a;
  --md-pink-500: #e91e63;
  --md-pink-600: #d81b60;
  --md-pink-700: #c2185b;
  --md-pink-800: #ad1457;
  --md-pink-900: #880e4f;
  --md-pink-A100: #ff80ab;
  --md-pink-A200: #ff4081;
  --md-pink-A400: #f50057;
  --md-pink-A700: #c51162;

  --md-purple-50: #f3e5f5;
  --md-purple-100: #e1bee7;
  --md-purple-200: #ce93d8;
  --md-purple-300: #ba68c8;
  --md-purple-400: #ab47bc;
  --md-purple-500: #9c27b0;
  --md-purple-600: #8e24aa;
  --md-purple-700: #7b1fa2;
  --md-purple-800: #6a1b9a;
  --md-purple-900: #4a148c;
  --md-purple-A100: #ea80fc;
  --md-purple-A200: #e040fb;
  --md-purple-A400: #d500f9;
  --md-purple-A700: #aa00ff;

  --md-deep-purple-50: #ede7f6;
  --md-deep-purple-100: #d1c4e9;
  --md-deep-purple-200: #b39ddb;
  --md-deep-purple-300: #9575cd;
  --md-deep-purple-400: #7e57c2;
  --md-deep-purple-500: #673ab7;
  --md-deep-purple-600: #5e35b1;
  --md-deep-purple-700: #512da8;
  --md-deep-purple-800: #4527a0;
  --md-deep-purple-900: #311b92;
  --md-deep-purple-A100: #b388ff;
  --md-deep-purple-A200: #7c4dff;
  --md-deep-purple-A400: #651fff;
  --md-deep-purple-A700: #6200ea;

  --md-indigo-50: #e8eaf6;
  --md-indigo-100: #c5cae9;
  --md-indigo-200: #9fa8da;
  --md-indigo-300: #7986cb;
  --md-indigo-400: #5c6bc0;
  --md-indigo-500: #3f51b5;
  --md-indigo-600: #3949ab;
  --md-indigo-700: #303f9f;
  --md-indigo-800: #283593;
  --md-indigo-900: #1a237e;
  --md-indigo-A100: #8c9eff;
  --md-indigo-A200: #536dfe;
  --md-indigo-A400: #3d5afe;
  --md-indigo-A700: #304ffe;

  --md-blue-50: #e3f2fd;
  --md-blue-100: #bbdefb;
  --md-blue-200: #90caf9;
  --md-blue-300: #64b5f6;
  --md-blue-400: #42a5f5;
  --md-blue-500: #2196f3;
  --md-blue-600: #1e88e5;
  --md-blue-700: #1976d2;
  --md-blue-800: #1565c0;
  --md-blue-900: #0d47a1;
  --md-blue-A100: #82b1ff;
  --md-blue-A200: #448aff;
  --md-blue-A400: #2979ff;
  --md-blue-A700: #2962ff;

  --md-light-blue-50: #e1f5fe;
  --md-light-blue-100: #b3e5fc;
  --md-light-blue-200: #81d4fa;
  --md-light-blue-300: #4fc3f7;
  --md-light-blue-400: #29b6f6;
  --md-light-blue-500: #03a9f4;
  --md-light-blue-600: #039be5;
  --md-light-blue-700: #0288d1;
  --md-light-blue-800: #0277bd;
  --md-light-blue-900: #01579b;
  --md-light-blue-A100: #80d8ff;
  --md-light-blue-A200: #40c4ff;
  --md-light-blue-A400: #00b0ff;
  --md-light-blue-A700: #0091ea;

  --md-cyan-50: #e0f7fa;
  --md-cyan-100: #b2ebf2;
  --md-cyan-200: #80deea;
  --md-cyan-300: #4dd0e1;
  --md-cyan-400: #26c6da;
  --md-cyan-500: #00bcd4;
  --md-cyan-600: #00acc1;
  --md-cyan-700: #0097a7;
  --md-cyan-800: #00838f;
  --md-cyan-900: #006064;
  --md-cyan-A100: #84ffff;
  --md-cyan-A200: #18ffff;
  --md-cyan-A400: #00e5ff;
  --md-cyan-A700: #00b8d4;

  --md-teal-50: #e0f2f1;
  --md-teal-100: #b2dfdb;
  --md-teal-200: #80cbc4;
  --md-teal-300: #4db6ac;
  --md-teal-400: #26a69a;
  --md-teal-500: #009688;
  --md-teal-600: #00897b;
  --md-teal-700: #00796b;
  --md-teal-800: #00695c;
  --md-teal-900: #004d40;
  --md-teal-A100: #a7ffeb;
  --md-teal-A200: #64ffda;
  --md-teal-A400: #1de9b6;
  --md-teal-A700: #00bfa5;

  --md-green-50: #e8f5e9;
  --md-green-100: #c8e6c9;
  --md-green-200: #a5d6a7;
  --md-green-300: #81c784;
  --md-green-400: #66bb6a;
  --md-green-500: #4caf50;
  --md-green-600: #43a047;
  --md-green-700: #388e3c;
  --md-green-800: #2e7d32;
  --md-green-900: #1b5e20;
  --md-green-A100: #b9f6ca;
  --md-green-A200: #69f0ae;
  --md-green-A400: #00e676;
  --md-green-A700: #00c853;

  --md-light-green-50: #f1f8e9;
  --md-light-green-100: #dcedc8;
  --md-light-green-200: #c5e1a5;
  --md-light-green-300: #aed581;
  --md-light-green-400: #9ccc65;
  --md-light-green-500: #8bc34a;
  --md-light-green-600: #7cb342;
  --md-light-green-700: #689f38;
  --md-light-green-800: #558b2f;
  --md-light-green-900: #33691e;
  --md-light-green-A100: #ccff90;
  --md-light-green-A200: #b2ff59;
  --md-light-green-A400: #76ff03;
  --md-light-green-A700: #64dd17;

  --md-lime-50: #f9fbe7;
  --md-lime-100: #f0f4c3;
  --md-lime-200: #e6ee9c;
  --md-lime-300: #dce775;
  --md-lime-400: #d4e157;
  --md-lime-500: #cddc39;
  --md-lime-600: #c0ca33;
  --md-lime-700: #afb42b;
  --md-lime-800: #9e9d24;
  --md-lime-900: #827717;
  --md-lime-A100: #f4ff81;
  --md-lime-A200: #eeff41;
  --md-lime-A400: #c6ff00;
  --md-lime-A700: #aeea00;

  --md-yellow-50: #fffde7;
  --md-yellow-100: #fff9c4;
  --md-yellow-200: #fff59d;
  --md-yellow-300: #fff176;
  --md-yellow-400: #ffee58;
  --md-yellow-500: #ffeb3b;
  --md-yellow-600: #fdd835;
  --md-yellow-700: #fbc02d;
  --md-yellow-800: #f9a825;
  --md-yellow-900: #f57f17;
  --md-yellow-A100: #ffff8d;
  --md-yellow-A200: #ffff00;
  --md-yellow-A400: #ffea00;
  --md-yellow-A700: #ffd600;

  --md-amber-50: #fff8e1;
  --md-amber-100: #ffecb3;
  --md-amber-200: #ffe082;
  --md-amber-300: #ffd54f;
  --md-amber-400: #ffca28;
  --md-amber-500: #ffc107;
  --md-amber-600: #ffb300;
  --md-amber-700: #ffa000;
  --md-amber-800: #ff8f00;
  --md-amber-900: #ff6f00;
  --md-amber-A100: #ffe57f;
  --md-amber-A200: #ffd740;
  --md-amber-A400: #ffc400;
  --md-amber-A700: #ffab00;

  --md-orange-50: #fff3e0;
  --md-orange-100: #ffe0b2;
  --md-orange-200: #ffcc80;
  --md-orange-300: #ffb74d;
  --md-orange-400: #ffa726;
  --md-orange-500: #ff9800;
  --md-orange-600: #fb8c00;
  --md-orange-700: #f57c00;
  --md-orange-800: #ef6c00;
  --md-orange-900: #e65100;
  --md-orange-A100: #ffd180;
  --md-orange-A200: #ffab40;
  --md-orange-A400: #ff9100;
  --md-orange-A700: #ff6d00;

  --md-deep-orange-50: #fbe9e7;
  --md-deep-orange-100: #ffccbc;
  --md-deep-orange-200: #ffab91;
  --md-deep-orange-300: #ff8a65;
  --md-deep-orange-400: #ff7043;
  --md-deep-orange-500: #ff5722;
  --md-deep-orange-600: #f4511e;
  --md-deep-orange-700: #e64a19;
  --md-deep-orange-800: #d84315;
  --md-deep-orange-900: #bf360c;
  --md-deep-orange-A100: #ff9e80;
  --md-deep-orange-A200: #ff6e40;
  --md-deep-orange-A400: #ff3d00;
  --md-deep-orange-A700: #dd2c00;

  --md-brown-50: #efebe9;
  --md-brown-100: #d7ccc8;
  --md-brown-200: #bcaaa4;
  --md-brown-300: #a1887f;
  --md-brown-400: #8d6e63;
  --md-brown-500: #795548;
  --md-brown-600: #6d4c41;
  --md-brown-700: #5d4037;
  --md-brown-800: #4e342e;
  --md-brown-900: #3e2723;

  --md-grey-50: #fafafa;
  --md-grey-100: #f5f5f5;
  --md-grey-200: #eeeeee;
  --md-grey-300: #e0e0e0;
  --md-grey-400: #bdbdbd;
  --md-grey-500: #9e9e9e;
  --md-grey-600: #757575;
  --md-grey-700: #616161;
  --md-grey-800: #424242;
  --md-grey-900: #212121;

  --md-blue-grey-50: #eceff1;
  --md-blue-grey-100: #cfd8dc;
  --md-blue-grey-200: #b0bec5;
  --md-blue-grey-300: #90a4ae;
  --md-blue-grey-400: #78909c;
  --md-blue-grey-500: #607d8b;
  --md-blue-grey-600: #546e7a;
  --md-blue-grey-700: #455a64;
  --md-blue-grey-800: #37474f;
  --md-blue-grey-900: #263238;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Spinner {
  position: absolute;
  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 10;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background: var(--jp-layout-color0);
  outline: none;
}

.jp-SpinnerContent {
  font-size: 10px;
  margin: 50px auto;
  text-indent: -9999em;
  width: 3em;
  height: 3em;
  border-radius: 50%;
  background: var(--jp-brand-color3);
  background: linear-gradient(
    to right,
    #f37626 10%,
    rgba(255, 255, 255, 0) 42%
  );
  position: relative;
  animation: load3 1s infinite linear, fadeIn 1s;
}

.jp-SpinnerContent:before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent:after {
  background: var(--jp-layout-color0);
  width: 75%;
  height: 75%;
  border-radius: 50%;
  content: '';
  margin: auto;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

@keyframes load3 {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

button.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: none;
  box-sizing: border-box;
  text-align: center;
  line-height: 32px;
  height: 32px;
  padding: 0px 12px;
  letter-spacing: 0.8px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input.jp-mod-styled {
  background: var(--jp-input-background);
  height: 28px;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color1);
  padding-left: 7px;
  padding-right: 7px;
  font-size: var(--jp-ui-font-size2);
  color: var(--jp-ui-font-color0);
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

input.jp-mod-styled:focus {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-select-wrapper {
  display: flex;
  position: relative;
  flex-direction: column;
  padding: 1px;
  background-color: var(--jp-layout-color1);
  height: 28px;
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  background-color: var(--jp-layout-color1);
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0px 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  height: 32px;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0px;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toolbar-height: calc(
    28px + var(--jp-border-width)
  ); /* leave 28px for content */
}

.jp-Toolbar {
  color: var(--jp-ui-font-color1);
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: 2px;
  z-index: 1;
}

/* Toolbar items */

.jp-Toolbar > .jp-Toolbar-item.jp-Toolbar-spacer {
  flex-grow: 1;
  flex-shrink: 1;
}

.jp-Toolbar-item.jp-Toolbar-kernelStatus {
  display: inline-block;
  width: 32px;
  background-repeat: no-repeat;
  background-position: center;
  background-size: 16px;
}

.jp-Toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  display: flex;
  padding-left: 1px;
  padding-right: 1px;
  font-size: var(--jp-ui-font-size1);
  line-height: var(--jp-private-toolbar-height);
  height: 100%;
}

/* Toolbar buttons */

/* This is the div we use to wrap the react component into a Widget */
div.jp-ToolbarButton {
  color: transparent;
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0px;
  margin: 0px;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0px 6px;
  margin: 0px;
  height: 24px;
  border-radius: var(--jp-border-radius);
  display: flex;
  align-items: center;
  text-align: center;
  font-size: 14px;
  min-width: unset;
  min-height: unset;
}

button.jp-ToolbarButtonComponent:disabled {
  opacity: 0.4;
}

button.jp-ToolbarButtonComponent span {
  padding: 0px;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/


/* <DEPRECATED> */ body.p-mod-override-cursor *, /* </DEPRECATED> */
body.lm-mod-override-cursor * {
  cursor: inherit !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-JSONEditor {
  display: flex;
  flex-direction: column;
  width: 100%;
}

.jp-JSONEditor-host {
  flex: 1 1 auto;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0px;
  background: var(--jp-layout-color0);
  min-height: 50px;
  padding: 1px;
}

.jp-JSONEditor.jp-mod-error .jp-JSONEditor-host {
  border-color: red;
  outline-color: red;
}

.jp-JSONEditor-header {
  display: flex;
  flex: 1 0 auto;
  padding: 0 0 0 12px;
}

.jp-JSONEditor-header label {
  flex: 0 0 auto;
}

.jp-JSONEditor-commitButton {
  height: 16px;
  width: 16px;
  background-size: 18px;
  background-repeat: no-repeat;
  background-position: center;
}

.jp-JSONEditor-host.jp-mod-focused {
  background-color: var(--jp-input-active-background);
  border: 1px solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

.jp-Editor.jp-mod-dropTarget {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* BASICS */

.CodeMirror {
  /* Set height, width, borders, and global font properties here */
  font-family: monospace;
  height: 300px;
  color: black;
  direction: ltr;
}

/* PADDING */

.CodeMirror-lines {
  padding: 4px 0; /* Vertical padding around content */
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  padding: 0 4px; /* Horizontal padding of content */
}

.CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
  background-color: white; /* The little square between H and V scrollbars */
}

/* GUTTER */

.CodeMirror-gutters {
  border-right: 1px solid #ddd;
  background-color: #f7f7f7;
  white-space: nowrap;
}
.CodeMirror-linenumbers {}
.CodeMirror-linenumber {
  padding: 0 3px 0 5px;
  min-width: 20px;
  text-align: right;
  color: #999;
  white-space: nowrap;
}

.CodeMirror-guttermarker { color: black; }
.CodeMirror-guttermarker-subtle { color: #999; }

/* CURSOR */

.CodeMirror-cursor {
  border-left: 1px solid black;
  border-right: none;
  width: 0;
}
/* Shown when moving in bi-directional text */
.CodeMirror div.CodeMirror-secondarycursor {
  border-left: 1px solid silver;
}
.cm-fat-cursor .CodeMirror-cursor {
  width: auto;
  border: 0 !important;
  background: #7e7;
}
.cm-fat-cursor div.CodeMirror-cursors {
  z-index: 1;
}
.cm-fat-cursor-mark {
  background-color: rgba(20, 255, 20, 0.5);
  -webkit-animation: blink 1.06s steps(1) infinite;
  -moz-animation: blink 1.06s steps(1) infinite;
  animation: blink 1.06s steps(1) infinite;
}
.cm-animate-fat-cursor {
  width: auto;
  border: 0;
  -webkit-animation: blink 1.06s steps(1) infinite;
  -moz-animation: blink 1.06s steps(1) infinite;
  animation: blink 1.06s steps(1) infinite;
  background-color: #7e7;
}
@-moz-keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}
@-webkit-keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}
@keyframes blink {
  0% {}
  50% { background-color: transparent; }
  100% {}
}

/* Can style cursor different in overwrite (non-insert) mode */
.CodeMirror-overwrite .CodeMirror-cursor {}

.cm-tab { display: inline-block; text-decoration: inherit; }

.CodeMirror-rulers {
  position: absolute;
  left: 0; right: 0; top: -50px; bottom: 0;
  overflow: hidden;
}
.CodeMirror-ruler {
  border-left: 1px solid #ccc;
  top: 0; bottom: 0;
  position: absolute;
}

/* DEFAULT THEME */

.cm-s-default .cm-header {color: blue;}
.cm-s-default .cm-quote {color: #090;}
.cm-negative {color: #d44;}
.cm-positive {color: #292;}
.cm-header, .cm-strong {font-weight: bold;}
.cm-em {font-style: italic;}
.cm-link {text-decoration: underline;}
.cm-strikethrough {text-decoration: line-through;}

.cm-s-default .cm-keyword {color: #708;}
.cm-s-default .cm-atom {color: #219;}
.cm-s-default .cm-number {color: #164;}
.cm-s-default .cm-def {color: #00f;}
.cm-s-default .cm-variable,
.cm-s-default .cm-punctuation,
.cm-s-default .cm-property,
.cm-s-default .cm-operator {}
.cm-s-default .cm-variable-2 {color: #05a;}
.cm-s-default .cm-variable-3, .cm-s-default .cm-type {color: #085;}
.cm-s-default .cm-comment {color: #a50;}
.cm-s-default .cm-string {color: #a11;}
.cm-s-default .cm-string-2 {color: #f50;}
.cm-s-default .cm-meta {color: #555;}
.cm-s-default .cm-qualifier {color: #555;}
.cm-s-default .cm-builtin {color: #30a;}
.cm-s-default .cm-bracket {color: #997;}
.cm-s-default .cm-tag {color: #170;}
.cm-s-default .cm-attribute {color: #00c;}
.cm-s-default .cm-hr {color: #999;}
.cm-s-default .cm-link {color: #00c;}

.cm-s-default .cm-error {color: #f00;}
.cm-invalidchar {color: #f00;}

.CodeMirror-composing { border-bottom: 2px solid; }

/* Default styles for common addons */

div.CodeMirror span.CodeMirror-matchingbracket {color: #0b0;}
div.CodeMirror span.CodeMirror-nonmatchingbracket {color: #a22;}
.CodeMirror-matchingtag { background: rgba(255, 150, 0, .3); }
.CodeMirror-activeline-background {background: #e8f2ff;}

/* STOP */

/* The rest of this file contains styles related to the mechanics of
   the editor. You probably shouldn't touch them. */

.CodeMirror {
  position: relative;
  overflow: hidden;
  background: white;
}

.CodeMirror-scroll {
  overflow: scroll !important; /* Things will break if this is overridden */
  /* 30px is the magic margin used to hide the element's real scrollbars */
  /* See overflow: hidden in .CodeMirror */
  margin-bottom: -30px; margin-right: -30px;
  padding-bottom: 30px;
  height: 100%;
  outline: none; /* Prevent dragging from highlighting the element */
  position: relative;
}
.CodeMirror-sizer {
  position: relative;
  border-right: 30px solid transparent;
}

/* The fake, visible scrollbars. Used to force redraw during scrolling
   before actual scrolling happens, thus preventing shaking and
   flickering artifacts. */
.CodeMirror-vscrollbar, .CodeMirror-hscrollbar, .CodeMirror-scrollbar-filler, .CodeMirror-gutter-filler {
  position: absolute;
  z-index: 6;
  display: none;
}
.CodeMirror-vscrollbar {
  right: 0; top: 0;
  overflow-x: hidden;
  overflow-y: scroll;
}
.CodeMirror-hscrollbar {
  bottom: 0; left: 0;
  overflow-y: hidden;
  overflow-x: scroll;
}
.CodeMirror-scrollbar-filler {
  right: 0; bottom: 0;
}
.CodeMirror-gutter-filler {
  left: 0; bottom: 0;
}

.CodeMirror-gutters {
  position: absolute; left: 0; top: 0;
  min-height: 100%;
  z-index: 3;
}
.CodeMirror-gutter {
  white-space: normal;
  height: 100%;
  display: inline-block;
  vertical-align: top;
  margin-bottom: -30px;
}
.CodeMirror-gutter-wrapper {
  position: absolute;
  z-index: 4;
  background: none !important;
  border: none !important;
}
.CodeMirror-gutter-background {
  position: absolute;
  top: 0; bottom: 0;
  z-index: 4;
}
.CodeMirror-gutter-elt {
  position: absolute;
  cursor: default;
  z-index: 4;
}
.CodeMirror-gutter-wrapper ::selection { background-color: transparent }
.CodeMirror-gutter-wrapper ::-moz-selection { background-color: transparent }

.CodeMirror-lines {
  cursor: text;
  min-height: 1px; /* prevents collapsing before first draw */
}
.CodeMirror pre.CodeMirror-line,
.CodeMirror pre.CodeMirror-line-like {
  /* Reset some styles that the rest of the page might have set */
  -moz-border-radius: 0; -webkit-border-radius: 0; border-radius: 0;
  border-width: 0;
  background: transparent;
  font-family: inherit;
  font-size: inherit;
  margin: 0;
  white-space: pre;
  word-wrap: normal;
  line-height: inherit;
  color: inherit;
  z-index: 2;
  position: relative;
  overflow: visible;
  -webkit-tap-highlight-color: transparent;
  -webkit-font-variant-ligatures: contextual;
  font-variant-ligatures: contextual;
}
.CodeMirror-wrap pre.CodeMirror-line,
.CodeMirror-wrap pre.CodeMirror-line-like {
  word-wrap: break-word;
  white-space: pre-wrap;
  word-break: normal;
}

.CodeMirror-linebackground {
  position: absolute;
  left: 0; right: 0; top: 0; bottom: 0;
  z-index: 0;
}

.CodeMirror-linewidget {
  position: relative;
  z-index: 2;
  padding: 0.1px; /* Force widget margins to stay inside of the container */
}

.CodeMirror-widget {}

.CodeMirror-rtl pre { direction: rtl; }

.CodeMirror-code {
  outline: none;
}

/* Force content-box sizing for the elements where we expect it */
.CodeMirror-scroll,
.CodeMirror-sizer,
.CodeMirror-gutter,
.CodeMirror-gutters,
.CodeMirror-linenumber {
  -moz-box-sizing: content-box;
  box-sizing: content-box;
}

.CodeMirror-measure {
  position: absolute;
  width: 100%;
  height: 0;
  overflow: hidden;
  visibility: hidden;
}

.CodeMirror-cursor {
  position: absolute;
  pointer-events: none;
}
.CodeMirror-measure pre { position: static; }

div.CodeMirror-cursors {
  visibility: hidden;
  position: relative;
  z-index: 3;
}
div.CodeMirror-dragcursors {
  visibility: visible;
}

.CodeMirror-focused div.CodeMirror-cursors {
  visibility: visible;
}

.CodeMirror-selected { background: #d9d9d9; }
.CodeMirror-focused .CodeMirror-selected { background: #d7d4f0; }
.CodeMirror-crosshair { cursor: crosshair; }
.CodeMirror-line::selection, .CodeMirror-line > span::selection, .CodeMirror-line > span > span::selection { background: #d7d4f0; }
.CodeMirror-line::-moz-selection, .CodeMirror-line > span::-moz-selection, .CodeMirror-line > span > span::-moz-selection { background: #d7d4f0; }

.cm-searching {
  background-color: #ffa;
  background-color: rgba(255, 255, 0, .4);
}

/* Used to force a border model for a node */
.cm-force-border { padding-right: .1px; }

@media print {
  /* Hide the cursor when printing */
  .CodeMirror div.CodeMirror-cursors {
    visibility: hidden;
  }
}

/* See issue #2901 */
.cm-tab-wrap-hack:after { content: ''; }

/* Help users use markselection to safely style text background */
span.CodeMirror-selectedtext { background: none; }

.CodeMirror-dialog {
  position: absolute;
  left: 0; right: 0;
  background: inherit;
  z-index: 15;
  padding: .1em .8em;
  overflow: hidden;
  color: inherit;
}

.CodeMirror-dialog-top {
  border-bottom: 1px solid #eee;
  top: 0;
}

.CodeMirror-dialog-bottom {
  border-top: 1px solid #eee;
  bottom: 0;
}

.CodeMirror-dialog input {
  border: none;
  outline: none;
  background: transparent;
  width: 20em;
  color: inherit;
  font-family: monospace;
}

.CodeMirror-dialog button {
  font-size: 70%;
}

.CodeMirror-foldmarker {
  color: blue;
  text-shadow: #b9f 1px 1px 2px, #b9f -1px -1px 2px, #b9f 1px -1px 2px, #b9f -1px 1px 2px;
  font-family: arial;
  line-height: .3;
  cursor: pointer;
}
.CodeMirror-foldgutter {
  width: .7em;
}
.CodeMirror-foldgutter-open,
.CodeMirror-foldgutter-folded {
  cursor: pointer;
}
.CodeMirror-foldgutter-open:after {
  content: "\25BE";
}
.CodeMirror-foldgutter-folded:after {
  content: "\25B8";
}

/*
  Name:       material
  Author:     Mattia Astorino (http://github.com/equinusocio)
  Website:    https://material-theme.site/
*/

.cm-s-material.CodeMirror {
  background-color: #263238;
  color: #EEFFFF;
}

.cm-s-material .CodeMirror-gutters {
  background: #263238;
  color: #546E7A;
  border: none;
}

.cm-s-material .CodeMirror-guttermarker,
.cm-s-material .CodeMirror-guttermarker-subtle,
.cm-s-material .CodeMirror-linenumber {
  color: #546E7A;
}

.cm-s-material .CodeMirror-cursor {
  border-left: 1px solid #FFCC00;
}

.cm-s-material div.CodeMirror-selected {
  background: rgba(128, 203, 196, 0.2);
}

.cm-s-material.CodeMirror-focused div.CodeMirror-selected {
  background: rgba(128, 203, 196, 0.2);
}

.cm-s-material .CodeMirror-line::selection,
.cm-s-material .CodeMirror-line>span::selection,
.cm-s-material .CodeMirror-line>span>span::selection {
  background: rgba(128, 203, 196, 0.2);
}

.cm-s-material .CodeMirror-line::-moz-selection,
.cm-s-material .CodeMirror-line>span::-moz-selection,
.cm-s-material .CodeMirror-line>span>span::-moz-selection {
  background: rgba(128, 203, 196, 0.2);
}

.cm-s-material .CodeMirror-activeline-background {
  background: rgba(0, 0, 0, 0.5);
}

.cm-s-material .cm-keyword {
  color: #C792EA;
}

.cm-s-material .cm-operator {
  color: #89DDFF;
}

.cm-s-material .cm-variable-2 {
  color: #EEFFFF;
}

.cm-s-material .cm-variable-3,
.cm-s-material .cm-type {
  color: #f07178;
}

.cm-s-material .cm-builtin {
  color: #FFCB6B;
}

.cm-s-material .cm-atom {
  color: #F78C6C;
}

.cm-s-material .cm-number {
  color: #FF5370;
}

.cm-s-material .cm-def {
  color: #82AAFF;
}

.cm-s-material .cm-string {
  color: #C3E88D;
}

.cm-s-material .cm-string-2 {
  color: #f07178;
}

.cm-s-material .cm-comment {
  color: #546E7A;
}

.cm-s-material .cm-variable {
  color: #f07178;
}

.cm-s-material .cm-tag {
  color: #FF5370;
}

.cm-s-material .cm-meta {
  color: #FFCB6B;
}

.cm-s-material .cm-attribute {
  color: #C792EA;
}

.cm-s-material .cm-property {
  color: #C792EA;
}

.cm-s-material .cm-qualifier {
  color: #DECB6B;
}

.cm-s-material .cm-variable-3,
.cm-s-material .cm-type {
  color: #DECB6B;
}


.cm-s-material .cm-error {
  color: rgba(255, 255, 255, 1.0);
  background-color: #FF5370;
}

.cm-s-material .CodeMirror-matchingbracket {
  text-decoration: underline;
  color: white !important;
}
/**
 * "
 *  Using Zenburn color palette from the Emacs Zenburn Theme
 *  https://github.com/bbatsov/zenburn-emacs/blob/master/zenburn-theme.el
 *
 *  Also using parts of https://github.com/xavi/coderay-lighttable-theme
 * "
 * From: https://github.com/wisenomad/zenburn-lighttable-theme/blob/master/zenburn.css
 */

.cm-s-zenburn .CodeMirror-gutters { background: #3f3f3f !important; }
.cm-s-zenburn .CodeMirror-foldgutter-open, .CodeMirror-foldgutter-folded { color: #999; }
.cm-s-zenburn .CodeMirror-cursor { border-left: 1px solid white; }
.cm-s-zenburn { background-color: #3f3f3f; color: #dcdccc; }
.cm-s-zenburn span.cm-builtin { color: #dcdccc; font-weight: bold; }
.cm-s-zenburn span.cm-comment { color: #7f9f7f; }
.cm-s-zenburn span.cm-keyword { color: #f0dfaf; font-weight: bold; }
.cm-s-zenburn span.cm-atom { color: #bfebbf; }
.cm-s-zenburn span.cm-def { color: #dcdccc; }
.cm-s-zenburn span.cm-variable { color: #dfaf8f; }
.cm-s-zenburn span.cm-variable-2 { color: #dcdccc; }
.cm-s-zenburn span.cm-string { color: #cc9393; }
.cm-s-zenburn span.cm-string-2 { color: #cc9393; }
.cm-s-zenburn span.cm-number { color: #dcdccc; }
.cm-s-zenburn span.cm-tag { color: #93e0e3; }
.cm-s-zenburn span.cm-property { color: #dfaf8f; }
.cm-s-zenburn span.cm-attribute { color: #dfaf8f; }
.cm-s-zenburn span.cm-qualifier { color: #7cb8bb; }
.cm-s-zenburn span.cm-meta { color: #f0dfaf; }
.cm-s-zenburn span.cm-header { color: #f0efd0; }
.cm-s-zenburn span.cm-operator { color: #f0efd0; }
.cm-s-zenburn span.CodeMirror-matchingbracket { box-sizing: border-box; background: transparent; border-bottom: 1px solid; }
.cm-s-zenburn span.CodeMirror-nonmatchingbracket { border-bottom: 1px solid; background: none; }
.cm-s-zenburn .CodeMirror-activeline { background: #000000; }
.cm-s-zenburn .CodeMirror-activeline-background { background: #000000; }
.cm-s-zenburn div.CodeMirror-selected { background: #545454; }
.cm-s-zenburn .CodeMirror-focused div.CodeMirror-selected { background: #4f4f4f; }

.cm-s-abcdef.CodeMirror { background: #0f0f0f; color: #defdef; }
.cm-s-abcdef div.CodeMirror-selected { background: #515151; }
.cm-s-abcdef .CodeMirror-line::selection, .cm-s-abcdef .CodeMirror-line > span::selection, .cm-s-abcdef .CodeMirror-line > span > span::selection { background: rgba(56, 56, 56, 0.99); }
.cm-s-abcdef .CodeMirror-line::-moz-selection, .cm-s-abcdef .CodeMirror-line > span::-moz-selection, .cm-s-abcdef .CodeMirror-line > span > span::-moz-selection { background: rgba(56, 56, 56, 0.99); }
.cm-s-abcdef .CodeMirror-gutters { background: #555; border-right: 2px solid #314151; }
.cm-s-abcdef .CodeMirror-guttermarker { color: #222; }
.cm-s-abcdef .CodeMirror-guttermarker-subtle { color: azure; }
.cm-s-abcdef .CodeMirror-linenumber { color: #FFFFFF; }
.cm-s-abcdef .CodeMirror-cursor { border-left: 1px solid #00FF00; }

.cm-s-abcdef span.cm-keyword { color: darkgoldenrod; font-weight: bold; }
.cm-s-abcdef span.cm-atom { color: #77F; }
.cm-s-abcdef span.cm-number { color: violet; }
.cm-s-abcdef span.cm-def { color: #fffabc; }
.cm-s-abcdef span.cm-variable { color: #abcdef; }
.cm-s-abcdef span.cm-variable-2 { color: #cacbcc; }
.cm-s-abcdef span.cm-variable-3, .cm-s-abcdef span.cm-type { color: #def; }
.cm-s-abcdef span.cm-property { color: #fedcba; }
.cm-s-abcdef span.cm-operator { color: #ff0; }
.cm-s-abcdef span.cm-comment { color: #7a7b7c; font-style: italic;}
.cm-s-abcdef span.cm-string { color: #2b4; }
.cm-s-abcdef span.cm-meta { color: #C9F; }
.cm-s-abcdef span.cm-qualifier { color: #FFF700; }
.cm-s-abcdef span.cm-builtin { color: #30aabc; }
.cm-s-abcdef span.cm-bracket { color: #8a8a8a; }
.cm-s-abcdef span.cm-tag { color: #FFDD44; }
.cm-s-abcdef span.cm-attribute { color: #DDFF00; }
.cm-s-abcdef span.cm-error { color: #FF0000; }
.cm-s-abcdef span.cm-header { color: aquamarine; font-weight: bold; }
.cm-s-abcdef span.cm-link { color: blueviolet; }

.cm-s-abcdef .CodeMirror-activeline-background { background: #314151; }

/*

    Name:       Base16 Default Light
    Author:     Chris Kempson (http://chriskempson.com)

    CodeMirror template by Jan T. Sott (https://github.com/idleberg/base16-codemirror)
    Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16)

*/

.cm-s-base16-light.CodeMirror { background: #f5f5f5; color: #202020; }
.cm-s-base16-light div.CodeMirror-selected { background: #e0e0e0; }
.cm-s-base16-light .CodeMirror-line::selection, .cm-s-base16-light .CodeMirror-line > span::selection, .cm-s-base16-light .CodeMirror-line > span > span::selection { background: #e0e0e0; }
.cm-s-base16-light .CodeMirror-line::-moz-selection, .cm-s-base16-light .CodeMirror-line > span::-moz-selection, .cm-s-base16-light .CodeMirror-line > span > span::-moz-selection { background: #e0e0e0; }
.cm-s-base16-light .CodeMirror-gutters { background: #f5f5f5; border-right: 0px; }
.cm-s-base16-light .CodeMirror-guttermarker { color: #ac4142; }
.cm-s-base16-light .CodeMirror-guttermarker-subtle { color: #b0b0b0; }
.cm-s-base16-light .CodeMirror-linenumber { color: #b0b0b0; }
.cm-s-base16-light .CodeMirror-cursor { border-left: 1px solid #505050; }

.cm-s-base16-light span.cm-comment { color: #8f5536; }
.cm-s-base16-light span.cm-atom { color: #aa759f; }
.cm-s-base16-light span.cm-number { color: #aa759f; }

.cm-s-base16-light span.cm-property, .cm-s-base16-light span.cm-attribute { color: #90a959; }
.cm-s-base16-light span.cm-keyword { color: #ac4142; }
.cm-s-base16-light span.cm-string { color: #f4bf75; }

.cm-s-base16-light span.cm-variable { color: #90a959; }
.cm-s-base16-light span.cm-variable-2 { color: #6a9fb5; }
.cm-s-base16-light span.cm-def { color: #d28445; }
.cm-s-base16-light span.cm-bracket { color: #202020; }
.cm-s-base16-light span.cm-tag { color: #ac4142; }
.cm-s-base16-light span.cm-link { color: #aa759f; }
.cm-s-base16-light span.cm-error { background: #ac4142; color: #505050; }

.cm-s-base16-light .CodeMirror-activeline-background { background: #DDDCDC; }
.cm-s-base16-light .CodeMirror-matchingbracket { color: #f5f5f5 !important; background-color: #6A9FB5 !important}

/*

    Name:       Base16 Default Dark
    Author:     Chris Kempson (http://chriskempson.com)

    CodeMirror template by Jan T. Sott (https://github.com/idleberg/base16-codemirror)
    Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16)

*/

.cm-s-base16-dark.CodeMirror { background: #151515; color: #e0e0e0; }
.cm-s-base16-dark div.CodeMirror-selected { background: #303030; }
.cm-s-base16-dark .CodeMirror-line::selection, .cm-s-base16-dark .CodeMirror-line > span::selection, .cm-s-base16-dark .CodeMirror-line > span > span::selection { background: rgba(48, 48, 48, .99); }
.cm-s-base16-dark .CodeMirror-line::-moz-selection, .cm-s-base16-dark .CodeMirror-line > span::-moz-selection, .cm-s-base16-dark .CodeMirror-line > span > span::-moz-selection { background: rgba(48, 48, 48, .99); }
.cm-s-base16-dark .CodeMirror-gutters { background: #151515; border-right: 0px; }
.cm-s-base16-dark .CodeMirror-guttermarker { color: #ac4142; }
.cm-s-base16-dark .CodeMirror-guttermarker-subtle { color: #505050; }
.cm-s-base16-dark .CodeMirror-linenumber { color: #505050; }
.cm-s-base16-dark .CodeMirror-cursor { border-left: 1px solid #b0b0b0; }

.cm-s-base16-dark span.cm-comment { color: #8f5536; }
.cm-s-base16-dark span.cm-atom { color: #aa759f; }
.cm-s-base16-dark span.cm-number { color: #aa759f; }

.cm-s-base16-dark span.cm-property, .cm-s-base16-dark span.cm-attribute { color: #90a959; }
.cm-s-base16-dark span.cm-keyword { color: #ac4142; }
.cm-s-base16-dark span.cm-string { color: #f4bf75; }

.cm-s-base16-dark span.cm-variable { color: #90a959; }
.cm-s-base16-dark span.cm-variable-2 { color: #6a9fb5; }
.cm-s-base16-dark span.cm-def { color: #d28445; }
.cm-s-base16-dark span.cm-bracket { color: #e0e0e0; }
.cm-s-base16-dark span.cm-tag { color: #ac4142; }
.cm-s-base16-dark span.cm-link { color: #aa759f; }
.cm-s-base16-dark span.cm-error { background: #ac4142; color: #b0b0b0; }

.cm-s-base16-dark .CodeMirror-activeline-background { background: #202020; }
.cm-s-base16-dark .CodeMirror-matchingbracket { text-decoration: underline; color: white !important; }

/*

    Name:       dracula
    Author:     Michael Kaminsky (http://github.com/mkaminsky11)

    Original dracula color scheme by Zeno Rocha (https://github.com/zenorocha/dracula-theme)

*/


.cm-s-dracula.CodeMirror, .cm-s-dracula .CodeMirror-gutters {
  background-color: #282a36 !important;
  color: #f8f8f2 !important;
  border: none;
}
.cm-s-dracula .CodeMirror-gutters { color: #282a36; }
.cm-s-dracula .CodeMirror-cursor { border-left: solid thin #f8f8f0; }
.cm-s-dracula .CodeMirror-linenumber { color: #6D8A88; }
.cm-s-dracula .CodeMirror-selected { background: rgba(255, 255, 255, 0.10); }
.cm-s-dracula .CodeMirror-line::selection, .cm-s-dracula .CodeMirror-line > span::selection, .cm-s-dracula .CodeMirror-line > span > span::selection { background: rgba(255, 255, 255, 0.10); }
.cm-s-dracula .CodeMirror-line::-moz-selection, .cm-s-dracula .CodeMirror-line > span::-moz-selection, .cm-s-dracula .CodeMirror-line > span > span::-moz-selection { background: rgba(255, 255, 255, 0.10); }
.cm-s-dracula span.cm-comment { color: #6272a4; }
.cm-s-dracula span.cm-string, .cm-s-dracula span.cm-string-2 { color: #f1fa8c; }
.cm-s-dracula span.cm-number { color: #bd93f9; }
.cm-s-dracula span.cm-variable { color: #50fa7b; }
.cm-s-dracula span.cm-variable-2 { color: white; }
.cm-s-dracula span.cm-def { color: #50fa7b; }
.cm-s-dracula span.cm-operator { color: #ff79c6; }
.cm-s-dracula span.cm-keyword { color: #ff79c6; }
.cm-s-dracula span.cm-atom { color: #bd93f9; }
.cm-s-dracula span.cm-meta { color: #f8f8f2; }
.cm-s-dracula span.cm-tag { color: #ff79c6; }
.cm-s-dracula span.cm-attribute { color: #50fa7b; }
.cm-s-dracula span.cm-qualifier { color: #50fa7b; }
.cm-s-dracula span.cm-property { color: #66d9ef; }
.cm-s-dracula span.cm-builtin { color: #50fa7b; }
.cm-s-dracula span.cm-variable-3, .cm-s-dracula span.cm-type { color: #ffb86c; }

.cm-s-dracula .CodeMirror-activeline-background { background: rgba(255,255,255,0.1); }
.cm-s-dracula .CodeMirror-matchingbracket { text-decoration: underline; color: white !important; }

/*

    Name:       Hopscotch
    Author:     Jan T. Sott

    CodeMirror template by Jan T. Sott (https://github.com/idleberg/base16-codemirror)
    Original Base16 color scheme by Chris Kempson (https://github.com/chriskempson/base16)

*/

.cm-s-hopscotch.CodeMirror {background: #322931; color: #d5d3d5;}
.cm-s-hopscotch div.CodeMirror-selected {background: #433b42 !important;}
.cm-s-hopscotch .CodeMirror-gutters {background: #322931; border-right: 0px;}
.cm-s-hopscotch .CodeMirror-linenumber {color: #797379;}
.cm-s-hopscotch .CodeMirror-cursor {border-left: 1px solid #989498 !important;}

.cm-s-hopscotch span.cm-comment {color: #b33508;}
.cm-s-hopscotch span.cm-atom {color: #c85e7c;}
.cm-s-hopscotch span.cm-number {color: #c85e7c;}

.cm-s-hopscotch span.cm-property, .cm-s-hopscotch span.cm-attribute {color: #8fc13e;}
.cm-s-hopscotch span.cm-keyword {color: #dd464c;}
.cm-s-hopscotch span.cm-string {color: #fdcc59;}

.cm-s-hopscotch span.cm-variable {color: #8fc13e;}
.cm-s-hopscotch span.cm-variable-2 {color: #1290bf;}
.cm-s-hopscotch span.cm-def {color: #fd8b19;}
.cm-s-hopscotch span.cm-error {background: #dd464c; color: #989498;}
.cm-s-hopscotch span.cm-bracket {color: #d5d3d5;}
.cm-s-hopscotch span.cm-tag {color: #dd464c;}
.cm-s-hopscotch span.cm-link {color: #c85e7c;}

.cm-s-hopscotch .CodeMirror-matchingbracket { text-decoration: underline; color: white !important;}
.cm-s-hopscotch .CodeMirror-activeline-background { background: #302020; }

/****************************************************************/
/*   Based on mbonaci's Brackets mbo theme                      */
/*   https://github.com/mbonaci/global/blob/master/Mbo.tmTheme  */
/*   Create your own: http://tmtheme-editor.herokuapp.com       */
/****************************************************************/

.cm-s-mbo.CodeMirror { background: #2c2c2c; color: #ffffec; }
.cm-s-mbo div.CodeMirror-selected { background: #716C62; }
.cm-s-mbo .CodeMirror-line::selection, .cm-s-mbo .CodeMirror-line > span::selection, .cm-s-mbo .CodeMirror-line > span > span::selection { background: rgba(113, 108, 98, .99); }
.cm-s-mbo .CodeMirror-line::-moz-selection, .cm-s-mbo .CodeMirror-line > span::-moz-selection, .cm-s-mbo .CodeMirror-line > span > span::-moz-selection { background: rgba(113, 108, 98, .99); }
.cm-s-mbo .CodeMirror-gutters { background: #4e4e4e; border-right: 0px; }
.cm-s-mbo .CodeMirror-guttermarker { color: white; }
.cm-s-mbo .CodeMirror-guttermarker-subtle { color: grey; }
.cm-s-mbo .CodeMirror-linenumber { color: #dadada; }
.cm-s-mbo .CodeMirror-cursor { border-left: 1px solid #ffffec; }

.cm-s-mbo span.cm-comment { color: #95958a; }
.cm-s-mbo span.cm-atom { color: #00a8c6; }
.cm-s-mbo span.cm-number { color: #00a8c6; }

.cm-s-mbo span.cm-property, .cm-s-mbo span.cm-attribute { color: #9ddfe9; }
.cm-s-mbo span.cm-keyword { color: #ffb928; }
.cm-s-mbo span.cm-string { color: #ffcf6c; }
.cm-s-mbo span.cm-string.cm-property { color: #ffffec; }

.cm-s-mbo span.cm-variable { color: #ffffec; }
.cm-s-mbo span.cm-variable-2 { color: #00a8c6; }
.cm-s-mbo span.cm-def { color: #ffffec; }
.cm-s-mbo span.cm-bracket { color: #fffffc; font-weight: bold; }
.cm-s-mbo span.cm-tag { color: #9ddfe9; }
.cm-s-mbo span.cm-link { color: #f54b07; }
.cm-s-mbo span.cm-error { border-bottom: #636363; color: #ffffec; }
.cm-s-mbo span.cm-qualifier { color: #ffffec; }

.cm-s-mbo .CodeMirror-activeline-background { background: #494b41; }
.cm-s-mbo .CodeMirror-matchingbracket { color: #ffb928 !important; }
.cm-s-mbo .CodeMirror-matchingtag { background: rgba(255, 255, 255, .37); }

/*
  MDN-LIKE Theme - Mozilla
  Ported to CodeMirror by Peter Kroon <plakroon@gmail.com>
  Report bugs/issues here: https://github.com/codemirror/CodeMirror/issues
  GitHub: @peterkroon

  The mdn-like theme is inspired on the displayed code examples at: https://developer.mozilla.org/en-US/docs/Web/CSS/animation

*/
.cm-s-mdn-like.CodeMirror { color: #999; background-color: #fff; }
.cm-s-mdn-like div.CodeMirror-selected { background: #cfc; }
.cm-s-mdn-like .CodeMirror-line::selection, .cm-s-mdn-like .CodeMirror-line > span::selection, .cm-s-mdn-like .CodeMirror-line > span > span::selection { background: #cfc; }
.cm-s-mdn-like .CodeMirror-line::-moz-selection, .cm-s-mdn-like .CodeMirror-line > span::-moz-selection, .cm-s-mdn-like .CodeMirror-line > span > span::-moz-selection { background: #cfc; }

.cm-s-mdn-like .CodeMirror-gutters { background: #f8f8f8; border-left: 6px solid rgba(0,83,159,0.65); color: #333; }
.cm-s-mdn-like .CodeMirror-linenumber { color: #aaa; padding-left: 8px; }
.cm-s-mdn-like .CodeMirror-cursor { border-left: 2px solid #222; }

.cm-s-mdn-like .cm-keyword { color: #6262FF; }
.cm-s-mdn-like .cm-atom { color: #F90; }
.cm-s-mdn-like .cm-number { color:  #ca7841; }
.cm-s-mdn-like .cm-def { color: #8DA6CE; }
.cm-s-mdn-like span.cm-variable-2, .cm-s-mdn-like span.cm-tag { color: #690; }
.cm-s-mdn-like span.cm-variable-3, .cm-s-mdn-like span.cm-def, .cm-s-mdn-like span.cm-type { color: #07a; }

.cm-s-mdn-like .cm-variable { color: #07a; }
.cm-s-mdn-like .cm-property { color: #905; }
.cm-s-mdn-like .cm-qualifier { color: #690; }

.cm-s-mdn-like .cm-operator { color: #cda869; }
.cm-s-mdn-like .cm-comment { color:#777; font-weight:normal; }
.cm-s-mdn-like .cm-string { color:#07a; font-style:italic; }
.cm-s-mdn-like .cm-string-2 { color:#bd6b18; } /*?*/
.cm-s-mdn-like .cm-meta { color: #000; } /*?*/
.cm-s-mdn-like .cm-builtin { color: #9B7536; } /*?*/
.cm-s-mdn-like .cm-tag { color: #997643; }
.cm-s-mdn-like .cm-attribute { color: #d6bb6d; } /*?*/
.cm-s-mdn-like .cm-header { color: #FF6400; }
.cm-s-mdn-like .cm-hr { color: #AEAEAE; }
.cm-s-mdn-like .cm-link { color:#ad9361; font-style:italic; text-decoration:none; }
.cm-s-mdn-like .cm-error { border-bottom: 1px solid red; }

div.cm-s-mdn-like .CodeMirror-activeline-background { background: #efefff; }
div.cm-s-mdn-like span.CodeMirror-matchingbracket { outline:1px solid grey; color: inherit; }

.cm-s-mdn-like.CodeMirror { background-image: url(data:image/png;base64,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); }

/*

    Name:       seti
    Author:     Michael Kaminsky (http://github.com/mkaminsky11)

    Original seti color scheme by Jesse Weed (https://github.com/jesseweed/seti-syntax)

*/


.cm-s-seti.CodeMirror {
  background-color: #151718 !important;
  color: #CFD2D1 !important;
  border: none;
}
.cm-s-seti .CodeMirror-gutters {
  color: #404b53;
  background-color: #0E1112;
  border: none;
}
.cm-s-seti .CodeMirror-cursor { border-left: solid thin #f8f8f0; }
.cm-s-seti .CodeMirror-linenumber { color: #6D8A88; }
.cm-s-seti.CodeMirror-focused div.CodeMirror-selected { background: rgba(255, 255, 255, 0.10); }
.cm-s-seti .CodeMirror-line::selection, .cm-s-seti .CodeMirror-line > span::selection, .cm-s-seti .CodeMirror-line > span > span::selection { background: rgba(255, 255, 255, 0.10); }
.cm-s-seti .CodeMirror-line::-moz-selection, .cm-s-seti .CodeMirror-line > span::-moz-selection, .cm-s-seti .CodeMirror-line > span > span::-moz-selection { background: rgba(255, 255, 255, 0.10); }
.cm-s-seti span.cm-comment { color: #41535b; }
.cm-s-seti span.cm-string, .cm-s-seti span.cm-string-2 { color: #55b5db; }
.cm-s-seti span.cm-number { color: #cd3f45; }
.cm-s-seti span.cm-variable { color: #55b5db; }
.cm-s-seti span.cm-variable-2 { color: #a074c4; }
.cm-s-seti span.cm-def { color: #55b5db; }
.cm-s-seti span.cm-keyword { color: #ff79c6; }
.cm-s-seti span.cm-operator { color: #9fca56; }
.cm-s-seti span.cm-keyword { color: #e6cd69; }
.cm-s-seti span.cm-atom { color: #cd3f45; }
.cm-s-seti span.cm-meta { color: #55b5db; }
.cm-s-seti span.cm-tag { color: #55b5db; }
.cm-s-seti span.cm-attribute { color: #9fca56; }
.cm-s-seti span.cm-qualifier { color: #9fca56; }
.cm-s-seti span.cm-property { color: #a074c4; }
.cm-s-seti span.cm-variable-3, .cm-s-seti span.cm-type { color: #9fca56; }
.cm-s-seti span.cm-builtin { color: #9fca56; }
.cm-s-seti .CodeMirror-activeline-background { background: #101213; }
.cm-s-seti .CodeMirror-matchingbracket { text-decoration: underline; color: white !important; }

/*
Solarized theme for code-mirror
http://ethanschoonover.com/solarized
*/

/*
Solarized color palette
http://ethanschoonover.com/solarized/img/solarized-palette.png
*/

.solarized.base03 { color: #002b36; }
.solarized.base02 { color: #073642; }
.solarized.base01 { color: #586e75; }
.solarized.base00 { color: #657b83; }
.solarized.base0 { color: #839496; }
.solarized.base1 { color: #93a1a1; }
.solarized.base2 { color: #eee8d5; }
.solarized.base3  { color: #fdf6e3; }
.solarized.solar-yellow  { color: #b58900; }
.solarized.solar-orange  { color: #cb4b16; }
.solarized.solar-red { color: #dc322f; }
.solarized.solar-magenta { color: #d33682; }
.solarized.solar-violet  { color: #6c71c4; }
.solarized.solar-blue { color: #268bd2; }
.solarized.solar-cyan { color: #2aa198; }
.solarized.solar-green { color: #859900; }

/* Color scheme for code-mirror */

.cm-s-solarized {
  line-height: 1.45em;
  color-profile: sRGB;
  rendering-intent: auto;
}
.cm-s-solarized.cm-s-dark {
  color: #839496;
  background-color: #002b36;
  text-shadow: #002b36 0 1px;
}
.cm-s-solarized.cm-s-light {
  background-color: #fdf6e3;
  color: #657b83;
  text-shadow: #eee8d5 0 1px;
}

.cm-s-solarized .CodeMirror-widget {
  text-shadow: none;
}

.cm-s-solarized .cm-header { color: #586e75; }
.cm-s-solarized .cm-quote { color: #93a1a1; }

.cm-s-solarized .cm-keyword { color: #cb4b16; }
.cm-s-solarized .cm-atom { color: #d33682; }
.cm-s-solarized .cm-number { color: #d33682; }
.cm-s-solarized .cm-def { color: #2aa198; }

.cm-s-solarized .cm-variable { color: #839496; }
.cm-s-solarized .cm-variable-2 { color: #b58900; }
.cm-s-solarized .cm-variable-3, .cm-s-solarized .cm-type { color: #6c71c4; }

.cm-s-solarized .cm-property { color: #2aa198; }
.cm-s-solarized .cm-operator { color: #6c71c4; }

.cm-s-solarized .cm-comment { color: #586e75; font-style:italic; }

.cm-s-solarized .cm-string { color: #859900; }
.cm-s-solarized .cm-string-2 { color: #b58900; }

.cm-s-solarized .cm-meta { color: #859900; }
.cm-s-solarized .cm-qualifier { color: #b58900; }
.cm-s-solarized .cm-builtin { color: #d33682; }
.cm-s-solarized .cm-bracket { color: #cb4b16; }
.cm-s-solarized .CodeMirror-matchingbracket { color: #859900; }
.cm-s-solarized .CodeMirror-nonmatchingbracket { color: #dc322f; }
.cm-s-solarized .cm-tag { color: #93a1a1; }
.cm-s-solarized .cm-attribute { color: #2aa198; }
.cm-s-solarized .cm-hr {
  color: transparent;
  border-top: 1px solid #586e75;
  display: block;
}
.cm-s-solarized .cm-link { color: #93a1a1; cursor: pointer; }
.cm-s-solarized .cm-special { color: #6c71c4; }
.cm-s-solarized .cm-em {
  color: #999;
  text-decoration: underline;
  text-decoration-style: dotted;
}
.cm-s-solarized .cm-error,
.cm-s-solarized .cm-invalidchar {
  color: #586e75;
  border-bottom: 1px dotted #dc322f;
}

.cm-s-solarized.cm-s-dark div.CodeMirror-selected { background: #073642; }
.cm-s-solarized.cm-s-dark.CodeMirror ::selection { background: rgba(7, 54, 66, 0.99); }
.cm-s-solarized.cm-s-dark .CodeMirror-line::-moz-selection, .cm-s-dark .CodeMirror-line > span::-moz-selection, .cm-s-dark .CodeMirror-line > span > span::-moz-selection { background: rgba(7, 54, 66, 0.99); }

.cm-s-solarized.cm-s-light div.CodeMirror-selected { background: #eee8d5; }
.cm-s-solarized.cm-s-light .CodeMirror-line::selection, .cm-s-light .CodeMirror-line > span::selection, .cm-s-light .CodeMirror-line > span > span::selection { background: #eee8d5; }
.cm-s-solarized.cm-s-light .CodeMirror-line::-moz-selection, .cm-s-ligh .CodeMirror-line > span::-moz-selection, .cm-s-ligh .CodeMirror-line > span > span::-moz-selection { background: #eee8d5; }

/* Editor styling */



/* Little shadow on the view-port of the buffer view */
.cm-s-solarized.CodeMirror {
  -moz-box-shadow: inset 7px 0 12px -6px #000;
  -webkit-box-shadow: inset 7px 0 12px -6px #000;
  box-shadow: inset 7px 0 12px -6px #000;
}

/* Remove gutter border */
.cm-s-solarized .CodeMirror-gutters {
  border-right: 0;
}

/* Gutter colors and line number styling based of color scheme (dark / light) */

/* Dark */
.cm-s-solarized.cm-s-dark .CodeMirror-gutters {
  background-color: #073642;
}

.cm-s-solarized.cm-s-dark .CodeMirror-linenumber {
  color: #586e75;
  text-shadow: #021014 0 -1px;
}

/* Light */
.cm-s-solarized.cm-s-light .CodeMirror-gutters {
  background-color: #eee8d5;
}

.cm-s-solarized.cm-s-light .CodeMirror-linenumber {
  color: #839496;
}

/* Common */
.cm-s-solarized .CodeMirror-linenumber {
  padding: 0 5px;
}
.cm-s-solarized .CodeMirror-guttermarker-subtle { color: #586e75; }
.cm-s-solarized.cm-s-dark .CodeMirror-guttermarker { color: #ddd; }
.cm-s-solarized.cm-s-light .CodeMirror-guttermarker { color: #cb4b16; }

.cm-s-solarized .CodeMirror-gutter .CodeMirror-gutter-text {
  color: #586e75;
}

/* Cursor */
.cm-s-solarized .CodeMirror-cursor { border-left: 1px solid #819090; }

/* Fat cursor */
.cm-s-solarized.cm-s-light.cm-fat-cursor .CodeMirror-cursor { background: #77ee77; }
.cm-s-solarized.cm-s-light .cm-animate-fat-cursor { background-color: #77ee77; }
.cm-s-solarized.cm-s-dark.cm-fat-cursor .CodeMirror-cursor { background: #586e75; }
.cm-s-solarized.cm-s-dark .cm-animate-fat-cursor { background-color: #586e75; }

/* Active line */
.cm-s-solarized.cm-s-dark .CodeMirror-activeline-background {
  background: rgba(255, 255, 255, 0.06);
}
.cm-s-solarized.cm-s-light .CodeMirror-activeline-background {
  background: rgba(0, 0, 0, 0.06);
}

.cm-s-the-matrix.CodeMirror { background: #000000; color: #00FF00; }
.cm-s-the-matrix div.CodeMirror-selected { background: #2D2D2D; }
.cm-s-the-matrix .CodeMirror-line::selection, .cm-s-the-matrix .CodeMirror-line > span::selection, .cm-s-the-matrix .CodeMirror-line > span > span::selection { background: rgba(45, 45, 45, 0.99); }
.cm-s-the-matrix .CodeMirror-line::-moz-selection, .cm-s-the-matrix .CodeMirror-line > span::-moz-selection, .cm-s-the-matrix .CodeMirror-line > span > span::-moz-selection { background: rgba(45, 45, 45, 0.99); }
.cm-s-the-matrix .CodeMirror-gutters { background: #060; border-right: 2px solid #00FF00; }
.cm-s-the-matrix .CodeMirror-guttermarker { color: #0f0; }
.cm-s-the-matrix .CodeMirror-guttermarker-subtle { color: white; }
.cm-s-the-matrix .CodeMirror-linenumber { color: #FFFFFF; }
.cm-s-the-matrix .CodeMirror-cursor { border-left: 1px solid #00FF00; }

.cm-s-the-matrix span.cm-keyword { color: #008803; font-weight: bold; }
.cm-s-the-matrix span.cm-atom { color: #3FF; }
.cm-s-the-matrix span.cm-number { color: #FFB94F; }
.cm-s-the-matrix span.cm-def { color: #99C; }
.cm-s-the-matrix span.cm-variable { color: #F6C; }
.cm-s-the-matrix span.cm-variable-2 { color: #C6F; }
.cm-s-the-matrix span.cm-variable-3, .cm-s-the-matrix span.cm-type { color: #96F; }
.cm-s-the-matrix span.cm-property { color: #62FFA0; }
.cm-s-the-matrix span.cm-operator { color: #999; }
.cm-s-the-matrix span.cm-comment { color: #CCCCCC; }
.cm-s-the-matrix span.cm-string { color: #39C; }
.cm-s-the-matrix span.cm-meta { color: #C9F; }
.cm-s-the-matrix span.cm-qualifier { color: #FFF700; }
.cm-s-the-matrix span.cm-builtin { color: #30a; }
.cm-s-the-matrix span.cm-bracket { color: #cc7; }
.cm-s-the-matrix span.cm-tag { color: #FFBD40; }
.cm-s-the-matrix span.cm-attribute { color: #FFF700; }
.cm-s-the-matrix span.cm-error { color: #FF0000; }

.cm-s-the-matrix .CodeMirror-activeline-background { background: #040; }

/*
Copyright (C) 2011 by MarkLogic Corporation
Author: Mike Brevoort <mike@brevoort.com>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
*/
.cm-s-xq-light span.cm-keyword { line-height: 1em; font-weight: bold; color: #5A5CAD; }
.cm-s-xq-light span.cm-atom { color: #6C8CD5; }
.cm-s-xq-light span.cm-number { color: #164; }
.cm-s-xq-light span.cm-def { text-decoration:underline; }
.cm-s-xq-light span.cm-variable { color: black; }
.cm-s-xq-light span.cm-variable-2 { color:black; }
.cm-s-xq-light span.cm-variable-3, .cm-s-xq-light span.cm-type { color: black; }
.cm-s-xq-light span.cm-property {}
.cm-s-xq-light span.cm-operator {}
.cm-s-xq-light span.cm-comment { color: #0080FF; font-style: italic; }
.cm-s-xq-light span.cm-string { color: red; }
.cm-s-xq-light span.cm-meta { color: yellow; }
.cm-s-xq-light span.cm-qualifier { color: grey; }
.cm-s-xq-light span.cm-builtin { color: #7EA656; }
.cm-s-xq-light span.cm-bracket { color: #cc7; }
.cm-s-xq-light span.cm-tag { color: #3F7F7F; }
.cm-s-xq-light span.cm-attribute { color: #7F007F; }
.cm-s-xq-light span.cm-error { color: #f00; }

.cm-s-xq-light .CodeMirror-activeline-background { background: #e8f2ff; }
.cm-s-xq-light .CodeMirror-matchingbracket { outline:1px solid grey;color:black !important;background:yellow; }

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.CodeMirror {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;
  /* Changed to auto to autogrow */
}

.CodeMirror pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

/* This causes https://github.com/jupyter/jupyterlab/issues/522 */
/* May not cause it not because we changed it! */
.CodeMirror-lines {
  padding: var(--jp-code-padding) 0;
}

.CodeMirror-linenumber {
  padding: 0 8px;
}

.jp-CodeMirrorEditor-static {
  margin: var(--jp-code-padding);
}

.jp-CodeMirrorEditor,
.jp-CodeMirrorEditor-static {
  cursor: text;
}

.jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
  border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .CodeMirror-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.CodeMirror.jp-mod-readOnly .CodeMirror-cursor {
  display: none;
}

.CodeMirror-gutters {
  border-right: 1px solid var(--jp-border-color2);
  background-color: var(--jp-layout-color0);
}

.jp-CollaboratorCursor {
  border-left: 5px solid transparent;
  border-right: 5px solid transparent;
  border-top: none;
  border-bottom: 3px solid;
  background-clip: content-box;
  margin-left: -5px;
  margin-right: -5px;
}

.CodeMirror-selectedtext.cm-searching {
  background-color: var(--jp-search-selected-match-background-color) !important;
  color: var(--jp-search-selected-match-color) !important;
}

.cm-searching {
  background-color: var(
    --jp-search-unselected-match-background-color
  ) !important;
  color: var(--jp-search-unselected-match-color) !important;
}

.CodeMirror-focused .CodeMirror-selected {
  background-color: var(--jp-editor-selected-focused-background);
}

.CodeMirror-selected {
  background-color: var(--jp-editor-selected-background);
}

.jp-CollaboratorCursor-hover {
  position: absolute;
  z-index: 1;
  transform: translateX(-50%);
  color: white;
  border-radius: 3px;
  padding-left: 4px;
  padding-right: 4px;
  padding-top: 1px;
  padding-bottom: 1px;
  text-align: center;
  font-size: var(--jp-ui-font-size1);
  white-space: nowrap;
}

.jp-CodeMirror-ruler {
  border-left: 1px dashed var(--jp-border-color2);
}

/**
 * Here is our jupyter theme for CodeMirror syntax highlighting
 * This is used in our marked.js syntax highlighting and CodeMirror itself
 * The string "jupyter" is set in ../codemirror/widget.DEFAULT_CODEMIRROR_THEME
 * This came from the classic notebook, which came form highlight.js/GitHub
 */

/**
 * CodeMirror themes are handling the background/color in this way. This works
 * fine for CodeMirror editors outside the notebook, but the notebook styles
 * these things differently.
 */
.CodeMirror.cm-s-jupyter {
  background: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

/* In the notebook, we want this styling to be handled by its container */
.jp-CodeConsole .CodeMirror.cm-s-jupyter,
.jp-Notebook .CodeMirror.cm-s-jupyter {
  background: transparent;
}

.cm-s-jupyter .CodeMirror-cursor {
  border-left: var(--jp-code-cursor-width0) solid var(--jp-editor-cursor-color);
}
.cm-s-jupyter span.cm-keyword {
  color: var(--jp-mirror-editor-keyword-color);
  font-weight: bold;
}
.cm-s-jupyter span.cm-atom {
  color: var(--jp-mirror-editor-atom-color);
}
.cm-s-jupyter span.cm-number {
  color: var(--jp-mirror-editor-number-color);
}
.cm-s-jupyter span.cm-def {
  color: var(--jp-mirror-editor-def-color);
}
.cm-s-jupyter span.cm-variable {
  color: var(--jp-mirror-editor-variable-color);
}
.cm-s-jupyter span.cm-variable-2 {
  color: var(--jp-mirror-editor-variable-2-color);
}
.cm-s-jupyter span.cm-variable-3 {
  color: var(--jp-mirror-editor-variable-3-color);
}
.cm-s-jupyter span.cm-punctuation {
  color: var(--jp-mirror-editor-punctuation-color);
}
.cm-s-jupyter span.cm-property {
  color: var(--jp-mirror-editor-property-color);
}
.cm-s-jupyter span.cm-operator {
  color: var(--jp-mirror-editor-operator-color);
  font-weight: bold;
}
.cm-s-jupyter span.cm-comment {
  color: var(--jp-mirror-editor-comment-color);
  font-style: italic;
}
.cm-s-jupyter span.cm-string {
  color: var(--jp-mirror-editor-string-color);
}
.cm-s-jupyter span.cm-string-2 {
  color: var(--jp-mirror-editor-string-2-color);
}
.cm-s-jupyter span.cm-meta {
  color: var(--jp-mirror-editor-meta-color);
}
.cm-s-jupyter span.cm-qualifier {
  color: var(--jp-mirror-editor-qualifier-color);
}
.cm-s-jupyter span.cm-builtin {
  color: var(--jp-mirror-editor-builtin-color);
}
.cm-s-jupyter span.cm-bracket {
  color: var(--jp-mirror-editor-bracket-color);
}
.cm-s-jupyter span.cm-tag {
  color: var(--jp-mirror-editor-tag-color);
}
.cm-s-jupyter span.cm-attribute {
  color: var(--jp-mirror-editor-attribute-color);
}
.cm-s-jupyter span.cm-header {
  color: var(--jp-mirror-editor-header-color);
}
.cm-s-jupyter span.cm-quote {
  color: var(--jp-mirror-editor-quote-color);
}
.cm-s-jupyter span.cm-link {
  color: var(--jp-mirror-editor-link-color);
}
.cm-s-jupyter span.cm-error {
  color: var(--jp-mirror-editor-error-color);
}
.cm-s-jupyter span.cm-hr {
  color: #999;
}

.cm-s-jupyter span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}

.cm-s-jupyter .CodeMirror-activeline-background,
.cm-s-jupyter .CodeMirror-gutter {
  background-color: var(--jp-layout-color2);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------*/

.jp-RenderedText {
  text-align: left;
  padding-left: var(--jp-code-padding);
  line-height: var(--jp-code-line-height);
  font-family: var(--jp-code-font-family);
}

.jp-RenderedText pre,
.jp-RenderedJavaScript pre,
.jp-RenderedHTMLCommon pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
  border: none;
  margin: 0px;
  padding: 0px;
  line-height: normal;
}

.jp-RenderedText pre a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}
.jp-RenderedText pre a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}
.jp-RenderedText pre a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* console foregrounds and backgrounds */
.jp-RenderedText pre .ansi-black-fg {
  color: #3e424d;
}
.jp-RenderedText pre .ansi-red-fg {
  color: #e75c58;
}
.jp-RenderedText pre .ansi-green-fg {
  color: #00a250;
}
.jp-RenderedText pre .ansi-yellow-fg {
  color: #ddb62b;
}
.jp-RenderedText pre .ansi-blue-fg {
  color: #208ffb;
}
.jp-RenderedText pre .ansi-magenta-fg {
  color: #d160c4;
}
.jp-RenderedText pre .ansi-cyan-fg {
  color: #60c6c8;
}
.jp-RenderedText pre .ansi-white-fg {
  color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-bg {
  background-color: #3e424d;
}
.jp-RenderedText pre .ansi-red-bg {
  background-color: #e75c58;
}
.jp-RenderedText pre .ansi-green-bg {
  background-color: #00a250;
}
.jp-RenderedText pre .ansi-yellow-bg {
  background-color: #ddb62b;
}
.jp-RenderedText pre .ansi-blue-bg {
  background-color: #208ffb;
}
.jp-RenderedText pre .ansi-magenta-bg {
  background-color: #d160c4;
}
.jp-RenderedText pre .ansi-cyan-bg {
  background-color: #60c6c8;
}
.jp-RenderedText pre .ansi-white-bg {
  background-color: #c5c1b4;
}

.jp-RenderedText pre .ansi-black-intense-fg {
  color: #282c36;
}
.jp-RenderedText pre .ansi-red-intense-fg {
  color: #b22b31;
}
.jp-RenderedText pre .ansi-green-intense-fg {
  color: #007427;
}
.jp-RenderedText pre .ansi-yellow-intense-fg {
  color: #b27d12;
}
.jp-RenderedText pre .ansi-blue-intense-fg {
  color: #0065ca;
}
.jp-RenderedText pre .ansi-magenta-intense-fg {
  color: #a03196;
}
.jp-RenderedText pre .ansi-cyan-intense-fg {
  color: #258f8f;
}
.jp-RenderedText pre .ansi-white-intense-fg {
  color: #a1a6b2;
}

.jp-RenderedText pre .ansi-black-intense-bg {
  background-color: #282c36;
}
.jp-RenderedText pre .ansi-red-intense-bg {
  background-color: #b22b31;
}
.jp-RenderedText pre .ansi-green-intense-bg {
  background-color: #007427;
}
.jp-RenderedText pre .ansi-yellow-intense-bg {
  background-color: #b27d12;
}
.jp-RenderedText pre .ansi-blue-intense-bg {
  background-color: #0065ca;
}
.jp-RenderedText pre .ansi-magenta-intense-bg {
  background-color: #a03196;
}
.jp-RenderedText pre .ansi-cyan-intense-bg {
  background-color: #258f8f;
}
.jp-RenderedText pre .ansi-white-intense-bg {
  background-color: #a1a6b2;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
  color: var(--jp-ui-inverse-font-color0);
}
.jp-RenderedText pre .ansi-default-inverse-bg {
  background-color: var(--jp-inverse-layout-color0);
}

.jp-RenderedText pre .ansi-bold {
  font-weight: bold;
}
.jp-RenderedText pre .ansi-underline {
  text-decoration: underline;
}

.jp-RenderedText[data-mime-type='application/vnd.jupyter.stderr'] {
  background: var(--jp-rendermime-error-background);
  padding-top: var(--jp-code-padding);
}

/*-----------------------------------------------------------------------------
| RenderedLatex
|----------------------------------------------------------------------------*/

.jp-RenderedLatex {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
}

/* Left-justify outputs.*/
.jp-OutputArea-output.jp-RenderedLatex {
  padding: var(--jp-code-padding);
  text-align: left;
}

/*-----------------------------------------------------------------------------
| RenderedHTML
|----------------------------------------------------------------------------*/

.jp-RenderedHTMLCommon {
  color: var(--jp-content-font-color1);
  font-family: var(--jp-content-font-family);
  font-size: var(--jp-content-font-size1);
  line-height: var(--jp-content-line-height);
  /* Give a bit more R padding on Markdown text to keep line lengths reasonable */
  padding-right: 20px;
}

.jp-RenderedHTMLCommon em {
  font-style: italic;
}

.jp-RenderedHTMLCommon strong {
  font-weight: bold;
}

.jp-RenderedHTMLCommon u {
  text-decoration: underline;
}

.jp-RenderedHTMLCommon a:link {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:hover {
  text-decoration: underline;
  color: var(--jp-content-link-color);
}

.jp-RenderedHTMLCommon a:visited {
  text-decoration: none;
  color: var(--jp-content-link-color);
}

/* Headings */

.jp-RenderedHTMLCommon h1,
.jp-RenderedHTMLCommon h2,
.jp-RenderedHTMLCommon h3,
.jp-RenderedHTMLCommon h4,
.jp-RenderedHTMLCommon h5,
.jp-RenderedHTMLCommon h6 {
  line-height: var(--jp-content-heading-line-height);
  font-weight: var(--jp-content-heading-font-weight);
  font-style: normal;
  margin: var(--jp-content-heading-margin-top) 0
    var(--jp-content-heading-margin-bottom) 0;
}

.jp-RenderedHTMLCommon h1:first-child,
.jp-RenderedHTMLCommon h2:first-child,
.jp-RenderedHTMLCommon h3:first-child,
.jp-RenderedHTMLCommon h4:first-child,
.jp-RenderedHTMLCommon h5:first-child,
.jp-RenderedHTMLCommon h6:first-child {
  margin-top: calc(0.5 * var(--jp-content-heading-margin-top));
}

.jp-RenderedHTMLCommon h1:last-child,
.jp-RenderedHTMLCommon h2:last-child,
.jp-RenderedHTMLCommon h3:last-child,
.jp-RenderedHTMLCommon h4:last-child,
.jp-RenderedHTMLCommon h5:last-child,
.jp-RenderedHTMLCommon h6:last-child {
  margin-bottom: calc(0.5 * var(--jp-content-heading-margin-bottom));
}

.jp-RenderedHTMLCommon h1 {
  font-size: var(--jp-content-font-size5);
}

.jp-RenderedHTMLCommon h2 {
  font-size: var(--jp-content-font-size4);
}

.jp-RenderedHTMLCommon h3 {
  font-size: var(--jp-content-font-size3);
}

.jp-RenderedHTMLCommon h4 {
  font-size: var(--jp-content-font-size2);
}

.jp-RenderedHTMLCommon h5 {
  font-size: var(--jp-content-font-size1);
}

.jp-RenderedHTMLCommon h6 {
  font-size: var(--jp-content-font-size0);
}

/* Lists */

.jp-RenderedHTMLCommon ul:not(.list-inline),
.jp-RenderedHTMLCommon ol:not(.list-inline) {
  padding-left: 2em;
}

.jp-RenderedHTMLCommon ul {
  list-style: disc;
}

.jp-RenderedHTMLCommon ul ul {
  list-style: square;
}

.jp-RenderedHTMLCommon ul ul ul {
  list-style: circle;
}

.jp-RenderedHTMLCommon ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol ol {
  list-style: upper-alpha;
}

.jp-RenderedHTMLCommon ol ol ol {
  list-style: lower-alpha;
}

.jp-RenderedHTMLCommon ol ol ol ol {
  list-style: lower-roman;
}

.jp-RenderedHTMLCommon ol ol ol ol ol {
  list-style: decimal;
}

.jp-RenderedHTMLCommon ol,
.jp-RenderedHTMLCommon ul {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon ul ul,
.jp-RenderedHTMLCommon ul ol,
.jp-RenderedHTMLCommon ol ul,
.jp-RenderedHTMLCommon ol ol {
  margin-bottom: 0em;
}

.jp-RenderedHTMLCommon hr {
  color: var(--jp-border-color2);
  background-color: var(--jp-border-color1);
  margin-top: 1em;
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon > pre {
  margin: 1.5em 2em;
}

.jp-RenderedHTMLCommon pre,
.jp-RenderedHTMLCommon code {
  border: 0;
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  line-height: var(--jp-code-line-height);
  padding: 0;
  white-space: pre-wrap;
}

.jp-RenderedHTMLCommon :not(pre) > code {
  background-color: var(--jp-layout-color2);
  padding: 1px 5px;
}

/* Tables */

.jp-RenderedHTMLCommon table {
  border-collapse: collapse;
  border-spacing: 0;
  border: none;
  color: var(--jp-ui-font-color1);
  font-size: 12px;
  table-layout: fixed;
  margin-left: auto;
  margin-right: auto;
}

.jp-RenderedHTMLCommon thead {
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  vertical-align: bottom;
}

.jp-RenderedHTMLCommon td,
.jp-RenderedHTMLCommon th,
.jp-RenderedHTMLCommon tr {
  vertical-align: middle;
  padding: 0.5em 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}

.jp-RenderedMarkdown.jp-RenderedHTMLCommon td,
.jp-RenderedMarkdown.jp-RenderedHTMLCommon th {
  max-width: none;
}

:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon td,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon th,
:not(.jp-RenderedMarkdown).jp-RenderedHTMLCommon tr {
  text-align: right;
}

.jp-RenderedHTMLCommon th {
  font-weight: bold;
}

.jp-RenderedHTMLCommon tbody tr:nth-child(odd) {
  background: var(--jp-layout-color0);
}

.jp-RenderedHTMLCommon tbody tr:nth-child(even) {
  background: var(--jp-rendermime-table-row-background);
}

.jp-RenderedHTMLCommon tbody tr:hover {
  background: var(--jp-rendermime-table-row-hover-background);
}

.jp-RenderedHTMLCommon table {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0px;
}

.jp-RenderedHTMLCommon p {
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon img {
  -moz-force-broken-image-icon: 1;
}

/* Restrict to direct children as other images could be nested in other content. */
.jp-RenderedHTMLCommon > img {
  display: block;
  margin-left: 0;
  margin-right: 0;
  margin-bottom: 1em;
}

/* Change color behind transparent images if they need it... */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-light-background {
  background-color: var(--jp-inverse-layout-color1);
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-dark-background {
  background-color: var(--jp-inverse-layout-color1);
}
/* ...or leave it untouched if they don't */
[data-jp-theme-light='false'] .jp-RenderedImage img.jp-needs-dark-background {
}
[data-jp-theme-light='true'] .jp-RenderedImage img.jp-needs-light-background {
}

.jp-RenderedHTMLCommon img,
.jp-RenderedImage img,
.jp-RenderedHTMLCommon svg,
.jp-RenderedSVG svg {
  max-width: 100%;
  height: auto;
}

.jp-RenderedHTMLCommon img.jp-mod-unconfined,
.jp-RenderedImage img.jp-mod-unconfined,
.jp-RenderedHTMLCommon svg.jp-mod-unconfined,
.jp-RenderedSVG svg.jp-mod-unconfined {
  max-width: none;
}

.jp-RenderedHTMLCommon .alert {
  padding: var(--jp-notebook-padding);
  border: var(--jp-border-width) solid transparent;
  border-radius: var(--jp-border-radius);
  margin-bottom: 1em;
}

.jp-RenderedHTMLCommon .alert-info {
  color: var(--jp-info-color0);
  background-color: var(--jp-info-color3);
  border-color: var(--jp-info-color2);
}
.jp-RenderedHTMLCommon .alert-info hr {
  border-color: var(--jp-info-color3);
}
.jp-RenderedHTMLCommon .alert-info > p:last-child,
.jp-RenderedHTMLCommon .alert-info > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-warning {
  color: var(--jp-warn-color0);
  background-color: var(--jp-warn-color3);
  border-color: var(--jp-warn-color2);
}
.jp-RenderedHTMLCommon .alert-warning hr {
  border-color: var(--jp-warn-color3);
}
.jp-RenderedHTMLCommon .alert-warning > p:last-child,
.jp-RenderedHTMLCommon .alert-warning > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-success {
  color: var(--jp-success-color0);
  background-color: var(--jp-success-color3);
  border-color: var(--jp-success-color2);
}
.jp-RenderedHTMLCommon .alert-success hr {
  border-color: var(--jp-success-color3);
}
.jp-RenderedHTMLCommon .alert-success > p:last-child,
.jp-RenderedHTMLCommon .alert-success > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon .alert-danger {
  color: var(--jp-error-color0);
  background-color: var(--jp-error-color3);
  border-color: var(--jp-error-color2);
}
.jp-RenderedHTMLCommon .alert-danger hr {
  border-color: var(--jp-error-color3);
}
.jp-RenderedHTMLCommon .alert-danger > p:last-child,
.jp-RenderedHTMLCommon .alert-danger > ul:last-child {
  margin-bottom: 0;
}

.jp-RenderedHTMLCommon blockquote {
  margin: 1em 2em;
  padding: 0 1em;
  border-left: 5px solid var(--jp-border-color2);
}

a.jp-InternalAnchorLink {
  visibility: hidden;
  margin-left: 8px;
  color: var(--md-blue-800);
}

h1:hover .jp-InternalAnchorLink,
h2:hover .jp-InternalAnchorLink,
h3:hover .jp-InternalAnchorLink,
h4:hover .jp-InternalAnchorLink,
h5:hover .jp-InternalAnchorLink,
h6:hover .jp-InternalAnchorLink {
  visibility: visible;
}

.jp-RenderedHTMLCommon kbd {
  background-color: var(--jp-rendermime-table-row-background);
  border: 1px solid var(--jp-border-color0);
  border-bottom-color: var(--jp-border-color2);
  border-radius: 3px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
  display: inline-block;
  font-size: 0.8em;
  line-height: 1em;
  padding: 0.2em 0.5em;
}

/* Most direct children of .jp-RenderedHTMLCommon have a margin-bottom of 1.0.
 * At the bottom of cells this is a bit too much as there is also spacing
 * between cells. Going all the way to 0 gets too tight between markdown and
 * code cells.
 */
.jp-RenderedHTMLCommon > *:last-child {
  margin-bottom: 0.5em;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MimeDocument {
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-filebrowser-button-height: 28px;
  --jp-private-filebrowser-button-width: 48px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FileBrowser {
  display: flex;
  flex-direction: column;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  border-bottom: none;
  height: auto;
  margin: var(--jp-toolbar-header-margin);
  box-shadow: none;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 4px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0px 2px;
  padding: 0px 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0px;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar.jp-Toolbar {
  padding: 0px;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  justify-content: space-evenly;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-Toolbar-item {
  flex: 1;
}

.jp-FileBrowser-toolbar.jp-Toolbar .jp-ToolbarButtonComponent {
  width: 100%;
}

/*-----------------------------------------------------------------------------
| DirListing
|----------------------------------------------------------------------------*/

.jp-DirListing {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
  outline: 0;
}

.jp-DirListing-header {
  flex: 0 0 auto;
  display: flex;
  flex-direction: row;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px 12px;
  font-weight: 500;
}

.jp-DirListing-headerItem:hover {
  background: var(--jp-layout-color2);
}

.jp-DirListing-headerItem.jp-id-name {
  flex: 1 0 84px;
}

.jp-DirListing-headerItem.jp-id-modified {
  flex: 0 0 112px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-DirListing-narrow .jp-id-modified,
.jp-DirListing-narrow .jp-DirListing-itemModified {
  display: none;
}

.jp-DirListing-headerItem.jp-mod-selected {
  font-weight: 600;
}

/* increase specificity to override bundled default */
.jp-DirListing-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

/* Style the directory listing content when a user drops a file to upload */
.jp-DirListing.jp-mod-native-drop .jp-DirListing-content {
  outline: 5px dashed rgba(128, 128, 128, 0.5);
  outline-offset: -10px;
  cursor: copy;
}

.jp-DirListing-item {
  display: flex;
  flex-direction: row;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-item.jp-mod-selected {
  color: white;
  background: var(--jp-brand-color1);
}

.jp-DirListing-item.jp-mod-dropTarget {
  background: var(--jp-brand-color3);
}

.jp-DirListing-item:hover:not(.jp-mod-selected) {
  background: var(--jp-layout-color2);
}

.jp-DirListing-itemIcon {
  flex: 0 0 20px;
  margin-right: 4px;
}

.jp-DirListing-itemText {
  flex: 1 0 64px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  user-select: none;
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon:before {
  color: limegreen;
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
  font-size: var(--jp-ui-font-size1);
  padding-left: 4px;
  margin-left: 4px;
  width: 160px;
  background-color: var(--jp-ui-inverse-font-color2);
  box-shadow: var(--jp-elevation-z2);
  border-radius: 0px;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-DirListing-deadSpace {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  list-style-type: none;
  overflow: auto;
  background-color: var(--jp-layout-color1);
}

.jp-Document {
  min-width: 120px;
  min-height: 120px;
  outline: none;
}

.jp-FileDialog.jp-mod-conflict input {
  color: red;
}

.jp-FileDialog .jp-new-name-title {
  margin-top: 12px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
}

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: flex;
  flex-direction: row;
}

.jp-OutputPrompt {
  flex: 0 0 var(--jp-cell-prompt-width);
  color: var(--jp-cell-outprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);
  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-OutputArea-output {
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea-child .jp-OutputArea-output {
  flex-grow: 1;
  flex-shrink: 1;
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `p-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated:before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: transparent;
}

/* pre */

.jp-OutputArea-output pre {
  border: none;
  margin: 0px;
  padding: 0px;
  overflow-x: auto;
  overflow-y: auto;
  word-break: break-all;
  word-wrap: break-word;
  white-space: pre-wrap;
}

/* tables */

.jp-OutputArea-output.jp-RenderedHTMLCommon table {
  margin-left: 0;
  margin-right: 0;
}

/* description lists */

.jp-OutputArea-output dl,
.jp-OutputArea-output dt,
.jp-OutputArea-output dd {
  display: block;
}

.jp-OutputArea-output dl {
  width: 100%;
  overflow: hidden;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dt {
  font-weight: bold;
  float: left;
  width: 20%;
  padding: 0;
  margin: 0;
}

.jp-OutputArea-output dd {
  float: left;
  width: 80%;
  padding: 0;
  margin: 0;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0px;
  flex: 1 1 auto;
}

.jp-OutputArea-executeResult.jp-RenderedText {
  padding-top: var(--jp-code-padding);
}

/*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------*/

.jp-OutputArea-stdin {
  line-height: var(--jp-code-line-height);
  padding-top: var(--jp-code-padding);
  display: flex;
}

.jp-Stdin-prompt {
  color: var(--jp-content-font-color0);
  padding-right: var(--jp-code-padding);
  vertical-align: baseline;
  flex: 0 0 auto;
}

.jp-Stdin-input {
  font-family: var(--jp-code-font-family);
  font-size: inherit;
  color: inherit;
  background-color: inherit;
  width: 42%;
  min-width: 200px;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

/*-----------------------------------------------------------------------------
| Output Area View
|----------------------------------------------------------------------------*/

.jp-LinkedOutputView .jp-OutputArea {
  height: 100%;
  display: block;
}

.jp-LinkedOutputView .jp-OutputArea-output:only-child {
  height: 100%;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0px;
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
  border-radius: var(--jp-border-radius);
  opacity: 1;
}

.jp-Collapser-child {
  display: block;
  width: 100%;
  box-sizing: border-box;
  /* height: 100% doesn't work because the height of its parent is computed from content */
  position: absolute;
  top: 0px;
  bottom: 0px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Header/Footer
|----------------------------------------------------------------------------*/

/* Hidden by zero height by default */
.jp-CellHeader,
.jp-CellFooter {
  height: 0px;
  width: 100%;
  padding: 0px;
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Input
|----------------------------------------------------------------------------*/

/* All input areas */
.jp-InputArea {
  display: flex;
  flex-direction: row;
}

.jp-InputArea-editor {
  flex: 1 1 auto;
}

.jp-InputArea-editor {
  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0px;
  background: var(--jp-cell-editor-background);
}

.jp-InputPrompt {
  flex: 0 0 var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
  opacity: var(--jp-cell-prompt-opacity);
  /* Right align prompt text, don't wrap to handle large prompt numbers */
  text-align: right;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  /* Disable text selection */
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: flex;
  flex-direction: row;
  flex: 1 1 auto;
}

.jp-Placeholder-prompt {
  box-sizing: border-box;
}

.jp-Placeholder-content {
  flex: 1 1 auto;
  border: none;
  background: transparent;
  height: 20px;
  box-sizing: border-box;
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-cell-scrolling-output-offset: 5px;
}

/*-----------------------------------------------------------------------------
| Cell
|----------------------------------------------------------------------------*/

.jp-Cell {
  padding: var(--jp-cell-padding);
  margin: 0px;
  border: none;
  outline: none;
  background: transparent;
}

/*-----------------------------------------------------------------------------
| Common input/output
|----------------------------------------------------------------------------*/

.jp-Cell-inputWrapper,
.jp-Cell-outputWrapper {
  display: flex;
  flex-direction: row;
  padding: 0px;
  margin: 0px;
  /* Added to reveal the box-shadow on the input and output collapsers. */
  overflow: visible;
}

/* Only input/output areas inside cells */
.jp-Cell-inputArea,
.jp-Cell-outputArea {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Collapser
|----------------------------------------------------------------------------*/

/* Make the output collapser disappear when there is not output, but do so
 * in a manner that leaves it in the layout and preserves its width.
 */
.jp-Cell.jp-mod-noOutputs .jp-Cell-outputCollapser {
  border: none !important;
  background: transparent !important;
}

.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputCollapser {
  min-height: var(--jp-cell-collapser-min-height);
}

/*-----------------------------------------------------------------------------
| Output
|----------------------------------------------------------------------------*/

/* Put a space between input and output when there IS output */
.jp-Cell:not(.jp-mod-noOutputs) .jp-Cell-outputWrapper {
  margin-top: 5px;
}

/* Text output with the Out[] prompt needs a top padding to match the
 * alignment of the Out[] prompt itself.
 */
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
  padding-top: var(--jp-code-padding);
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
  overflow-y: auto;
  max-height: 200px;
  box-shadow: inset 0 0 6px 2px rgba(0, 0, 0, 0.3);
  margin-left: var(--jp-private-cell-scrolling-output-offset);
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  flex: 0 0
    calc(
      var(--jp-cell-prompt-width) -
        var(--jp-private-cell-scrolling-output-offset)
    );
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  flex: 1 1 auto;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Variables
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: 2px;
}

.jp-Toolbar-item.jp-Notebook-toolbarCellType .jp-select-wrapper.jp-mod-focused {
  border: none;
  box-shadow: none;
}

.jp-Notebook-toolbarCellTypeDropdown select {
  height: 24px;
  font-size: var(--jp-ui-font-size1);
  line-height: 14px;
  border-radius: 0;
  display: block;
}

.jp-Notebook-toolbarCellTypeDropdown span {
  top: 5px !important;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Private CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

.jp-NotebookPanel {
  display: block;
  height: 100%;
}

.jp-NotebookPanel.jp-Document {
  min-width: 240px;
  min-height: 120px;
}

.jp-Notebook {
  padding: var(--jp-notebook-padding);
  outline: none;
  overflow: auto;
  background: var(--jp-layout-color0);
}

.jp-Notebook.jp-mod-scrollPastEnd::after {
  display: block;
  content: '';
  min-height: var(--jp-notebook-scroll-padding);
}

.jp-Notebook .jp-Cell {
  overflow: visible;
}

.jp-Notebook .jp-Cell .jp-InputPrompt {
  cursor: move;
}

/*-----------------------------------------------------------------------------
| Notebook state related styling
|
| The notebook and cells each have states, here are the possibilities:
|
| - Notebook
|   - Command
|   - Edit
| - Cell
|   - None
|   - Active (only one can be active)
|   - Selected (the cells actions are applied to)
|   - Multiselected (when multiple selected, the cursor)
|   - No outputs
|----------------------------------------------------------------------------*/

/* Command or edit modes */

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-InputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

.jp-Notebook .jp-Cell:not(.jp-mod-active) .jp-OutputPrompt {
  opacity: var(--jp-cell-prompt-not-active-opacity);
  color: var(--jp-cell-prompt-not-active-font-color);
}

/* cell is active */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser {
  background: var(--jp-brand-color1);
}

/* collapser is hovered */
.jp-Notebook .jp-Cell .jp-Collapser:hover {
  box-shadow: var(--jp-elevation-z2);
  background: var(--jp-brand-color1);
  opacity: var(--jp-cell-collapser-not-active-hover-opacity);
}

/* cell is active and collapser is hovered */
.jp-Notebook .jp-Cell.jp-mod-active .jp-Collapser:hover {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/* Command mode */

.jp-Notebook.jp-mod-commandMode .jp-Cell.jp-mod-selected {
  background: var(--jp-notebook-multiselected-color);
}

.jp-Notebook.jp-mod-commandMode
  .jp-Cell.jp-mod-active.jp-mod-selected:not(.jp-mod-multiSelected) {
  background: transparent;
}

/* Edit mode */

.jp-Notebook.jp-mod-editMode .jp-Cell.jp-mod-active .jp-InputArea-editor {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-cell-editor-active-background);
}

/*-----------------------------------------------------------------------------
| Notebook drag and drop
|----------------------------------------------------------------------------*/

.jp-Notebook-cell.jp-mod-dropSource {
  opacity: 0.5;
}

.jp-Notebook-cell.jp-mod-dropTarget,
.jp-Notebook.jp-mod-commandMode
  .jp-Notebook-cell.jp-mod-active.jp-mod-selected.jp-mod-dropTarget {
  border-top-color: var(--jp-private-notebook-selected-color);
  border-top-style: solid;
  border-top-width: 2px;
}

.jp-dragImage {
  display: flex;
  flex-direction: row;
  width: var(--jp-private-notebook-dragImage-width);
  height: var(--jp-private-notebook-dragImage-height);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
  overflow: visible;
}

.jp-dragImage-singlePrompt {
  box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
}

.jp-dragImage .jp-dragImage-content {
  flex: 1 1 auto;
  z-index: 2;
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  line-height: var(--jp-code-line-height);
  padding: var(--jp-code-padding);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background-color);
  color: var(--jp-content-font-color3);
  text-align: left;
  margin: 4px 4px 4px 0px;
}

.jp-dragImage .jp-dragImage-prompt {
  flex: 0 0 auto;
  min-width: 36px;
  color: var(--jp-cell-inprompt-font-color);
  padding: var(--jp-code-padding);
  padding-left: 12px;
  font-family: var(--jp-cell-prompt-font-family);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  line-height: 1.9;
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;
}

.jp-dragImage-multipleBack {
  z-index: -1;
  position: absolute;
  height: 32px;
  width: 300px;
  top: 8px;
  left: 8px;
  background: var(--jp-layout-color2);
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  box-shadow: 2px 2px 4px 0px rgba(0, 0, 0, 0.12);
}

/*-----------------------------------------------------------------------------
| Cell toolbar
|----------------------------------------------------------------------------*/

.jp-NotebookTools {
  display: block;
  min-width: var(--jp-sidebar-min-width);
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  /* This is needed so that all font sizing of children done in ems is
    * relative to this base size */
  font-size: var(--jp-ui-font-size1);
  overflow: auto;
}

.jp-NotebookTools-tool {
  padding: 0px 12px 0 12px;
}

.jp-ActiveCellTool {
  padding: 12px;
  background-color: var(--jp-layout-color1);
  border-top: none !important;
}

.jp-ActiveCellTool .jp-InputArea-prompt {
  flex: 0 0 auto;
  padding-left: 0px;
}

.jp-ActiveCellTool .jp-InputArea-editor {
  flex: 1 1 auto;
  background: var(--jp-cell-editor-background);
  border-color: var(--jp-cell-editor-border-color);
}

.jp-ActiveCellTool .jp-InputArea-editor .CodeMirror {
  background: transparent;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0px 12px 0px;
}

.jp-RankedPanel > :not(:first-child) {
  margin-top: 12px;
}

.jp-KeySelector select.jp-mod-styled {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color0);
  border: var(--jp-border-width) solid var(--jp-border-color1);
}

.jp-KeySelector label,
.jp-MetadataEditorTool label {
  line-height: 1.4;
}

/*-----------------------------------------------------------------------------
| Presentation Mode (.jp-mod-presentationMode)
|----------------------------------------------------------------------------*/

.jp-mod-presentationMode .jp-Notebook {
  --jp-content-font-size1: var(--jp-content-presentation-font-size1);
  --jp-code-font-size: var(--jp-code-presentation-font-size);
}

.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-InputPrompt,
.jp-mod-presentationMode .jp-Notebook .jp-Cell .jp-OutputPrompt {
  flex: 0 0 110px;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* This file was auto-generated by ensurePackage() in @jupyterlab/buildutils */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

</style>

    <style type="text/css">
/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*
The following CSS variables define the main, public API for styling JupyterLab.
These variables should be used by all plugins wherever possible. In other
words, plugins should not define custom colors, sizes, etc unless absolutely
necessary. This enables users to change the visual theme of JupyterLab
by changing these variables.

Many variables appear in an ordered sequence (0,1,2,3). These sequences
are designed to work well together, so for example, `--jp-border-color1` should
be used with `--jp-layout-color1`. The numbers have the following meanings:

* 0: super-primary, reserved for special emphasis
* 1: primary, most important under normal situations
* 2: secondary, next most important under normal situations
* 3: tertiary, next most important under normal situations

Throughout JupyterLab, we are mostly following principles from Google's
Material Design when selecting colors. We are not, however, following
all of MD as it is not optimized for dense, information rich UIs.
*/

:root {
  /* Elevation
   *
   * We style box-shadows using Material Design's idea of elevation. These particular numbers are taken from here:
   *
   * https://github.com/material-components/material-components-web
   * https://material-components-web.appspot.com/elevation.html
   */

  --jp-shadow-base-lightness: 0;
  --jp-shadow-umbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.2
  );
  --jp-shadow-penumbra-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.14
  );
  --jp-shadow-ambient-color: rgba(
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    var(--jp-shadow-base-lightness),
    0.12
  );
  --jp-elevation-z0: none;
  --jp-elevation-z1: 0px 2px 1px -1px var(--jp-shadow-umbra-color),
    0px 1px 1px 0px var(--jp-shadow-penumbra-color),
    0px 1px 3px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0px 3px 1px -2px var(--jp-shadow-umbra-color),
    0px 2px 2px 0px var(--jp-shadow-penumbra-color),
    0px 1px 5px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0px 2px 4px -1px var(--jp-shadow-umbra-color),
    0px 4px 5px 0px var(--jp-shadow-penumbra-color),
    0px 1px 10px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0px 3px 5px -1px var(--jp-shadow-umbra-color),
    0px 6px 10px 0px var(--jp-shadow-penumbra-color),
    0px 1px 18px 0px var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0px 5px 5px -3px var(--jp-shadow-umbra-color),
    0px 8px 10px 1px var(--jp-shadow-penumbra-color),
    0px 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0px 7px 8px -4px var(--jp-shadow-umbra-color),
    0px 12px 17px 2px var(--jp-shadow-penumbra-color),
    0px 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0px 8px 10px -5px var(--jp-shadow-umbra-color),
    0px 16px 24px 2px var(--jp-shadow-penumbra-color),
    0px 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0px 10px 13px -6px var(--jp-shadow-umbra-color),
    0px 20px 31px 3px var(--jp-shadow-penumbra-color),
    0px 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0px 11px 15px -7px var(--jp-shadow-umbra-color),
    0px 24px 38px 3px var(--jp-shadow-penumbra-color),
    0px 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-border-radius: 2px;

  /* UI Fonts
   *
   * The UI font CSS variables are used for the typography all of the JupyterLab
   * user interface elements that are not directly user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-ui-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-ui-font-scale-factor: 1.2;
  --jp-ui-font-size0: 0.83333em;
  --jp-ui-font-size1: 13px; /* Base font size */
  --jp-ui-font-size2: 1.2em;
  --jp-ui-font-size3: 1.44em;

  --jp-ui-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica,
    Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Use these font colors against the corresponding main layout colors.
   * In a light theme, these go from dark to light.
   */

  /* Defaults use Material Design specification */
  --jp-ui-font-color0: rgba(0, 0, 0, 1);
  --jp-ui-font-color1: rgba(0, 0, 0, 0.87);
  --jp-ui-font-color2: rgba(0, 0, 0, 0.54);
  --jp-ui-font-color3: rgba(0, 0, 0, 0.38);

  /*
   * Use these against the brand/accent/warn/error colors.
   * These will typically go from light to darker, in both a dark and light theme.
   */

  --jp-ui-inverse-font-color0: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color1: rgba(255, 255, 255, 1);
  --jp-ui-inverse-font-color2: rgba(255, 255, 255, 0.7);
  --jp-ui-inverse-font-color3: rgba(255, 255, 255, 0.5);

  /* Content Fonts
   *
   * Content font variables are used for typography of user generated content.
   *
   * The font sizing here is done assuming that the body font size of --jp-content-font-size1
   * is applied to a parent element. When children elements, such as headings, are sized
   * in em all things will be computed relative to that body size.
   */

  --jp-content-line-height: 1.6;
  --jp-content-font-scale-factor: 1.2;
  --jp-content-font-size0: 0.83333em;
  --jp-content-font-size1: 14px; /* Base font size */
  --jp-content-font-size2: 1.2em;
  --jp-content-font-size3: 1.44em;
  --jp-content-font-size4: 1.728em;
  --jp-content-font-size5: 2.0736em;

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-content-presentation-font-size1: 17px;

  --jp-content-heading-line-height: 1;
  --jp-content-heading-margin-top: 1.2em;
  --jp-content-heading-margin-bottom: 0.8em;
  --jp-content-heading-font-weight: 500;

  /* Defaults use Material Design specification */
  --jp-content-font-color0: rgba(0, 0, 0, 1);
  --jp-content-font-color1: rgba(0, 0, 0, 0.87);
  --jp-content-font-color2: rgba(0, 0, 0, 0.54);
  --jp-content-font-color3: rgba(0, 0, 0, 0.38);

  --jp-content-link-color: var(--md-blue-700);

  --jp-content-font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: Menlo, Consolas, 'DejaVu Sans Mono', monospace;
  --jp-code-font-family: var(--jp-code-font-family-default);

  /* This gives a magnification of about 125% in presentation mode over normal. */
  --jp-code-presentation-font-size: 16px;

  /* may need to tweak cursor width if you change font size */
  --jp-code-cursor-width0: 1.4px;
  --jp-code-cursor-width1: 2px;
  --jp-code-cursor-width2: 4px;

  /* Layout
   *
   * The following are the main layout colors use in JupyterLab. In a light
   * theme these would go from light to dark.
   */

  --jp-layout-color0: white;
  --jp-layout-color1: white;
  --jp-layout-color2: var(--md-grey-200);
  --jp-layout-color3: var(--md-grey-400);
  --jp-layout-color4: var(--md-grey-600);

  /* Inverse Layout
   *
   * The following are the inverse layout colors use in JupyterLab. In a light
   * theme these would go from dark to light.
   */

  --jp-inverse-layout-color0: #111111;
  --jp-inverse-layout-color1: var(--md-grey-900);
  --jp-inverse-layout-color2: var(--md-grey-800);
  --jp-inverse-layout-color3: var(--md-grey-700);
  --jp-inverse-layout-color4: var(--md-grey-600);

  /* Brand/accent */

  --jp-brand-color0: var(--md-blue-700);
  --jp-brand-color1: var(--md-blue-500);
  --jp-brand-color2: var(--md-blue-300);
  --jp-brand-color3: var(--md-blue-100);
  --jp-brand-color4: var(--md-blue-50);

  --jp-accent-color0: var(--md-green-700);
  --jp-accent-color1: var(--md-green-500);
  --jp-accent-color2: var(--md-green-300);
  --jp-accent-color3: var(--md-green-100);

  /* State colors (warn, error, success, info) */

  --jp-warn-color0: var(--md-orange-700);
  --jp-warn-color1: var(--md-orange-500);
  --jp-warn-color2: var(--md-orange-300);
  --jp-warn-color3: var(--md-orange-100);

  --jp-error-color0: var(--md-red-700);
  --jp-error-color1: var(--md-red-500);
  --jp-error-color2: var(--md-red-300);
  --jp-error-color3: var(--md-red-100);

  --jp-success-color0: var(--md-green-700);
  --jp-success-color1: var(--md-green-500);
  --jp-success-color2: var(--md-green-300);
  --jp-success-color3: var(--md-green-100);

  --jp-info-color0: var(--md-cyan-700);
  --jp-info-color1: var(--md-cyan-500);
  --jp-info-color2: var(--md-cyan-300);
  --jp-info-color3: var(--md-cyan-100);

  /* Cell specific styles */

  --jp-cell-padding: 5px;

  --jp-cell-collapser-width: 8px;
  --jp-cell-collapser-min-height: 20px;
  --jp-cell-collapser-not-active-hover-opacity: 0.6;

  --jp-cell-editor-background: var(--md-grey-100);
  --jp-cell-editor-border-color: var(--md-grey-300);
  --jp-cell-editor-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-cell-editor-active-background: var(--jp-layout-color0);
  --jp-cell-editor-active-border-color: var(--jp-brand-color1);

  --jp-cell-prompt-width: 64px;
  --jp-cell-prompt-font-family: 'Source Code Pro', monospace;
  --jp-cell-prompt-letter-spacing: 0px;
  --jp-cell-prompt-opacity: 1;
  --jp-cell-prompt-not-active-opacity: 0.5;
  --jp-cell-prompt-not-active-font-color: var(--md-grey-700);
  /* A custom blend of MD grey and blue 600
   * See https://meyerweb.com/eric/tools/color-blend/#546E7A:1E88E5:5:hex */
  --jp-cell-inprompt-font-color: #307fc1;
  /* A custom blend of MD grey and orange 600
   * https://meyerweb.com/eric/tools/color-blend/#546E7A:F4511E:5:hex */
  --jp-cell-outprompt-font-color: #bf5b3d;

  /* Notebook specific styles */

  --jp-notebook-padding: 10px;
  --jp-notebook-select-background: var(--jp-layout-color1);
  --jp-notebook-multiselected-color: var(--md-blue-50);

  /* The scroll padding is calculated to fill enough space at the bottom of the
  notebook to show one single-line cell (with appropriate padding) at the top
  when the notebook is scrolled all the way to the bottom. We also subtract one
  pixel so that no scrollbar appears if we have just one single-line cell in the
  notebook. This padding is to enable a 'scroll past end' feature in a notebook.
  */
  --jp-notebook-scroll-padding: calc(
    100% - var(--jp-code-font-size) * var(--jp-code-line-height) -
      var(--jp-code-padding) - var(--jp-cell-padding) - 1px
  );

  /* Rendermime styles */

  --jp-rendermime-error-background: #fdd;
  --jp-rendermime-table-row-background: var(--md-grey-100);
  --jp-rendermime-table-row-hover-background: var(--md-light-blue-50);

  /* Dialog specific styles */

  --jp-dialog-background: rgba(0, 0, 0, 0.25);

  /* Console specific styles */

  --jp-console-padding: 10px;

  /* Toolbar specific styles */

  --jp-toolbar-border-color: var(--jp-border-color1);
  --jp-toolbar-micro-height: 8px;
  --jp-toolbar-background: var(--jp-layout-color1);
  --jp-toolbar-box-shadow: 0px 0px 2px 0px rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0px 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-border-color1);
  --jp-input-active-border-color: var(--jp-brand-color1);
  --jp-input-active-box-shadow-color: rgba(19, 124, 189, 0.3);

  /* General editor styles */

  --jp-editor-selected-background: #d9d9d9;
  --jp-editor-selected-focused-background: #d7d4f0;
  --jp-editor-cursor-color: var(--jp-ui-font-color0);

  /* Code mirror specific styles */

  --jp-mirror-editor-keyword-color: #008000;
  --jp-mirror-editor-atom-color: #88f;
  --jp-mirror-editor-number-color: #080;
  --jp-mirror-editor-def-color: #00f;
  --jp-mirror-editor-variable-color: var(--md-grey-900);
  --jp-mirror-editor-variable-2-color: #05a;
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #aa22ff;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #aa22ff;
  --jp-mirror-editor-qualifier-color: #555;
  --jp-mirror-editor-builtin-color: #008000;
  --jp-mirror-editor-bracket-color: #997;
  --jp-mirror-editor-tag-color: #170;
  --jp-mirror-editor-attribute-color: #00c;
  --jp-mirror-editor-header-color: blue;
  --jp-mirror-editor-quote-color: #090;
  --jp-mirror-editor-link-color: #00c;
  --jp-mirror-editor-error-color: #f00;
  --jp-mirror-editor-hr-color: #999;

  /* Vega extension styles */

  --jp-vega-background: white;

  /* Sidebar-related styles */

  --jp-sidebar-min-width: 180px;

  /* Search-related styles */

  --jp-search-toggle-off-opacity: 0.5;
  --jp-search-toggle-hover-opacity: 0.8;
  --jp-search-toggle-on-opacity: 1;
  --jp-search-selected-match-background-color: rgb(245, 200, 0);
  --jp-search-selected-match-color: black;
  --jp-search-unselected-match-background-color: var(
    --jp-inverse-layout-color0
  );
  --jp-search-unselected-match-color: var(--jp-ui-inverse-font-color0);

  /* Icon colors that work well with light or dark backgrounds */
  --jp-icon-contrast-color0: var(--md-purple-600);
  --jp-icon-contrast-color1: var(--md-green-600);
  --jp-icon-contrast-color2: var(--md-pink-600);
  --jp-icon-contrast-color3: var(--md-blue-600);
}
</style>

<style type="text/css">
a.anchor-link {
   display: none;
}
.highlight  {
    margin: 0.4em;
}

/* Input area styling */
.jp-InputArea {
    overflow: hidden;
}

.jp-InputArea-editor {
    overflow: hidden;
}

@media print {
  body {
    margin: 0;
  }
}
</style>



<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-MML-AM_CHTML-full,Safe"> </script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    init_mathjax = function() {
        if (window.MathJax) {
        // MathJax loaded
            MathJax.Hub.Config({
                TeX: {
                    equationNumbers: {
                    autoNumber: "AMS",
                    useLabelIds: true
                    }
                },
                tex2jax: {
                    inlineMath: [ ['$','$'], ["\\(","\\)"] ],
                    displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
                    processEscapes: true,
                    processEnvironments: true
                },
                displayAlign: 'center',
                CommonHTML: {
                    linebreaks: { 
                    automatic: true 
                    }
                },
                "HTML-CSS": {
                    linebreaks: { 
                    automatic: true 
                    }
                }
            });
        
            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
        }
    }
    init_mathjax();
    </script>
    <!-- End of mathjax configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">

<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h1 id="Do-the-grades-students-receive-influence-the-ratings-they-leave-on-professor-reviews?">Do the grades students receive influence the ratings they leave on professor reviews?<a class="anchor-link" href="#Do-the-grades-students-receive-influence-the-ratings-they-leave-on-professor-reviews?">&#182;</a></h1><p>Among people who design course review websites, there is a common concern that the reviews of the professors
paint a misleading picture. The idea is that if a professor is teaching a difficult course, then the average grades they give out will likely be lower. As a result, students will be more likely to negatively rate their experience with that professor, and if someone reads their reviews, they may get the wrong impression that the professor is bad when in reality,
it's just that the course they teach is more difficult.</p>
<p>In this analysis, I will use grade and review data from PlanetTerp to look at the relationship between a professor's ratings
and the grades they give out. According to the PlanetTerp website, the review data comes in part from OurUMD.com. 
Professor and course information comes from umd.io. Grade data comes from the UMD Office of Institutional Research, Planning &amp; Assessment (IRPA) and through a request under the state of Maryland's Public Information Act (PIA) (grade data initially from VAgrades.com).</p>
<p>The null hypothesis will be that there is a positive correlation between a professor's ratings and the grades they give out in their courses.</p>

</div>
</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h1 id="Average-Rating-vs.-Average-GPA">Average Rating vs. Average GPA<a class="anchor-link" href="#Average-Rating-vs.-Average-GPA">&#182;</a></h1>
</div>
</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>Our first task will be to gather some data. There are two things that we need to start out. The average rating of each professor and their average GPA over all the courses they teach. The first of these is really easy. The PlanetTerp API provides the average rating for a requested professor when you hit a certain endpoint.</p>
<p>First, we need to get all of the professors. We will use this code below to build a dataframe object that contains the following properties:</p>
<ul>
<li>name: name of professor</li>
<li>slug</li>
<li>type: professor or TA</li>
<li>courses: list of courses taught</li>
<li>average_rating</li>
</ul>

</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs  ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[205]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">requests</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">import</span> <span class="nn">io</span>
<span class="kn">import</span> <span class="nn">time</span>
<span class="kn">from</span> <span class="nn">bs4</span> <span class="kn">import</span> <span class="n">BeautifulSoup</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>

<span class="n">cur_offset</span> <span class="o">=</span> <span class="mi">0</span>
<span class="n">professor_df</span> <span class="o">=</span> <span class="kc">None</span>
<span class="k">while</span> <span class="n">cur_offset</span> <span class="o">&lt;</span> <span class="mi">11039</span><span class="p">:</span>
    <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mi">3</span><span class="p">)</span>
    <span class="c1"># print(f&quot;Requesting data. Offset is {cur_offset}&quot;)</span>
    <span class="n">req</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;https://api.planetterp.com/v1/professors?limit=1000&amp;offset=</span><span class="si">{</span><span class="n">cur_offset</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">content</span>
    <span class="n">df</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">read_json</span><span class="p">(</span><span class="n">io</span><span class="o">.</span><span class="n">StringIO</span><span class="p">(</span><span class="n">req</span><span class="o">.</span><span class="n">decode</span><span class="p">(</span><span class="s1">&#39;utf-8&#39;</span><span class="p">)))</span>
    <span class="n">cur_offset</span> <span class="o">+=</span> <span class="mi">1000</span>
    <span class="k">if</span> <span class="n">professor_df</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
        <span class="n">professor_df</span> <span class="o">=</span> <span class="n">df</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="n">professor_df</span> <span class="o">=</span> <span class="n">professor_df</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">df</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[206]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">professor_df</span> <span class="o">=</span> <span class="n">professor_df</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">professor_df</span><span class="p">[</span><span class="s2">&quot;type&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;professor&quot;</span><span class="p">]</span> <span class="c1"># Filter out all the TA&#39;s</span>
<span class="n">professor_df</span> <span class="o">=</span> <span class="n">professor_df</span><span class="p">[</span><span class="n">professor_df</span><span class="p">[</span><span class="s2">&quot;average_rating&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">notna</span><span class="p">()]</span> <span class="c1"># Drop anyone who doesn&#39;t have any ratings</span>
<span class="n">professor_df</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[206]:</div>



<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>slug</th>
      <th>type</th>
      <th>courses</th>
      <th>average_rating</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>A Anthony</td>
      <td>anthony</td>
      <td>professor</td>
      <td>[AMST202, AMST203, AMST101]</td>
      <td>1.00</td>
    </tr>
    <tr>
      <th>2</th>
      <td>A Kruglanski</td>
      <td>kruglanski</td>
      <td>professor</td>
      <td>[PSYC743, PSYC748M, PSYC489H, PSYC489T, PSYC78...</td>
      <td>2.00</td>
    </tr>
    <tr>
      <th>4</th>
      <td>A Sharma</td>
      <td>sharma_a</td>
      <td>professor</td>
      <td>[ASTR300]</td>
      <td>1.80</td>
    </tr>
    <tr>
      <th>6</th>
      <td>A.U. Shankar</td>
      <td>shankar_a.u.</td>
      <td>professor</td>
      <td>[CMSC412, CMSC414, CMSC712, CMSC216, CMSC798]</td>
      <td>2.10</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Aaron Allen</td>
      <td>allen_aaron</td>
      <td>professor</td>
      <td>[HHUM205, HHUM206]</td>
      <td>5.00</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Zhengguo Xiao</td>
      <td>xiao_zhengguo</td>
      <td>professor</td>
      <td>[ANSC460, ANSC214, GEMS296, ANSC212, GEMS297, ...</td>
      <td>4.00</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Zhongchi Liu</td>
      <td>liu_zhongchi</td>
      <td>professor</td>
      <td>[BSCI378H, BSCI410, CBMG699Y, MOCB899]</td>
      <td>4.50</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Zita Nunes</td>
      <td>nunes_zita</td>
      <td>professor</td>
      <td>[ENGL234, ENGL749B, ENGL448B, ENGL300, ENGL301...</td>
      <td>3.75</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Zohreh Davoudi</td>
      <td>davoudi</td>
      <td>professor</td>
      <td>[PHYS604, PHYS411, PHYS624]</td>
      <td>2.50</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Zsuzsa Daczo</td>
      <td>daczo</td>
      <td>professor</td>
      <td>[SOCY105, SOCY227, SOCY325, WMST325]</td>
      <td>4.50</td>
    </tr>
  </tbody>
</table>
<p>2481 rows × 5 columns</p>
</div>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>Now that we have a table for our professors, we need to figure out the average GPA they give out for their courses. We'll do this by navigating to their page on PlanetTerp and scraping the content using BeautifulSoup.</p>

</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[207]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">re</span>

<span class="n">base_url</span> <span class="o">=</span> <span class="s2">&quot;https://planetterp.com/professor/&quot;</span>
<span class="n">matches</span> <span class="o">=</span> <span class="p">[]</span>
<span class="k">for</span> <span class="n">idx</span><span class="p">,</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">professor_df</span><span class="o">.</span><span class="n">iterrows</span><span class="p">():</span>
    <span class="n">time</span><span class="o">.</span><span class="n">sleep</span><span class="p">(</span><span class="mf">0.1</span><span class="p">)</span>
    <span class="n">r</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">base_url</span> <span class="o">+</span> <span class="n">row</span><span class="p">[</span><span class="s2">&quot;slug&quot;</span><span class="p">])</span>
    <span class="n">root</span> <span class="o">=</span> <span class="n">BeautifulSoup</span><span class="p">(</span><span class="n">r</span><span class="o">.</span><span class="n">content</span><span class="p">,</span> <span class="s2">&quot;html&quot;</span><span class="p">)</span>
    <span class="n">s</span> <span class="o">=</span> <span class="n">root</span><span class="o">.</span><span class="n">find</span><span class="p">(</span><span class="s2">&quot;strong&quot;</span><span class="p">,</span> <span class="nb">id</span><span class="o">=</span><span class="s2">&quot;grade-statistics&quot;</span><span class="p">)</span> 
    <span class="c1"># print(s)</span>
    <span class="n">search_res</span> <span class="o">=</span> <span class="n">re</span><span class="o">.</span><span class="n">search</span><span class="p">(</span><span class="sa">r</span><span class="s2">&quot;\d\.\d</span><span class="si">{2}</span><span class="s2">&quot;</span><span class="p">,</span> <span class="nb">str</span><span class="p">(</span><span class="n">s</span><span class="p">))</span>
    <span class="k">if</span> <span class="n">search_res</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
        <span class="c1"># print(row[&quot;slug&quot;])</span>
        <span class="n">matches</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">float</span><span class="p">(</span><span class="s2">&quot;NaN&quot;</span><span class="p">))</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="n">matches</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">search_res</span><span class="o">.</span><span class="n">group</span><span class="p">(</span><span class="mi">0</span><span class="p">))</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[207]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>[&#39;2.48&#39;,
 &#39;3.49&#39;,
 &#39;2.82&#39;,
 &#39;2.41&#39;,
 &#39;3.61&#39;,
 &#39;2.52&#39;,
 &#39;2.53&#39;,
 &#39;3.70&#39;,
 &#39;3.82&#39;,
 &#39;3.10&#39;,
 &#39;3.14&#39;,
 &#39;3.37&#39;,
 &#39;3.19&#39;,
 &#39;3.01&#39;,
 &#39;3.18&#39;,
 &#39;2.88&#39;,
 &#39;3.08&#39;,
 nan,
 &#39;3.13&#39;,
 &#39;3.23&#39;,
 &#39;3.21&#39;,
 &#39;3.18&#39;,
 &#39;2.53&#39;,
 &#39;2.49&#39;,
 &#39;3.17&#39;,
 nan,
 &#39;2.91&#39;,
 &#39;3.99&#39;,
 &#39;3.51&#39;,
 &#39;2.87&#39;,
 &#39;3.20&#39;,
 &#39;2.91&#39;,
 &#39;3.31&#39;,
 &#39;2.89&#39;,
 &#39;2.64&#39;,
 &#39;2.94&#39;,
 &#39;3.17&#39;,
 &#39;3.57&#39;,
 &#39;3.20&#39;,
 &#39;3.12&#39;,
 &#39;3.42&#39;,
 &#39;2.81&#39;,
 &#39;2.95&#39;,
 &#39;2.55&#39;,
 &#39;3.15&#39;,
 &#39;3.29&#39;,
 &#39;3.42&#39;,
 &#39;2.98&#39;,
 &#39;3.52&#39;,
 &#39;3.29&#39;,
 &#39;2.73&#39;,
 &#39;2.62&#39;,
 nan,
 &#39;3.59&#39;,
 &#39;3.07&#39;,
 &#39;2.24&#39;,
 &#39;2.49&#39;,
 nan,
 &#39;3.25&#39;,
 &#39;3.31&#39;,
 &#39;3.71&#39;,
 &#39;3.39&#39;,
 &#39;2.98&#39;,
 &#39;3.33&#39;,
 &#39;3.20&#39;,
 &#39;3.80&#39;,
 &#39;2.91&#39;,
 &#39;2.94&#39;,
 &#39;3.41&#39;,
 nan,
 &#39;3.50&#39;,
 &#39;3.42&#39;,
 &#39;3.70&#39;,
 &#39;3.40&#39;,
 &#39;3.85&#39;,
 &#39;2.80&#39;,
 &#39;3.18&#39;,
 &#39;2.59&#39;,
 &#39;2.40&#39;,
 &#39;2.48&#39;,
 &#39;3.59&#39;,
 &#39;3.48&#39;,
 &#39;3.83&#39;,
 &#39;3.71&#39;,
 &#39;3.56&#39;,
 &#39;2.14&#39;,
 &#39;2.90&#39;,
 &#39;3.41&#39;,
 &#39;2.72&#39;,
 &#39;2.58&#39;,
 &#39;3.65&#39;,
 &#39;3.48&#39;,
 &#39;2.79&#39;,
 &#39;2.81&#39;,
 &#39;3.44&#39;,
 &#39;3.49&#39;,
 &#39;3.33&#39;,
 &#39;3.58&#39;,
 &#39;2.34&#39;,
 &#39;3.21&#39;,
 &#39;3.40&#39;,
 &#39;2.76&#39;,
 &#39;3.37&#39;,
 &#39;3.54&#39;,
 &#39;2.61&#39;,
 &#39;3.27&#39;,
 &#39;3.55&#39;,
 &#39;3.42&#39;,
 &#39;3.60&#39;,
 &#39;3.51&#39;,
 &#39;2.44&#39;,
 &#39;3.00&#39;,
 &#39;3.11&#39;,
 &#39;3.64&#39;,
 &#39;3.01&#39;,
 &#39;3.56&#39;,
 &#39;3.21&#39;,
 &#39;3.51&#39;,
 &#39;3.04&#39;,
 &#39;3.80&#39;,
 &#39;3.03&#39;,
 &#39;3.10&#39;,
 &#39;3.71&#39;,
 &#39;3.13&#39;,
 &#39;3.36&#39;,
 &#39;3.46&#39;,
 nan,
 &#39;3.18&#39;,
 &#39;3.62&#39;,
 &#39;3.42&#39;,
 &#39;3.38&#39;,
 &#39;2.48&#39;,
 &#39;3.38&#39;,
 &#39;3.13&#39;,
 &#39;3.32&#39;,
 &#39;3.71&#39;,
 &#39;2.75&#39;,
 nan,
 &#39;3.31&#39;,
 &#39;2.89&#39;,
 &#39;3.55&#39;,
 &#39;3.44&#39;,
 &#39;3.17&#39;,
 &#39;3.86&#39;,
 &#39;2.81&#39;,
 nan,
 &#39;3.48&#39;,
 &#39;3.04&#39;,
 &#39;3.46&#39;,
 &#39;3.29&#39;,
 &#39;3.31&#39;,
 &#39;2.79&#39;,
 &#39;3.23&#39;,
 &#39;3.50&#39;,
 &#39;3.41&#39;,
 &#39;3.75&#39;,
 &#39;2.63&#39;,
 &#39;3.28&#39;,
 &#39;3.14&#39;,
 &#39;2.78&#39;,
 &#39;3.70&#39;,
 &#39;3.35&#39;,
 &#39;3.99&#39;,
 &#39;2.27&#39;,
 &#39;3.43&#39;,
 &#39;3.41&#39;,
 &#39;3.50&#39;,
 &#39;3.35&#39;,
 &#39;2.88&#39;,
 &#39;3.17&#39;,
 &#39;3.69&#39;,
 &#39;3.70&#39;,
 &#39;0.00&#39;,
 &#39;3.33&#39;,
 &#39;3.48&#39;,
 nan,
 &#39;3.06&#39;,
 &#39;2.29&#39;,
 &#39;3.70&#39;,
 &#39;3.45&#39;,
 &#39;2.25&#39;,
 &#39;2.54&#39;,
 &#39;3.20&#39;,
 &#39;2.69&#39;,
 &#39;2.99&#39;,
 &#39;2.68&#39;,
 &#39;2.81&#39;,
 &#39;3.07&#39;,
 &#39;1.71&#39;,
 &#39;2.90&#39;,
 &#39;3.29&#39;,
 &#39;3.73&#39;,
 &#39;2.26&#39;,
 &#39;3.28&#39;,
 &#39;2.04&#39;,
 &#39;2.85&#39;,
 nan,
 &#39;3.37&#39;,
 &#39;3.72&#39;,
 &#39;3.78&#39;,
 &#39;3.38&#39;,
 &#39;3.22&#39;,
 &#39;2.94&#39;,
 &#39;3.38&#39;,
 &#39;3.94&#39;,
 &#39;3.62&#39;,
 &#39;3.47&#39;,
 &#39;3.16&#39;,
 &#39;3.07&#39;,
 &#39;3.54&#39;,
 &#39;3.63&#39;,
 &#39;3.30&#39;,
 &#39;3.35&#39;,
 &#39;3.40&#39;,
 &#39;3.83&#39;,
 &#39;3.30&#39;,
 &#39;3.54&#39;,
 &#39;3.82&#39;,
 &#39;3.10&#39;,
 &#39;3.43&#39;,
 &#39;3.29&#39;,
 &#39;3.54&#39;,
 &#39;3.76&#39;,
 nan,
 &#39;3.35&#39;,
 &#39;3.56&#39;,
 &#39;2.95&#39;,
 &#39;0.71&#39;,
 &#39;3.38&#39;,
 &#39;3.15&#39;,
 &#39;3.52&#39;,
 &#39;3.04&#39;,
 &#39;2.65&#39;,
 &#39;3.05&#39;,
 &#39;3.32&#39;,
 &#39;2.77&#39;,
 &#39;2.04&#39;,
 &#39;2.99&#39;,
 &#39;3.75&#39;,
 &#39;3.20&#39;,
 &#39;2.89&#39;,
 &#39;3.68&#39;,
 nan,
 &#39;3.08&#39;,
 &#39;3.14&#39;,
 &#39;3.64&#39;,
 &#39;3.34&#39;,
 &#39;3.18&#39;,
 &#39;3.29&#39;,
 &#39;2.96&#39;,
 &#39;3.39&#39;,
 &#39;3.51&#39;,
 nan,
 &#39;3.25&#39;,
 &#39;3.39&#39;,
 &#39;3.25&#39;,
 &#39;2.98&#39;,
 &#39;3.04&#39;,
 &#39;3.17&#39;,
 &#39;2.35&#39;,
 &#39;3.48&#39;,
 &#39;3.67&#39;,
 &#39;3.04&#39;,
 &#39;2.28&#39;,
 nan,
 &#39;2.71&#39;,
 nan,
 &#39;2.37&#39;,
 &#39;3.28&#39;,
 &#39;2.22&#39;,
 &#39;3.73&#39;,
 &#39;3.45&#39;,
 &#39;3.46&#39;,
 &#39;2.93&#39;,
 &#39;3.17&#39;,
 &#39;3.58&#39;,
 &#39;3.44&#39;,
 &#39;3.16&#39;,
 &#39;3.50&#39;,
 &#39;3.57&#39;,
 &#39;3.06&#39;,
 &#39;3.87&#39;,
 &#39;3.65&#39;,
 &#39;3.19&#39;,
 nan,
 &#39;3.22&#39;,
 &#39;3.43&#39;,
 &#39;3.52&#39;,
 &#39;3.33&#39;,
 &#39;3.27&#39;,
 &#39;2.23&#39;,
 nan,
 &#39;3.58&#39;,
 &#39;3.88&#39;,
 &#39;3.06&#39;,
 &#39;3.46&#39;,
 &#39;3.10&#39;,
 &#39;2.29&#39;,
 &#39;3.16&#39;,
 &#39;2.95&#39;,
 &#39;3.85&#39;,
 &#39;3.64&#39;,
 &#39;2.81&#39;,
 &#39;3.31&#39;,
 &#39;3.33&#39;,
 &#39;3.84&#39;,
 &#39;3.62&#39;,
 nan,
 &#39;3.36&#39;,
 &#39;3.09&#39;,
 &#39;2.84&#39;,
 &#39;3.36&#39;,
 &#39;3.53&#39;,
 &#39;3.63&#39;,
 &#39;3.54&#39;,
 &#39;2.15&#39;,
 &#39;3.51&#39;,
 &#39;3.42&#39;,
 nan,
 &#39;3.55&#39;,
 &#39;3.51&#39;,
 &#39;3.25&#39;,
 &#39;2.37&#39;,
 &#39;3.21&#39;,
 &#39;3.44&#39;,
 &#39;3.45&#39;,
 &#39;2.75&#39;,
 &#39;2.75&#39;,
 &#39;2.42&#39;,
 &#39;3.03&#39;,
 &#39;3.59&#39;,
 &#39;3.04&#39;,
 &#39;3.56&#39;,
 &#39;3.18&#39;,
 &#39;2.93&#39;,
 &#39;3.24&#39;,
 &#39;3.56&#39;,
 &#39;2.98&#39;,
 &#39;3.82&#39;,
 &#39;3.09&#39;,
 &#39;3.46&#39;,
 &#39;3.62&#39;,
 &#39;3.73&#39;,
 &#39;2.93&#39;,
 &#39;2.85&#39;,
 &#39;3.45&#39;,
 &#39;2.84&#39;,
 &#39;3.47&#39;,
 &#39;3.70&#39;,
 &#39;2.86&#39;,
 &#39;2.12&#39;,
 &#39;3.32&#39;,
 &#39;3.37&#39;,
 &#39;2.49&#39;,
 &#39;2.52&#39;,
 &#39;2.95&#39;,
 &#39;3.48&#39;,
 &#39;2.93&#39;,
 &#39;2.57&#39;,
 &#39;3.43&#39;,
 &#39;3.75&#39;,
 &#39;3.68&#39;,
 &#39;2.57&#39;,
 &#39;3.79&#39;,
 &#39;2.40&#39;,
 &#39;3.41&#39;,
 &#39;2.24&#39;,
 &#39;3.27&#39;,
 &#39;3.25&#39;,
 &#39;3.39&#39;,
 &#39;3.60&#39;,
 &#39;3.38&#39;,
 &#39;2.47&#39;,
 &#39;2.72&#39;,
 &#39;2.73&#39;,
 &#39;3.34&#39;,
 &#39;3.46&#39;,
 &#39;3.42&#39;,
 &#39;3.10&#39;,
 &#39;2.85&#39;,
 &#39;3.57&#39;,
 &#39;2.88&#39;,
 &#39;3.35&#39;,
 &#39;3.08&#39;,
 &#39;3.23&#39;,
 &#39;3.21&#39;,
 &#39;2.68&#39;,
 &#39;2.72&#39;,
 &#39;2.85&#39;,
 &#39;3.39&#39;,
 &#39;3.45&#39;,
 &#39;3.46&#39;,
 &#39;3.27&#39;,
 &#39;3.59&#39;,
 &#39;2.84&#39;,
 &#39;2.83&#39;,
 &#39;3.09&#39;,
 &#39;2.80&#39;,
 &#39;2.91&#39;,
 &#39;2.91&#39;,
 &#39;3.78&#39;,
 &#39;3.11&#39;,
 &#39;3.47&#39;,
 &#39;3.02&#39;,
 &#39;3.39&#39;,
 &#39;3.22&#39;,
 &#39;3.01&#39;,
 &#39;3.82&#39;,
 &#39;3.78&#39;,
 &#39;3.67&#39;,
 &#39;2.96&#39;,
 &#39;3.70&#39;,
 &#39;3.49&#39;,
 &#39;3.82&#39;,
 &#39;3.68&#39;,
 nan,
 &#39;2.32&#39;,
 &#39;2.51&#39;,
 &#39;3.93&#39;,
 &#39;2.51&#39;,
 &#39;3.29&#39;,
 &#39;0.00&#39;,
 &#39;3.25&#39;,
 &#39;3.03&#39;,
 &#39;3.78&#39;,
 &#39;3.37&#39;,
 &#39;3.02&#39;,
 nan,
 &#39;3.14&#39;,
 &#39;3.27&#39;,
 &#39;2.87&#39;,
 &#39;3.94&#39;,
 &#39;2.45&#39;,
 &#39;3.81&#39;,
 &#39;3.49&#39;,
 &#39;3.60&#39;,
 &#39;3.53&#39;,
 &#39;3.51&#39;,
 &#39;3.31&#39;,
 &#39;2.96&#39;,
 &#39;2.95&#39;,
 &#39;2.64&#39;,
 &#39;3.14&#39;,
 &#39;3.15&#39;,
 &#39;3.33&#39;,
 &#39;3.21&#39;,
 &#39;2.78&#39;,
 &#39;3.70&#39;,
 &#39;2.64&#39;,
 &#39;2.84&#39;,
 &#39;3.12&#39;,
 &#39;3.24&#39;,
 &#39;2.68&#39;,
 &#39;2.72&#39;,
 &#39;3.35&#39;,
 &#39;3.24&#39;,
 &#39;3.14&#39;,
 &#39;3.02&#39;,
 nan,
 &#39;3.19&#39;,
 &#39;2.66&#39;,
 &#39;3.19&#39;,
 &#39;3.81&#39;,
 &#39;3.52&#39;,
 &#39;3.35&#39;,
 &#39;3.41&#39;,
 &#39;3.27&#39;,
 &#39;3.09&#39;,
 &#39;2.53&#39;,
 &#39;3.90&#39;,
 &#39;3.18&#39;,
 &#39;2.40&#39;,
 &#39;3.52&#39;,
 &#39;3.33&#39;,
 &#39;3.84&#39;,
 &#39;3.25&#39;,
 nan,
 &#39;3.10&#39;,
 &#39;3.57&#39;,
 &#39;2.78&#39;,
 &#39;3.59&#39;,
 &#39;3.02&#39;,
 &#39;3.49&#39;,
 &#39;3.16&#39;,
 &#39;3.56&#39;,
 &#39;3.26&#39;,
 &#39;3.33&#39;,
 &#39;2.74&#39;,
 &#39;3.24&#39;,
 &#39;2.70&#39;,
 nan,
 &#39;1.86&#39;,
 &#39;3.50&#39;,
 &#39;3.20&#39;,
 &#39;3.23&#39;,
 &#39;3.47&#39;,
 &#39;4.00&#39;,
 &#39;3.40&#39;,
 &#39;2.59&#39;,
 &#39;3.15&#39;,
 &#39;3.41&#39;,
 &#39;3.59&#39;,
 &#39;3.32&#39;,
 &#39;2.79&#39;,
 &#39;3.19&#39;,
 &#39;3.15&#39;,
 &#39;2.87&#39;,
 &#39;2.84&#39;,
 &#39;2.48&#39;,
 &#39;2.38&#39;,
 &#39;3.06&#39;,
 &#39;3.35&#39;,
 &#39;3.01&#39;,
 &#39;3.55&#39;,
 &#39;3.43&#39;,
 &#39;3.78&#39;,
 &#39;2.68&#39;,
 &#39;3.37&#39;,
 &#39;3.75&#39;,
 &#39;3.28&#39;,
 &#39;2.48&#39;,
 &#39;2.80&#39;,
 &#39;3.92&#39;,
 &#39;3.86&#39;,
 &#39;3.39&#39;,
 &#39;3.70&#39;,
 &#39;3.84&#39;,
 &#39;3.46&#39;,
 &#39;3.49&#39;,
 &#39;2.59&#39;,
 &#39;3.09&#39;,
 &#39;3.02&#39;,
 &#39;3.64&#39;,
 &#39;3.70&#39;,
 &#39;3.78&#39;,
 &#39;3.12&#39;,
 &#39;3.32&#39;,
 &#39;2.91&#39;,
 &#39;3.48&#39;,
 &#39;3.57&#39;,
 &#39;3.51&#39;,
 &#39;2.31&#39;,
 &#39;3.43&#39;,
 &#39;2.98&#39;,
 &#39;3.17&#39;,
 &#39;3.90&#39;,
 &#39;2.72&#39;,
 &#39;3.38&#39;,
 &#39;3.15&#39;,
 &#39;3.42&#39;,
 &#39;3.22&#39;,
 &#39;3.49&#39;,
 &#39;3.38&#39;,
 &#39;3.11&#39;,
 &#39;2.82&#39;,
 &#39;3.88&#39;,
 &#39;2.70&#39;,
 &#39;1.60&#39;,
 &#39;3.16&#39;,
 nan,
 &#39;2.73&#39;,
 &#39;3.61&#39;,
 &#39;2.00&#39;,
 &#39;3.54&#39;,
 &#39;3.26&#39;,
 &#39;3.12&#39;,
 &#39;3.09&#39;,
 &#39;3.56&#39;,
 &#39;3.53&#39;,
 &#39;3.73&#39;,
 &#39;2.84&#39;,
 &#39;3.20&#39;,
 &#39;2.63&#39;,
 &#39;2.54&#39;,
 &#39;3.15&#39;,
 &#39;3.57&#39;,
 &#39;3.31&#39;,
 &#39;2.82&#39;,
 &#39;2.63&#39;,
 &#39;3.59&#39;,
 &#39;3.06&#39;,
 &#39;2.58&#39;,
 &#39;3.97&#39;,
 &#39;2.63&#39;,
 &#39;3.02&#39;,
 &#39;2.65&#39;,
 &#39;3.36&#39;,
 &#39;3.25&#39;,
 &#39;3.30&#39;,
 &#39;3.42&#39;,
 &#39;3.77&#39;,
 &#39;2.86&#39;,
 &#39;3.51&#39;,
 &#39;3.80&#39;,
 &#39;2.40&#39;,
 nan,
 &#39;3.22&#39;,
 &#39;3.32&#39;,
 &#39;2.63&#39;,
 &#39;3.14&#39;,
 &#39;3.30&#39;,
 &#39;3.65&#39;,
 &#39;3.38&#39;,
 &#39;2.52&#39;,
 &#39;2.84&#39;,
 &#39;3.49&#39;,
 &#39;3.48&#39;,
 &#39;3.15&#39;,
 &#39;3.43&#39;,
 &#39;3.02&#39;,
 &#39;2.64&#39;,
 &#39;3.71&#39;,
 &#39;3.48&#39;,
 nan,
 &#39;3.72&#39;,
 &#39;3.74&#39;,
 nan,
 &#39;3.54&#39;,
 &#39;2.58&#39;,
 &#39;2.14&#39;,
 &#39;3.41&#39;,
 &#39;3.91&#39;,
 &#39;3.50&#39;,
 &#39;2.90&#39;,
 &#39;3.65&#39;,
 &#39;2.92&#39;,
 &#39;3.16&#39;,
 &#39;3.17&#39;,
 &#39;3.85&#39;,
 nan,
 &#39;3.03&#39;,
 &#39;3.51&#39;,
 &#39;3.47&#39;,
 &#39;3.57&#39;,
 &#39;2.84&#39;,
 &#39;3.94&#39;,
 nan,
 &#39;3.01&#39;,
 &#39;2.57&#39;,
 nan,
 &#39;4.00&#39;,
 &#39;3.06&#39;,
 &#39;3.38&#39;,
 &#39;3.27&#39;,
 nan,
 &#39;3.09&#39;,
 &#39;3.89&#39;,
 &#39;3.88&#39;,
 &#39;2.88&#39;,
 &#39;3.73&#39;,
 &#39;3.38&#39;,
 &#39;2.83&#39;,
 &#39;3.61&#39;,
 &#39;3.83&#39;,
 &#39;3.58&#39;,
 &#39;2.93&#39;,
 &#39;3.63&#39;,
 &#39;3.04&#39;,
 &#39;2.96&#39;,
 &#39;3.56&#39;,
 &#39;2.99&#39;,
 &#39;3.26&#39;,
 &#39;3.81&#39;,
 nan,
 &#39;2.97&#39;,
 &#39;3.61&#39;,
 &#39;3.78&#39;,
 &#39;3.11&#39;,
 &#39;2.82&#39;,
 &#39;3.68&#39;,
 &#39;2.76&#39;,
 &#39;3.01&#39;,
 &#39;2.94&#39;,
 &#39;3.58&#39;,
 &#39;3.24&#39;,
 &#39;2.65&#39;,
 &#39;3.70&#39;,
 &#39;3.23&#39;,
 &#39;2.98&#39;,
 &#39;3.03&#39;,
 &#39;3.10&#39;,
 &#39;3.11&#39;,
 &#39;2.18&#39;,
 &#39;3.61&#39;,
 &#39;3.06&#39;,
 &#39;3.60&#39;,
 &#39;3.78&#39;,
 &#39;3.33&#39;,
 &#39;3.78&#39;,
 &#39;2.58&#39;,
 &#39;2.52&#39;,
 &#39;3.81&#39;,
 nan,
 &#39;3.34&#39;,
 &#39;2.73&#39;,
 &#39;3.01&#39;,
 &#39;3.70&#39;,
 &#39;3.28&#39;,
 &#39;2.91&#39;,
 &#39;2.91&#39;,
 &#39;3.30&#39;,
 &#39;3.12&#39;,
 &#39;3.39&#39;,
 &#39;2.76&#39;,
 &#39;2.49&#39;,
 &#39;3.45&#39;,
 nan,
 &#39;2.98&#39;,
 &#39;3.49&#39;,
 &#39;2.85&#39;,
 &#39;3.10&#39;,
 &#39;3.54&#39;,
 &#39;3.26&#39;,
 nan,
 &#39;3.30&#39;,
 nan,
 &#39;3.59&#39;,
 &#39;2.41&#39;,
 &#39;3.07&#39;,
 &#39;2.74&#39;,
 &#39;3.60&#39;,
 &#39;3.15&#39;,
 &#39;3.44&#39;,
 &#39;3.31&#39;,
 &#39;1.68&#39;,
 &#39;3.39&#39;,
 &#39;3.85&#39;,
 &#39;3.17&#39;,
 &#39;3.11&#39;,
 &#39;3.07&#39;,
 &#39;3.05&#39;,
 &#39;3.34&#39;,
 &#39;3.50&#39;,
 &#39;2.81&#39;,
 &#39;3.36&#39;,
 &#39;3.73&#39;,
 &#39;3.49&#39;,
 &#39;3.61&#39;,
 &#39;3.43&#39;,
 &#39;3.43&#39;,
 &#39;3.23&#39;,
 &#39;3.05&#39;,
 &#39;2.65&#39;,
 &#39;3.58&#39;,
 &#39;3.32&#39;,
 &#39;3.32&#39;,
 &#39;2.82&#39;,
 &#39;3.42&#39;,
 &#39;2.97&#39;,
 &#39;3.08&#39;,
 &#39;3.51&#39;,
 &#39;3.69&#39;,
 &#39;3.53&#39;,
 nan,
 &#39;3.12&#39;,
 &#39;3.34&#39;,
 &#39;3.13&#39;,
 &#39;3.51&#39;,
 &#39;3.74&#39;,
 &#39;3.49&#39;,
 &#39;2.74&#39;,
 &#39;3.67&#39;,
 &#39;3.57&#39;,
 &#39;2.22&#39;,
 &#39;3.01&#39;,
 &#39;3.50&#39;,
 &#39;2.72&#39;,
 &#39;3.63&#39;,
 &#39;3.38&#39;,
 &#39;3.65&#39;,
 &#39;3.07&#39;,
 &#39;3.63&#39;,
 &#39;3.01&#39;,
 &#39;3.69&#39;,
 &#39;3.61&#39;,
 nan,
 &#39;3.09&#39;,
 &#39;3.15&#39;,
 &#39;2.73&#39;,
 &#39;3.04&#39;,
 &#39;3.72&#39;,
 &#39;2.89&#39;,
 &#39;2.97&#39;,
 &#39;2.82&#39;,
 &#39;3.23&#39;,
 &#39;3.22&#39;,
 &#39;3.40&#39;,
 &#39;3.23&#39;,
 &#39;4.00&#39;,
 &#39;2.73&#39;,
 &#39;2.82&#39;,
 &#39;2.92&#39;,
 &#39;2.95&#39;,
 &#39;3.14&#39;,
 &#39;3.14&#39;,
 &#39;3.58&#39;,
 &#39;3.25&#39;,
 &#39;3.14&#39;,
 &#39;3.39&#39;,
 &#39;3.50&#39;,
 &#39;3.92&#39;,
 &#39;3.09&#39;,
 &#39;3.65&#39;,
 &#39;3.75&#39;,
 &#39;2.99&#39;,
 &#39;2.72&#39;,
 &#39;3.36&#39;,
 &#39;3.90&#39;,
 &#39;3.48&#39;,
 &#39;3.27&#39;,
 &#39;3.61&#39;,
 nan,
 &#39;2.65&#39;,
 &#39;3.48&#39;,
 nan,
 &#39;3.12&#39;,
 &#39;2.92&#39;,
 &#39;3.45&#39;,
 &#39;2.31&#39;,
 &#39;3.25&#39;,
 &#39;3.73&#39;,
 &#39;3.50&#39;,
 &#39;3.54&#39;,
 nan,
 &#39;3.36&#39;,
 &#39;3.64&#39;,
 &#39;2.50&#39;,
 &#39;3.40&#39;,
 &#39;3.64&#39;,
 &#39;2.55&#39;,
 &#39;3.44&#39;,
 &#39;2.81&#39;,
 &#39;2.49&#39;,
 &#39;3.07&#39;,
 &#39;2.70&#39;,
 nan,
 &#39;3.37&#39;,
 &#39;0.00&#39;,
 nan,
 &#39;3.65&#39;,
 &#39;3.24&#39;,
 &#39;3.07&#39;,
 &#39;2.74&#39;,
 &#39;3.63&#39;,
 &#39;3.27&#39;,
 &#39;3.13&#39;,
 &#39;3.66&#39;,
 &#39;2.97&#39;,
 &#39;3.49&#39;,
 &#39;3.06&#39;,
 &#39;2.70&#39;,
 &#39;2.83&#39;,
 &#39;3.75&#39;,
 &#39;3.21&#39;,
 &#39;3.95&#39;,
 &#39;3.06&#39;,
 &#39;3.54&#39;,
 &#39;3.67&#39;,
 &#39;3.66&#39;,
 &#39;2.57&#39;,
 &#39;3.30&#39;,
 &#39;2.78&#39;,
 &#39;2.59&#39;,
 &#39;2.72&#39;,
 &#39;3.25&#39;,
 &#39;3.97&#39;,
 &#39;3.16&#39;,
 &#39;2.43&#39;,
 &#39;3.43&#39;,
 &#39;3.35&#39;,
 &#39;3.16&#39;,
 &#39;3.80&#39;,
 &#39;2.42&#39;,
 &#39;3.49&#39;,
 &#39;3.41&#39;,
 &#39;3.26&#39;,
 &#39;2.80&#39;,
 nan,
 &#39;3.13&#39;,
 &#39;3.62&#39;,
 &#39;3.09&#39;,
 &#39;3.60&#39;,
 &#39;3.56&#39;,
 &#39;3.36&#39;,
 &#39;2.99&#39;,
 &#39;2.42&#39;,
 &#39;3.58&#39;,
 &#39;3.37&#39;,
 &#39;2.05&#39;,
 &#39;3.18&#39;,
 &#39;3.64&#39;,
 &#39;3.13&#39;,
 &#39;3.01&#39;,
 &#39;3.44&#39;,
 &#39;3.14&#39;,
 &#39;3.39&#39;,
 nan,
 &#39;3.27&#39;,
 &#39;1.19&#39;,
 &#39;3.43&#39;,
 &#39;3.67&#39;,
 nan,
 &#39;2.10&#39;,
 &#39;3.23&#39;,
 &#39;2.88&#39;,
 &#39;3.11&#39;,
 &#39;2.32&#39;,
 &#39;3.07&#39;,
 &#39;3.15&#39;,
 &#39;3.38&#39;,
 &#39;3.52&#39;,
 &#39;2.65&#39;,
 &#39;3.46&#39;,
 &#39;3.12&#39;,
 &#39;3.66&#39;,
 &#39;3.62&#39;,
 &#39;3.17&#39;,
 &#39;3.44&#39;,
 &#39;3.85&#39;,
 &#39;3.14&#39;,
 &#39;2.56&#39;,
 &#39;3.35&#39;,
 &#39;3.80&#39;,
 &#39;3.06&#39;,
 &#39;3.31&#39;,
 &#39;3.61&#39;,
 &#39;3.46&#39;,
 &#39;2.75&#39;,
 &#39;3.52&#39;,
 &#39;2.82&#39;,
 &#39;3.11&#39;,
 &#39;2.64&#39;,
 &#39;3.68&#39;,
 &#39;3.31&#39;,
 &#39;3.47&#39;,
 &#39;3.01&#39;,
 &#39;3.12&#39;,
 &#39;3.33&#39;,
 &#39;2.61&#39;,
 &#39;3.47&#39;,
 &#39;3.10&#39;,
 &#39;3.57&#39;,
 &#39;3.73&#39;,
 &#39;2.84&#39;,
 &#39;3.58&#39;,
 &#39;3.53&#39;,
 &#39;3.01&#39;,
 &#39;3.07&#39;,
 &#39;3.57&#39;,
 &#39;3.17&#39;,
 &#39;2.95&#39;,
 &#39;3.38&#39;,
 &#39;2.65&#39;,
 &#39;2.81&#39;,
 &#39;3.46&#39;,
 &#39;3.24&#39;,
 &#39;3.51&#39;,
 &#39;3.25&#39;,
 nan,
 &#39;3.33&#39;,
 &#39;3.71&#39;,
 &#39;2.70&#39;,
 &#39;2.66&#39;,
 &#39;3.35&#39;,
 &#39;3.06&#39;,
 &#39;3.30&#39;,
 &#39;3.60&#39;,
 &#39;3.04&#39;,
 nan,
 &#39;3.19&#39;,
 &#39;3.95&#39;,
 &#39;2.81&#39;,
 &#39;3.02&#39;,
 &#39;3.60&#39;,
 &#39;3.02&#39;,
 &#39;2.28&#39;,
 &#39;3.83&#39;,
 &#39;2.90&#39;,
 &#39;2.81&#39;,
 &#39;2.86&#39;,
 &#39;2.85&#39;,
 &#39;3.28&#39;,
 &#39;3.17&#39;,
 &#39;3.08&#39;,
 &#39;3.18&#39;,
 &#39;3.50&#39;,
 &#39;2.94&#39;,
 &#39;3.51&#39;,
 &#39;3.59&#39;,
 &#39;3.37&#39;,
 &#39;3.33&#39;,
 &#39;2.88&#39;,
 &#39;3.54&#39;,
 &#39;3.52&#39;,
 nan,
 &#39;3.58&#39;,
 &#39;3.53&#39;,
 &#39;3.61&#39;,
 &#39;3.67&#39;,
 &#39;2.59&#39;,
 ...]</pre>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[208]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">professor_df</span><span class="p">[</span><span class="s2">&quot;average_gpa&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">matches</span>
<span class="n">old_professor_df</span> <span class="o">=</span> <span class="n">professor_df</span>
<span class="n">professor_df</span> <span class="o">=</span> <span class="n">professor_df</span><span class="p">[</span><span class="n">professor_df</span><span class="p">[</span><span class="s2">&quot;average_gpa&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">notna</span><span class="p">()]</span> <span class="c1"># Drop anyone who doesn&#39;t have an average gpa</span>
<span class="n">professor_df</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[208]:</div>



<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>slug</th>
      <th>type</th>
      <th>courses</th>
      <th>average_rating</th>
      <th>average_gpa</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>A Anthony</td>
      <td>anthony</td>
      <td>professor</td>
      <td>[AMST202, AMST203, AMST101]</td>
      <td>1.00</td>
      <td>2.48</td>
    </tr>
    <tr>
      <th>2</th>
      <td>A Kruglanski</td>
      <td>kruglanski</td>
      <td>professor</td>
      <td>[PSYC743, PSYC748M, PSYC489H, PSYC489T, PSYC78...</td>
      <td>2.00</td>
      <td>3.49</td>
    </tr>
    <tr>
      <th>4</th>
      <td>A Sharma</td>
      <td>sharma_a</td>
      <td>professor</td>
      <td>[ASTR300]</td>
      <td>1.80</td>
      <td>2.82</td>
    </tr>
    <tr>
      <th>6</th>
      <td>A.U. Shankar</td>
      <td>shankar_a.u.</td>
      <td>professor</td>
      <td>[CMSC412, CMSC414, CMSC712, CMSC216, CMSC798]</td>
      <td>2.10</td>
      <td>2.41</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Aaron Allen</td>
      <td>allen_aaron</td>
      <td>professor</td>
      <td>[HHUM205, HHUM206]</td>
      <td>5.00</td>
      <td>3.61</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Zhengguo Xiao</td>
      <td>xiao_zhengguo</td>
      <td>professor</td>
      <td>[ANSC460, ANSC214, GEMS296, ANSC212, GEMS297, ...</td>
      <td>4.00</td>
      <td>2.95</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Zhongchi Liu</td>
      <td>liu_zhongchi</td>
      <td>professor</td>
      <td>[BSCI378H, BSCI410, CBMG699Y, MOCB899]</td>
      <td>4.50</td>
      <td>3.37</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Zita Nunes</td>
      <td>nunes_zita</td>
      <td>professor</td>
      <td>[ENGL234, ENGL749B, ENGL448B, ENGL300, ENGL301...</td>
      <td>3.75</td>
      <td>2.75</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Zohreh Davoudi</td>
      <td>davoudi</td>
      <td>professor</td>
      <td>[PHYS604, PHYS411, PHYS624]</td>
      <td>2.50</td>
      <td>3.38</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Zsuzsa Daczo</td>
      <td>daczo</td>
      <td>professor</td>
      <td>[SOCY105, SOCY227, SOCY325, WMST325]</td>
      <td>4.50</td>
      <td>3.62</td>
    </tr>
  </tbody>
</table>
<p>2363 rows × 6 columns</p>
</div>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[209]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="n">plt</span><span class="o">.</span><span class="n">rcParams</span><span class="p">[</span><span class="s1">&#39;figure.figsize&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="mi">10</span><span class="p">,</span> <span class="mi">8</span><span class="p">]</span>
<span class="n">average_rating</span> <span class="o">=</span> <span class="p">[</span><span class="nb">float</span><span class="p">(</span><span class="n">x</span><span class="p">)</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">professor_df</span><span class="p">[</span><span class="s2">&quot;average_rating&quot;</span><span class="p">]]</span>
<span class="n">average_gpa</span> <span class="o">=</span> <span class="p">[</span><span class="nb">float</span><span class="p">(</span><span class="n">x</span><span class="p">)</span> <span class="k">for</span> <span class="n">x</span> <span class="ow">in</span> <span class="n">professor_df</span><span class="p">[</span><span class="s2">&quot;average_gpa&quot;</span><span class="p">]]</span>
<span class="c1"># print(average_gpa)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">scatter</span><span class="p">(</span><span class="n">x</span><span class="o">=</span><span class="n">average_rating</span><span class="p">,</span> <span class="n">y</span><span class="o">=</span><span class="n">average_gpa</span><span class="p">,</span> <span class="n">s</span><span class="o">=</span><span class="mi">2</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="s2">&quot;Average rating vs. Average GPA&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Average rating&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Average GPA&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylim</span><span class="p">([</span><span class="mi">1</span><span class="p">,</span><span class="mi">4</span><span class="p">])</span>
<span class="n">plt</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">unique</span><span class="p">(</span><span class="n">average_rating</span><span class="p">),</span> <span class="n">np</span><span class="o">.</span><span class="n">poly1d</span><span class="p">(</span><span class="n">np</span><span class="o">.</span><span class="n">polyfit</span><span class="p">(</span><span class="n">average_rating</span><span class="p">,</span> <span class="n">average_gpa</span><span class="p">,</span> <span class="mi">1</span><span class="p">))(</span><span class="n">np</span><span class="o">.</span><span class="n">unique</span><span class="p">(</span><span class="n">average_rating</span><span class="p">)),</span> <span class="n">c</span> <span class="o">=</span> <span class="s2">&quot;orange&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>Due to the volume of data, I've made each point rather small so that we can better distinguish between the different data points. As expected, there are a lot of points concentrated on ratings that are whole numbers (1.0, 2.0, 3.0, 4.0, 5.0). This is likely because not every professor has multiple reviews and even the ones who do may have just a few reviews that are all of the same rating. However, despite the volume of data points, we can see that there seems to be a large density of points around the 5.0 rating and they seem to be skewed towards high GPA. Furthermore, the line of best fit seems to show that there is some positive relationship between the two measures. Let's calculate the R squared value to be sure.</p>

</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[210]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="kn">import</span> <span class="nn">statsmodels.formula.api</span> <span class="k">as</span> <span class="nn">smf</span>
<span class="n">res</span> <span class="o">=</span> <span class="n">smf</span><span class="o">.</span><span class="n">ols</span><span class="p">(</span><span class="n">formula</span><span class="o">=</span><span class="s2">&quot;average_rating ~ average_gpa&quot;</span><span class="p">,</span> <span class="n">data</span><span class="o">=</span><span class="n">professor_df</span><span class="p">)</span><span class="o">.</span><span class="n">fit</span><span class="p">()</span>
<span class="nb">print</span><span class="p">(</span><span class="s1">&#39;R squared: </span><span class="si">{}</span><span class="s1">&#39;</span><span class="o">.</span><span class="n">format</span><span class="p">(</span><span class="n">res</span><span class="o">.</span><span class="n">rsquared</span><span class="p">))</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>R squared: 0.15051243926885027
</pre>
</div>
</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>While an R squared value of 0.15 is not huge, it does seem appropriate given what we are measuring. There are a lot of factors that students take into consideration when rating a professor, such as how organized the class was, the professor's lecture style, how good the TA's were, etc. Furthermore, even if a student receives a low grade, it could be the case that they received that grade just because the class was difficult, and it had nothing to do with the quality of the professor. When  you consider the multitude of factors that influence the reviews students give, anything more than a modest relationship between the professor's rating and their average GPA would seem suspicious.</p>

</div>
</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h1 id="Another-Approach">Another Approach<a class="anchor-link" href="#Another-Approach">&#182;</a></h1>
</div>
</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>There may be a better, more direct way to go about measuring this relationship. On PlanetTerp, when you leave a review, there is an option to leave what grade you are expecting in the class. Instead of just measuring the average GPA of a professor across all the courses that he/she teaches, we could instead look at the individual reviews for each professor and see if there is a relationship between the grade that the reviewer is expecting to get and the rating they give the professor.</p>
<p>In the code below, I've marked down the grades as A, B, C, D, F, Pass (P), Withdrawn (W), and Not Reported (NR). The expectation is that those who received high grades (A's and B's) are likely going to leave higher ratings than those who recieved low grades. We also expect that people who withdrew from the class, passed the class (which was likely a lot of people during the COVID semesters), or simply didn't report the grade they got will give lower ratings to the professors.</p>
<p>This next block of code takes a long time to run, so you might want to go for a walk or put on a TV show if you are going to try and run this snippet yourself.</p>

</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[211]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">grades</span> <span class="o">=</span> <span class="p">{</span>
    <span class="s2">&quot;A&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;1&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">},</span> 
    <span class="s2">&quot;B&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;1&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">},</span> 
    <span class="s2">&quot;C&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;1&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">},</span> 
    <span class="s2">&quot;D&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;1&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">},</span>
    <span class="s2">&quot;F&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;1&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">},</span>
    <span class="s2">&quot;P&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;1&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">},</span>
    <span class="s2">&quot;W&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;1&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">},</span>
    <span class="s2">&quot;NR&quot;</span><span class="p">:</span> <span class="p">{</span><span class="s2">&quot;1&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">:</span> <span class="mi">0</span><span class="p">}</span>
<span class="p">}</span>
<span class="n">g</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;A&quot;</span><span class="p">,</span> <span class="s2">&quot;B&quot;</span><span class="p">,</span> <span class="s2">&quot;C&quot;</span><span class="p">,</span> <span class="s2">&quot;D&quot;</span><span class="p">,</span> <span class="s2">&quot;F&quot;</span><span class="p">,</span> <span class="s2">&quot;P&quot;</span><span class="p">,</span> <span class="s2">&quot;W&quot;</span><span class="p">]</span>
<span class="k">for</span> <span class="n">idx</span><span class="p">,</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">professor_df</span><span class="o">.</span><span class="n">iterrows</span><span class="p">():</span>
    <span class="c1"># print(idx)</span>
    <span class="n">reviews</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;https://api.planetterp.com/v1/professor?name=</span><span class="si">{</span><span class="n">row</span><span class="p">[</span><span class="s1">&#39;name&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&amp;reviews=true&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">json</span><span class="p">()</span>
    <span class="k">if</span> <span class="n">reviews</span> <span class="ow">is</span> <span class="kc">None</span> <span class="ow">or</span> <span class="s2">&quot;reviews&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">reviews</span><span class="p">:</span>
        <span class="c1"># print(reviews)</span>
        <span class="k">continue</span>
    <span class="n">reviews</span> <span class="o">=</span> <span class="n">reviews</span><span class="p">[</span><span class="s2">&quot;reviews&quot;</span><span class="p">]</span>
    <span class="k">for</span> <span class="n">rev</span> <span class="ow">in</span> <span class="n">reviews</span><span class="p">:</span>
        <span class="k">if</span> <span class="n">rev</span><span class="p">[</span><span class="s2">&quot;expected_grade&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span> <span class="ow">or</span> <span class="n">rev</span><span class="p">[</span><span class="s2">&quot;expected_grade&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
            <span class="c1"># print(rev[&quot;course&quot;])</span>
            <span class="n">grades</span><span class="p">[</span><span class="s2">&quot;NR&quot;</span><span class="p">][</span><span class="nb">str</span><span class="p">(</span><span class="n">rev</span><span class="p">[</span><span class="s2">&quot;rating&quot;</span><span class="p">])]</span> <span class="o">+=</span> <span class="mi">1</span>
            <span class="k">continue</span>
        <span class="n">grade</span> <span class="o">=</span> <span class="n">rev</span><span class="p">[</span><span class="s2">&quot;expected_grade&quot;</span><span class="p">][</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">upper</span><span class="p">()</span>
        <span class="k">if</span> <span class="n">grade</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">g</span><span class="p">:</span>
            <span class="c1"># print(f&quot;Continuing, {grade}&quot;)</span>
            <span class="k">continue</span>
        <span class="c1"># print(grade)</span>
        <span class="n">grades</span><span class="p">[</span><span class="n">grade</span><span class="p">][</span><span class="nb">str</span><span class="p">(</span><span class="n">rev</span><span class="p">[</span><span class="s2">&quot;rating&quot;</span><span class="p">])]</span> <span class="o">+=</span> <span class="mi">1</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>{&#39;A&#39;: {&#39;1&#39;: 432, &#39;2&#39;: 391, &#39;3&#39;: 643, &#39;4&#39;: 1457, &#39;5&#39;: 4294}, &#39;B&#39;: {&#39;1&#39;: 463, &#39;2&#39;: 369, &#39;3&#39;: 455, &#39;4&#39;: 562, &#39;5&#39;: 619}, &#39;C&#39;: {&#39;1&#39;: 256, &#39;2&#39;: 124, &#39;3&#39;: 82, &#39;4&#39;: 82, &#39;5&#39;: 51}, &#39;D&#39;: {&#39;1&#39;: 42, &#39;2&#39;: 14, &#39;3&#39;: 7, &#39;4&#39;: 5, &#39;5&#39;: 0}, &#39;F&#39;: {&#39;1&#39;: 31, &#39;2&#39;: 1, &#39;3&#39;: 1, &#39;4&#39;: 2, &#39;5&#39;: 4}, &#39;P&#39;: {&#39;1&#39;: 22, &#39;2&#39;: 11, &#39;3&#39;: 9, &#39;4&#39;: 6, &#39;5&#39;: 9}, &#39;W&#39;: {&#39;1&#39;: 31, &#39;2&#39;: 9, &#39;3&#39;: 2, &#39;4&#39;: 0, &#39;5&#39;: 0}, &#39;NR&#39;: {&#39;1&#39;: 815, &#39;2&#39;: 361, &#39;3&#39;: 332, &#39;4&#39;: 424, &#39;5&#39;: 824}}
</pre>
</div>
</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[212]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">data</span> <span class="o">=</span> <span class="p">[</span><span class="n">np</span><span class="o">.</span><span class="n">array</span><span class="p">(</span><span class="nb">list</span><span class="p">(</span><span class="n">d</span><span class="o">.</span><span class="n">values</span><span class="p">()))</span> <span class="k">for</span> <span class="n">d</span> <span class="ow">in</span> <span class="n">grades</span><span class="o">.</span><span class="n">values</span><span class="p">()]</span>
<span class="kn">import</span> <span class="nn">seaborn</span> <span class="k">as</span> <span class="nn">sb</span>
<span class="n">sb</span><span class="o">.</span><span class="n">heatmap</span><span class="p">(</span><span class="n">data</span><span class="p">,</span> <span class="n">xticklabels</span><span class="o">=</span><span class="s2">&quot;12345&quot;</span><span class="p">,</span> <span class="n">yticklabels</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;A&quot;</span><span class="p">,</span> <span class="s2">&quot;B&quot;</span><span class="p">,</span> <span class="s2">&quot;C&quot;</span><span class="p">,</span> <span class="s2">&quot;D&quot;</span><span class="p">,</span> <span class="s2">&quot;F&quot;</span><span class="p">,</span> <span class="s2">&quot;P&quot;</span><span class="p">,</span> <span class="s2">&quot;W&quot;</span><span class="p">,</span> <span class="s2">&quot;NR&quot;</span><span class="p">],</span> <span class="n">cmap</span><span class="o">=</span><span class="s2">&quot;Blues&quot;</span><span class="p">,</span> <span class="n">annot</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">fmt</span><span class="o">=</span><span class="s2">&quot;g&quot;</span><span class="p">);</span>
<span class="n">plt</span><span class="o">.</span><span class="n">xlabel</span><span class="p">(</span><span class="s2">&quot;Rating&quot;</span><span class="p">)</span>
<span class="n">plt</span><span class="o">.</span><span class="n">ylabel</span><span class="p">(</span><span class="s2">&quot;Grades&quot;</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[212]:</div>




<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain">
<pre>Text(69.0, 0.5, &#39;Grades&#39;)</pre>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>Wow. That certainly tells us something about the kinds of people who are leaving reviews on PlanetTerp. It's not even a contest. People who gave their professor 5-star ratings and also got A's in the class make up the grand majority of the reviews on the site. The group that comes in second place (people who got A's and left 4-star reviews) has less than half the number of people in this majority group. All other groups look absolutely tiny by comparison, as evidenced by the fact that they are all colored a very pale blue.</p>
<p>It is worth noting that all of the trends that we anticipated seem to be born out in this heat map. If we look at each of the different grade categories, we can see that people who got A's are overwhelmingly more likely to leave high reviews. The people who got B's, on the other hand, seem to have a more mixed relationship with a pretty even spread among the different ratings. People who got C's or lower were skewed in the opposite direction as those who got A's, with more people leaving low ratings. This is also true of those who passed or withdrew from the class.</p>
<p>It is also interesting to observe that there doesn't seem to be a clear relationship between not reporting one's grade and the rating. In the group of people who didn't report their grades, we see that about the same number of people of people left 1-star and 5-star ratings, with the rest pretty evenly spread among 2 to 4-star ratings.</p>
<p>You might find the pie charts below to be helpful in seeing these proportions among the different grade categories more clearly.</p>

</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[213]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">get_title</span><span class="p">(</span><span class="n">grade</span><span class="p">):</span>
    <span class="n">switcher</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;A&quot;</span><span class="p">:</span> <span class="s2">&quot;those who got A&#39;s&quot;</span><span class="p">,</span>
        <span class="s2">&quot;B&quot;</span><span class="p">:</span> <span class="s2">&quot;those who got B&#39;s&quot;</span><span class="p">,</span>
        <span class="s2">&quot;C&quot;</span><span class="p">:</span> <span class="s2">&quot;those who got C&#39;s&quot;</span><span class="p">,</span>
        <span class="s2">&quot;D&quot;</span><span class="p">:</span> <span class="s2">&quot;those who got D&#39;s&quot;</span><span class="p">,</span>
        <span class="s2">&quot;F&quot;</span><span class="p">:</span> <span class="s2">&quot;those who got F&#39;s&quot;</span><span class="p">,</span>
        <span class="s2">&quot;P&quot;</span><span class="p">:</span> <span class="s2">&quot;those who passed&quot;</span><span class="p">,</span>
        <span class="s2">&quot;W&quot;</span><span class="p">:</span> <span class="s2">&quot;those who withdrew&quot;</span><span class="p">,</span>
        <span class="s2">&quot;NR&quot;</span><span class="p">:</span> <span class="s2">&quot;those who didn&#39;t report their grade&quot;</span>
    <span class="p">}</span>
    <span class="k">return</span> <span class="n">switcher</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">grade</span><span class="p">)</span>
        
<span class="k">for</span> <span class="n">grade</span> <span class="ow">in</span> <span class="n">grades</span><span class="o">.</span><span class="n">keys</span><span class="p">():</span>
    <span class="n">title</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;Ratings left by </span><span class="si">{</span><span class="n">get_title</span><span class="p">(</span><span class="n">grade</span><span class="p">)</span><span class="si">}</span><span class="s2">&quot;</span>
    <span class="n">ratings</span> <span class="o">=</span> <span class="n">grades</span><span class="p">[</span><span class="n">grade</span><span class="p">]</span>
    <span class="n">rate_vals</span> <span class="o">=</span> <span class="p">[]</span>
    <span class="k">for</span> <span class="n">rating</span> <span class="ow">in</span> <span class="n">ratings</span><span class="o">.</span><span class="n">values</span><span class="p">():</span>
        <span class="n">rate_vals</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">rating</span><span class="p">)</span>
    <span class="n">labels</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;1&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">]</span>
    <span class="n">plt</span><span class="o">.</span><span class="n">pie</span><span class="p">(</span><span class="n">rate_vals</span><span class="p">,</span><span class="n">labels</span><span class="o">=</span><span class="n">labels</span><span class="p">,</span> <span class="n">autopct</span><span class="o">=</span><span class="s1">&#39;</span><span class="si">%1.1f%%</span><span class="s1">&#39;</span><span class="p">)</span>
    <span class="n">plt</span><span class="o">.</span><span class="n">title</span><span class="p">(</span><span class="n">title</span><span class="p">)</span>
    <span class="n">plt</span><span class="o">.</span><span class="n">show</span><span class="p">()</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>




<div class="jp-RenderedImage jp-OutputArea-output ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h1 id="A-new-measure?">A new measure?<a class="anchor-link" href="#A-new-measure?">&#182;</a></h1>
</div>
</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>Given our analysis so far, it seems fair to conclude that people who leave reviews on PlanetTerp are more likely to be people who received high grades in the courses they are reviewing. This presents a problem for those who are relying on PlanetTerp reviews and rating data to determine the quality of a professor, as these ratings might be biased towards professors who simply teach easy classes or grade easily. In this last part of the analysis, let's try and see if we can devise a way to measure the quality of a professor that doesn't suffer from the issues we face with the current information. I think that it's fair to say that if a student receives a high grade in a class, but rates the professor very low, then that indicates that the professor might not be very good. Similarly, if a student receives a low grade, but still rates the professor very highly, that would be a strong indication that the professor is very good. Obviously, it's not perfect. For example, some professors might still be very bad, but have cool personalities that cause students to still leave high ratings and vice versa. However, analyzing the review data in this way might yield some interesting results.</p>
<p>I'm going to only create this score for professors that have more than 20 ratings, as it likely wouldn't be very meaningful otherwise.</p>

</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[214]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">get_number_ratings</span><span class="p">(</span><span class="n">prof_df</span><span class="p">):</span>
    <span class="n">ratings_count</span> <span class="o">=</span> <span class="p">[]</span>
    <span class="k">for</span> <span class="n">idx</span><span class="p">,</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">prof_df</span><span class="o">.</span><span class="n">iterrows</span><span class="p">():</span>
        <span class="nb">print</span><span class="p">(</span><span class="n">idx</span><span class="p">)</span>
        <span class="n">reviews</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;https://api.planetterp.com/v1/professor?name=</span><span class="si">{</span><span class="n">row</span><span class="p">[</span><span class="s1">&#39;name&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&amp;reviews=true&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">json</span><span class="p">()</span>
        <span class="k">if</span> <span class="n">reviews</span> <span class="ow">is</span> <span class="kc">None</span> <span class="ow">or</span> <span class="s2">&quot;reviews&quot;</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">reviews</span><span class="p">:</span>
            <span class="n">ratings_count</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">float</span><span class="p">(</span><span class="s2">&quot;NaN&quot;</span><span class="p">))</span>
            <span class="k">continue</span>
        <span class="n">reviews</span> <span class="o">=</span> <span class="n">reviews</span><span class="p">[</span><span class="s2">&quot;reviews&quot;</span><span class="p">]</span>
        <span class="n">ratings_count</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">reviews</span><span class="p">))</span>
    <span class="k">return</span> <span class="n">ratings_count</span>

<span class="n">num_ratings</span> <span class="o">=</span> <span class="n">get_number_ratings</span><span class="p">(</span><span class="n">professor_df</span><span class="p">)</span>
<span class="n">professor_df</span><span class="p">[</span><span class="s2">&quot;num_ratings&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">num_ratings</span>
<span class="n">professor_df</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>1
2
4
6
8
10
15
19
27
42
45
47
53
58
61
64
68
74
76
79
92
97
104
105
113
115
120
124
129
132
136
138
139
140
146
173
176
178
181
183
184
187
194
198
200
205
206
214
215
216
223
224
227
229
236
240
241
242
245
247
249
251
252
276
279
282
291
301
305
307
319
329
331
334
341
344
349
350
351
357
362
365
368
369
371
372
376
377
378
381
399
413
417
426
428
432
433
438
453
465
467
472
478
482
485
489
491
492
495
503
504
506
511
512
518
525
529
536
537
550
551
561
562
566
570
592
598
599
602
609
611
622
630
634
641
642
643
647
679
685
691
693
694
698
703
724
728
731
732
739
741
752
757
760
768
769
773
778
783
795
802
803
804
807
809
814
828
832
833
842
848
849
850
872
873
890
892
894
902
914
915
916
917
922
931
932
934
942
960
961
967
968
988
989
998
2
3
5
11
24
25
26
31
33
35
36
37
38
40
42
45
46
49
56
63
70
71
76
77
79
83
88
90
102
105
110
111
112
114
116
125
128
129
140
142
151
155
156
159
168
176
182
183
186
201
203
210
213
214
218
221
224
232
234
248
252
256
259
263
265
285
289
295
296
301
307
308
309
310
322
325
332
336
340
343
374
398
405
407
408
416
424
425
428
442
444
448
457
462
476
490
501
519
531
534
539
542
543
548
555
566
569
578
579
581
587
590
597
600
607
609
618
621
625
631
632
639
643
648
649
663
665
674
681
684
686
691
696
703
715
717
720
722
726
732
733
736
740
742
744
746
753
755
759
768
777
781
784
790
791
797
806
807
830
831
832
846
847
853
855
859
863
865
875
878
880
894
899
902
904
907
908
914
918
919
924
930
934
936
938
946
951
955
961
964
967
979
985
986
993
6
10
11
12
17
21
31
37
47
51
52
58
59
63
67
74
78
98
111
121
126
127
128
132
137
141
148
152
171
176
185
186
195
196
197
200
206
209
218
220
226
229
236
239
247
248
257
264
286
287
288
289
295
297
301
306
319
326
329
342
345
356
359
363
366
369
373
374
383
388
389
395
398
406
409
411
413
421
423
431
437
438
440
446
452
454
458
465
467
471
472
474
487
498
501
505
508
509
513
517
518
520
521
523
524
526
527
535
544
546
548
551
561
565
566
575
579
583
589
602
606
609
610
614
617
620
622
623
627
631
632
636
638
642
659
677
694
696
698
699
701
705
706
708
709
713
716
717
721
722
725
728
731
733
737
751
752
754
757
759
762
764
768
778
780
781
783
788
800
801
803
804
810
820
827
836
838
845
847
849
859
860
863
864
868
870
874
883
886
887
889
891
893
896
903
909
921
926
933
935
939
940
943
944
947
948
957
958
962
966
967
974
976
977
978
980
986
992
997
13
15
19
21
26
28
32
33
42
51
55
59
62
65
68
70
73
79
84
88
91
92
103
105
123
132
137
150
152
154
162
167
169
171
179
183
184
186
190
192
193
195
196
197
198
200
203
209
214
221
237
244
245
254
256
277
280
281
285
290
303
306
311
317
320
323
324
327
329
347
349
355
358
360
365
377
379
390
397
399
406
407
408
409
412
425
430
438
441
447
449
469
477
479
483
484
486
487
489
490
493
494
495
503
516
521
531
538
540
543
544
545
546
548
555
558
559
563
571
573
575
578
579
580
584
592
595
597
604
609
614
617
624
630
631
636
639
641
642
643
647
648
650
661
664
666
668
670
672
683
687
689
694
698
708
715
717
721
722
725
727
734
746
751
756
762
765
768
770
773
776
779
787
808
813
818
821
823
824
825
826
830
831
833
852
853
866
870
873
880
882
888
896
897
901
906
909
910
911
914
921
923
928
933
943
947
949
951
952
954
959
961
962
964
979
981
985
990
9
10
14
20
21
25
27
29
30
33
35
40
41
42
66
67
78
79
80
85
92
97
98
103
113
130
131
134
138
141
147
173
178
181
184
189
198
205
206
214
216
219
221
225
232
235
237
239
240
241
245
246
251
254
256
267
277
278
282
284
286
293
296
298
301
302
305
310
326
334
338
339
345
347
348
351
352
360
364
367
368
377
379
385
394
400
401
408
409
415
417
418
429
434
437
439
443
450
452
453
464
465
467
468
471
481
484
487
492
496
497
498
503
504
506
507
510
512
517
530
531
532
536
538
539
558
560
561
562
565
578
597
613
617
626
640
641
646
652
656
659
660
661
664
666
690
712
713
715
724
726
738
746
747
751
753
756
768
784
786
788
793
796
799
802
803
804
805
813
814
817
820
822
829
836
838
843
850
851
854
857
860
862
863
867
874
875
876
877
882
884
885
888
890
892
900
907
914
916
934
938
945
946
950
956
960
961
966
967
971
976
982
987
996
999
1
10
12
17
22
24
25
32
35
38
46
49
50
52
62
67
74
77
78
80
84
89
91
101
103
107
117
120
121
130
131
132
137
140
142
143
144
159
168
169
178
183
186
200
201
202
204
208
211
220
224
231
233
234
235
236
243
245
250
251
257
258
259
263
264
267
269
275
302
310
314
320
323
327
329
330
331
335
338
345
354
359
360
363
365
371
375
377
380
381
383
384
385
386
391
394
411
414
416
418
423
424
426
428
434
437
443
447
449
450
452
455
459
469
477
487
491
496
497
505
506
513
524
529
531
546
547
560
569
571
581
592
616
620
631
632
645
646
651
652
658
668
669
675
676
679
680
681
682
692
697
701
710
712
735
743
745
749
754
755
756
768
769
776
777
779
784
785
788
791
801
807
813
817
820
821
829
831
832
836
844
846
855
869
874
876
881
888
898
909
913
934
935
938
941
944
945
946
956
958
970
972
980
994
995
999
2
5
20
23
28
30
31
46
51
52
53
54
62
66
68
69
71
77
79
81
83
84
86
91
103
105
106
109
110
115
129
132
137
140
155
161
173
176
178
185
190
200
205
207
209
213
219
236
238
239
241
242
243
248
249
253
262
266
270
271
274
276
288
290
298
301
307
308
309
311
313
314
315
324
330
331
332
336
337
345
355
359
364
370
375
376
378
386
393
403
417
419
424
425
430
450
462
476
479
485
490
495
497
504
521
525
533
537
541
551
553
557
564
565
583
588
593
604
607
610
611
629
631
634
635
636
638
645
649
657
661
663
668
677
678
683
699
700
701
704
707
709
715
721
723
729
740
764
775
788
789
790
795
804
815
818
820
822
828
830
832
834
835
837
838
842
856
859
860
871
875
878
884
890
899
904
910
912
913
914
916
917
921
928
940
944
949
950
958
962
964
965
980
990
992
996
999
8
10
14
17
21
23
26
35
46
50
59
65
71
75
79
80
82
91
92
94
101
104
109
116
122
123
126
128
133
136
137
142
154
155
157
158
164
175
179
193
194
205
208
212
225
227
232
235
236
237
241
242
257
258
269
272
277
278
279
281
283
284
286
296
316
317
319
321
322
330
335
340
342
345
348
352
369
371
373
377
381
387
391
392
395
396
401
403
404
410
411
413
420
424
428
434
446
458
466
475
478
483
494
500
502
504
505
509
510
511
512
515
520
522
526
528
532
536
537
541
543
545
546
550
551
552
557
579
585
588
590
596
597
599
600
602
609
611
615
624
625
628
631
640
646
647
652
664
678
680
683
687
691
694
699
702
707
712
714
716
718
722
746
752
758
759
768
776
778
779
784
799
804
809
819
821
822
827
832
836
842
846
847
850
853
861
864
870
878
885
893
896
907
915
917
930
938
941
953
955
977
978
979
6
16
18
19
21
23
28
36
38
40
43
50
72
80
83
85
91
97
98
99
100
101
102
103
104
107
115
118
123
125
132
133
136
144
151
153
157
158
162
165
166
168
169
171
174
175
177
182
183
186
189
192
193
200
203
216
218
222
225
226
231
232
234
236
248
256
261
262
264
267
281
282
283
284
285
286
287
297
300
301
304
308
310
313
315
316
323
325
327
331
332
344
346
347
349
352
354
355
360
370
371
373
374
375
376
386
388
390
394
395
400
401
402
411
412
413
421
426
430
431
435
439
445
456
459
467
476
479
481
482
488
489
492
494
495
496
501
507
511
519
521
526
530
531
532
536
538
540
543
546
553
558
560
579
582
585
586
590
592
595
596
598
599
622
632
634
646
649
650
654
655
662
666
669
673
675
686
689
691
694
696
697
698
700
702
705
707
708
709
711
712
714
715
718
722
725
729
730
735
737
742
748
754
763
764
767
768
774
776
777
781
782
783
784
787
790
792
799
804
808
812
824
825
829
835
840
841
853
856
860
863
873
874
878
885
886
892
907
909
910
914
919
925
926
929
936
937
939
943
945
953
957
964
967
972
976
979
983
994
998
1
9
10
13
14
18
22
30
31
34
39
42
43
50
51
57
59
65
67
70
71
81
83
85
92
94
101
107
113
128
133
139
142
143
144
146
150
151
152
155
159
160
161
162
163
169
172
178
180
183
189
191
192
197
198
199
205
208
216
222
228
230
234
238
242
248
253
254
255
257
260
261
265
268
279
282
284
285
288
298
302
303
304
323
325
328
331
332
335
343
344
346
347
353
355
361
374
381
392
402
404
407
410
415
420
421
438
446
450
452
453
457
460
463
470
473
480
488
494
499
501
502
512
513
522
527
529
532
533
534
538
544
551
557
563
566
578
579
584
587
595
605
606
610
612
619
620
631
635
639
644
647
649
656
657
660
668
693
696
706
717
724
728
729
733
734
737
751
752
772
780
785
786
788
789
798
809
810
813
815
816
818
822
823
831
834
836
837
839
841
847
848
851
859
864
868
870
871
879
890
891
892
907
911
916
917
924
930
939
941
948
949
950
955
960
961
962
965
966
975
981
983
988
990
991
994
5
7
8
13
21
27
31
42
61
65
67
72
74
79
82
84
96
98
110
116
118
119
120
121
122
127
135
142
146
149
155
157
160
170
178
179
180
182
184
187
190
192
193
194
195
196
199
201
202
203
205
206
218
223
226
239
249
256
261
265
267
272
274
279
281
290
292
301
302
303
304
305
308
312
321
326
332
333
334
338
346
347
349
350
358
360
366
379
380
391
393
396
398
400
405
410
411
415
424
426
441
445
449
451
457
462
464
468
471
475
482
483
509
511
513
514
519
521
534
537
538
540
544
564
566
568
571
577
579
586
587
589
592
596
603
605
607
616
617
630
632
639
640
641
642
643
647
648
649
650
654
655
663
668
672
676
677
684
685
688
689
690
691
694
696
699
700
706
707
710
712
727
728
729
730
739
743
746
763
766
767
772
777
784
788
791
797
801
802
803
806
811
816
823
824
825
827
834
835
837
851
853
875
878
887
888
893
922
927
928
933
934
935
951
954
958
966
967
969
977
987
992
998
999
4
20
29
32
34
</pre>
</div>
</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr">
<pre>&lt;ipython-input-214-ac9bd26733b1&gt;:14: SettingWithCopyWarning: 
A value is trying to be set on a copy of a slice from a DataFrame.
Try using .loc[row_indexer,col_indexer] = value instead

See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
  professor_df[&#34;num_ratings&#34;] = num_ratings
</pre>
</div>
</div>

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[214]:</div>



<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>slug</th>
      <th>type</th>
      <th>courses</th>
      <th>average_rating</th>
      <th>average_gpa</th>
      <th>num_ratings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1</th>
      <td>A Anthony</td>
      <td>anthony</td>
      <td>professor</td>
      <td>[AMST202, AMST203, AMST101]</td>
      <td>1.00</td>
      <td>2.48</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>2</th>
      <td>A Kruglanski</td>
      <td>kruglanski</td>
      <td>professor</td>
      <td>[PSYC743, PSYC748M, PSYC489H, PSYC489T, PSYC78...</td>
      <td>2.00</td>
      <td>3.49</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>A Sharma</td>
      <td>sharma_a</td>
      <td>professor</td>
      <td>[ASTR300]</td>
      <td>1.80</td>
      <td>2.82</td>
      <td>5.0</td>
    </tr>
    <tr>
      <th>6</th>
      <td>A.U. Shankar</td>
      <td>shankar_a.u.</td>
      <td>professor</td>
      <td>[CMSC412, CMSC414, CMSC712, CMSC216, CMSC798]</td>
      <td>2.10</td>
      <td>2.41</td>
      <td>20.0</td>
    </tr>
    <tr>
      <th>8</th>
      <td>Aaron Allen</td>
      <td>allen_aaron</td>
      <td>professor</td>
      <td>[HHUM205, HHUM206]</td>
      <td>5.00</td>
      <td>3.61</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>4</th>
      <td>Zhengguo Xiao</td>
      <td>xiao_zhengguo</td>
      <td>professor</td>
      <td>[ANSC460, ANSC214, GEMS296, ANSC212, GEMS297, ...</td>
      <td>4.00</td>
      <td>2.95</td>
      <td>1.0</td>
    </tr>
    <tr>
      <th>20</th>
      <td>Zhongchi Liu</td>
      <td>liu_zhongchi</td>
      <td>professor</td>
      <td>[BSCI378H, BSCI410, CBMG699Y, MOCB899]</td>
      <td>4.50</td>
      <td>3.37</td>
      <td>6.0</td>
    </tr>
    <tr>
      <th>29</th>
      <td>Zita Nunes</td>
      <td>nunes_zita</td>
      <td>professor</td>
      <td>[ENGL234, ENGL749B, ENGL448B, ENGL300, ENGL301...</td>
      <td>3.75</td>
      <td>2.75</td>
      <td>4.0</td>
    </tr>
    <tr>
      <th>32</th>
      <td>Zohreh Davoudi</td>
      <td>davoudi</td>
      <td>professor</td>
      <td>[PHYS604, PHYS411, PHYS624]</td>
      <td>2.50</td>
      <td>3.38</td>
      <td>2.0</td>
    </tr>
    <tr>
      <th>34</th>
      <td>Zsuzsa Daczo</td>
      <td>daczo</td>
      <td>professor</td>
      <td>[SOCY105, SOCY227, SOCY325, WMST325]</td>
      <td>4.50</td>
      <td>3.62</td>
      <td>4.0</td>
    </tr>
  </tbody>
</table>
<p>2363 rows × 7 columns</p>
</div>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[215]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">more_than_20</span> <span class="o">=</span> <span class="n">professor_df</span><span class="o">.</span><span class="n">loc</span><span class="p">[</span><span class="n">professor_df</span><span class="p">[</span><span class="s2">&quot;num_ratings&quot;</span><span class="p">]</span> <span class="o">&gt;=</span> <span class="mi">20</span><span class="p">]</span>
<span class="n">more_than_20</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[215]:</div>



<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>slug</th>
      <th>type</th>
      <th>courses</th>
      <th>average_rating</th>
      <th>average_gpa</th>
      <th>num_ratings</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>6</th>
      <td>A.U. Shankar</td>
      <td>shankar_a.u.</td>
      <td>professor</td>
      <td>[CMSC412, CMSC414, CMSC712, CMSC216, CMSC798]</td>
      <td>2.1000</td>
      <td>2.41</td>
      <td>20.0</td>
    </tr>
    <tr>
      <th>124</th>
      <td>Adrianos Papamarcou</td>
      <td>papamarcou</td>
      <td>professor</td>
      <td>[ENEE222, ENEE324, ENEE620, ENEE322, ENEE322H,...</td>
      <td>4.2400</td>
      <td>2.87</td>
      <td>25.0</td>
    </tr>
    <tr>
      <th>331</th>
      <td>Alice Mignerey</td>
      <td>mignerey</td>
      <td>professor</td>
      <td>[CHEM271, CHEM705, CHEM889A, CHEM403, CHEM131,...</td>
      <td>2.4444</td>
      <td>2.59</td>
      <td>36.0</td>
    </tr>
    <tr>
      <th>362</th>
      <td>Alka Gandhi</td>
      <td>gandhi</td>
      <td>professor</td>
      <td>[ECON312, ECON422, ECON321, ECON325]</td>
      <td>3.8788</td>
      <td>2.14</td>
      <td>33.0</td>
    </tr>
    <tr>
      <th>369</th>
      <td>Allan Yashinski</td>
      <td>yashinski</td>
      <td>professor</td>
      <td>[MATH240, MATH401, MATH406, MATH461, MATH141H,...</td>
      <td>4.6400</td>
      <td>2.72</td>
      <td>25.0</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>605</th>
      <td>Wesley Lawson</td>
      <td>lawson_wesley</td>
      <td>professor</td>
      <td>[ENEE131, ENEE132, ENEE200, ENEE205, ENEE381, ...</td>
      <td>3.7027</td>
      <td>3.10</td>
      <td>37.0</td>
    </tr>
    <tr>
      <th>649</th>
      <td>William Higgins</td>
      <td>higgins_william</td>
      <td>professor</td>
      <td>[BIOL608F, BSCI440, BSCI105, BSCI207, CLFS510,...</td>
      <td>3.4082</td>
      <td>2.66</td>
      <td>49.0</td>
    </tr>
    <tr>
      <th>676</th>
      <td>William McClenahan</td>
      <td>mcclenahan</td>
      <td>professor</td>
      <td>[BMGT380H, BMGT381, BMGT380, BUSI764, BMGT496,...</td>
      <td>4.1250</td>
      <td>3.10</td>
      <td>24.0</td>
    </tr>
    <tr>
      <th>727</th>
      <td>Wiseley Wong</td>
      <td>wong_wiseley</td>
      <td>professor</td>
      <td>[MATH141, MATH241H, MATH401, MATH241, MATH475,...</td>
      <td>4.8621</td>
      <td>2.49</td>
      <td>29.0</td>
    </tr>
    <tr>
      <th>729</th>
      <td>Wojciech Czaja</td>
      <td>czaja</td>
      <td>professor</td>
      <td>[MATH648I, MATH141H, MATH411, MATH648Q, MATH14...</td>
      <td>3.8929</td>
      <td>2.03</td>
      <td>28.0</td>
    </tr>
  </tbody>
</table>
<p>126 rows × 7 columns</p>
</div>
</div>

</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[216]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">get_grade_point</span><span class="p">(</span><span class="n">grade</span><span class="p">):</span>
    <span class="n">switcher</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;A&quot;</span><span class="p">:</span> <span class="mi">5</span><span class="p">,</span>
        <span class="s2">&quot;B&quot;</span><span class="p">:</span> <span class="mi">4</span><span class="p">,</span>
        <span class="s2">&quot;C&quot;</span><span class="p">:</span> <span class="mi">3</span><span class="p">,</span>
        <span class="s2">&quot;D&quot;</span><span class="p">:</span> <span class="mi">2</span><span class="p">,</span>
        <span class="s2">&quot;F&quot;</span><span class="p">:</span> <span class="mi">1</span><span class="p">,</span>
        <span class="s2">&quot;P&quot;</span><span class="p">:</span> <span class="mi">1</span><span class="p">,</span>
        <span class="s2">&quot;W&quot;</span><span class="p">:</span> <span class="mi">1</span>
    <span class="p">}</span>
    <span class="k">return</span> <span class="n">switcher</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">grade</span><span class="p">)</span>

<span class="n">g</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;A&quot;</span><span class="p">,</span> <span class="s2">&quot;B&quot;</span><span class="p">,</span> <span class="s2">&quot;C&quot;</span><span class="p">,</span> <span class="s2">&quot;D&quot;</span><span class="p">,</span> <span class="s2">&quot;F&quot;</span><span class="p">,</span> <span class="s2">&quot;P&quot;</span><span class="p">,</span> <span class="s2">&quot;W&quot;</span><span class="p">]</span>
<span class="n">scores</span> <span class="o">=</span> <span class="p">[]</span>
<span class="k">for</span> <span class="n">idx</span><span class="p">,</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">more_than_20</span><span class="o">.</span><span class="n">iterrows</span><span class="p">():</span>
    <span class="n">reviews</span> <span class="o">=</span> <span class="n">requests</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;https://api.planetterp.com/v1/professor?name=</span><span class="si">{</span><span class="n">row</span><span class="p">[</span><span class="s1">&#39;name&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&amp;reviews=true&quot;</span><span class="p">)</span><span class="o">.</span><span class="n">json</span><span class="p">()</span>
    <span class="n">reviews</span> <span class="o">=</span> <span class="n">reviews</span><span class="p">[</span><span class="s2">&quot;reviews&quot;</span><span class="p">]</span>
    <span class="n">cur_score</span> <span class="o">=</span> <span class="mi">0</span>
    <span class="k">for</span> <span class="n">rev</span> <span class="ow">in</span> <span class="n">reviews</span><span class="p">:</span>
        <span class="k">if</span> <span class="n">rev</span><span class="p">[</span><span class="s2">&quot;expected_grade&quot;</span><span class="p">]</span> <span class="o">==</span> <span class="s2">&quot;&quot;</span> <span class="ow">or</span> <span class="n">rev</span><span class="p">[</span><span class="s2">&quot;expected_grade&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
            <span class="k">continue</span>
        <span class="n">grade</span> <span class="o">=</span> <span class="n">rev</span><span class="p">[</span><span class="s2">&quot;expected_grade&quot;</span><span class="p">][</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">upper</span><span class="p">()</span>
        <span class="k">if</span> <span class="n">grade</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">g</span><span class="p">:</span>
            <span class="k">continue</span>
        <span class="c1"># print(grade)</span>
        <span class="n">rating</span> <span class="o">=</span> <span class="n">rev</span><span class="p">[</span><span class="s2">&quot;rating&quot;</span><span class="p">]</span>
        <span class="n">cur_score</span> <span class="o">+=</span> <span class="n">rating</span> <span class="o">-</span> <span class="n">get_grade_point</span><span class="p">(</span><span class="n">grade</span><span class="p">)</span> <span class="c1"># High rating, low grade -&gt; high score. Low rating, high grade -&gt; low score</span>
    <span class="n">scores</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">cur_score</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain">
<pre>[-35, -3, -27, -13, 6, -14, -24, 1, -16, -15, -34, -16, -6, -57, -8, -23, -30, -40, -49, -18, -65, -32, -51, 2, -3, -8, -1, -41, -10, -33, 3, -1, -62, -6, -10, -46, -41, -24, 0, -23, -22, -13, -8, -8, -29, -75, -26, -36, -9, -21, -7, 5, -31, -13, -36, -27, -7, -12, -16, -47, -8, -10, 21, -5, -21, -25, -4, -5, -42, -103, 0, -22, -29, -7, -15, -53, -11, -38, -24, -22, -28, -30, -34, 3, -21, -15, -8, 2, -99, -14, -7, 0, -13, -10, -28, -42, -25, -7, -39, -45, -5, -19, -17, -2, -13, -42, -27, -26, -5, -55, 7, 3, -1, -36, -20, -4, -13, -12, -43, -60, -24, -27, -40, -6, 0, -8]
</pre>
</div>
</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[217]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">more_than_20</span><span class="p">[</span><span class="s2">&quot;score&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">scores</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt"></div>


<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr">
<pre>&lt;ipython-input-217-76e9b4c5cf59&gt;:1: SettingWithCopyWarning: 
A value is trying to be set on a copy of a slice from a DataFrame.
Try using .loc[row_indexer,col_indexer] = value instead

See the caveats in the documentation: https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html#returning-a-view-versus-a-copy
  more_than_20[&#34;score&#34;] = scores
</pre>
</div>
</div>

</div>

</div>

</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell   ">
<div class="jp-Cell-inputWrapper">
<div class="jp-InputArea jp-Cell-inputArea">
<div class="jp-InputPrompt jp-InputArea-prompt">In&nbsp;[218]:</div>
<div class="jp-CodeMirrorEditor jp-Editor jp-InputArea-editor" data-type="inline">
     <div class="CodeMirror cm-s-jupyter">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">sorted_by_score</span> <span class="o">=</span> <span class="n">more_than_20</span><span class="o">.</span><span class="n">sort_values</span><span class="p">(</span><span class="n">by</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;score&quot;</span><span class="p">],</span><span class="n">ascending</span><span class="o">=</span><span class="kc">False</span><span class="p">)</span>
<span class="n">sorted_by_score</span><span class="o">.</span><span class="n">head</span><span class="p">(</span><span class="mi">40</span><span class="p">)</span>
</pre></div>

     </div>
</div>
</div>
</div>

<div class="jp-Cell-outputWrapper">


<div class="jp-OutputArea jp-Cell-outputArea">

<div class="jp-OutputArea-child">

    
    <div class="jp-OutputPrompt jp-OutputArea-prompt">Out[218]:</div>



<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html">
<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>name</th>
      <th>slug</th>
      <th>type</th>
      <th>courses</th>
      <th>average_rating</th>
      <th>average_gpa</th>
      <th>num_ratings</th>
      <th>score</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>386</th>
      <td>Justin Wyss-Gallifent</td>
      <td>wyss-gallifent</td>
      <td>professor</td>
      <td>[MATH206, MATH241, MATH410, MATH695, HONR219O,...</td>
      <td>4.9149</td>
      <td>3.29</td>
      <td>141.0</td>
      <td>21</td>
    </tr>
    <tr>
      <th>724</th>
      <td>Stefan Doboszczak</td>
      <td>doboszczak</td>
      <td>professor</td>
      <td>[AMSC460, CMSC460, MATH140, MATH410, MATH120, ...</td>
      <td>4.9500</td>
      <td>2.72</td>
      <td>20.0</td>
      <td>7</td>
    </tr>
    <tr>
      <th>369</th>
      <td>Allan Yashinski</td>
      <td>yashinski</td>
      <td>professor</td>
      <td>[MATH240, MATH401, MATH406, MATH461, MATH141H,...</td>
      <td>4.6400</td>
      <td>2.72</td>
      <td>25.0</td>
      <td>6</td>
    </tr>
    <tr>
      <th>467</th>
      <td>Jeffery Davis</td>
      <td>davis_jeffery</td>
      <td>professor</td>
      <td>[CHEM241, CHEM611, CHEM889D, CHEM648F, CHEM640...</td>
      <td>4.7407</td>
      <td>2.81</td>
      <td>27.0</td>
      <td>5</td>
    </tr>
    <tr>
      <th>352</th>
      <td>Michael Galczynski</td>
      <td>galczynski</td>
      <td>professor</td>
      <td>[ENES100, ENES100A, ENES113, ENES102, ENES102H...</td>
      <td>4.9677</td>
      <td>3.56</td>
      <td>31.0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>997</th>
      <td>Elizabeth Griffith</td>
      <td>griffith</td>
      <td>professor</td>
      <td>[CHEM135, CHEM482, CHEM177, CHEM271, CHEM131, ...</td>
      <td>4.4167</td>
      <td>2.57</td>
      <td>24.0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>823</th>
      <td>Steven Chadwick</td>
      <td>chadwick</td>
      <td>professor</td>
      <td>[MATH140, MATH140H, STAT410, MATH141, MATH401,...</td>
      <td>4.2000</td>
      <td>2.57</td>
      <td>20.0</td>
      <td>3</td>
    </tr>
    <tr>
      <th>434</th>
      <td>Michael Ross</td>
      <td>ross_michael</td>
      <td>professor</td>
      <td>[HIST289K, HIST455, HIST454, HIST619R, HIST131...</td>
      <td>4.4286</td>
      <td>3.14</td>
      <td>21.0</td>
      <td>2</td>
    </tr>
    <tr>
      <th>513</th>
      <td>David Straney</td>
      <td>straney</td>
      <td>professor</td>
      <td>[BSCI222, CPSP219L, BSCI348R, BSCI415]</td>
      <td>4.8621</td>
      <td>3.01</td>
      <td>29.0</td>
      <td>2</td>
    </tr>
    <tr>
      <th>803</th>
      <td>Anne Simon</td>
      <td>simon_anne</td>
      <td>professor</td>
      <td>[BSCI105C, BSCI105S, CBMG688B, CBMG688X, BSCI1...</td>
      <td>3.2245</td>
      <td>3.17</td>
      <td>49.0</td>
      <td>1</td>
    </tr>
    <tr>
      <th>503</th>
      <td>Gary Pertmer</td>
      <td>pertmer</td>
      <td>professor</td>
      <td>[ENES102, ENES102H, ENME489V, ENME472, ENME201...</td>
      <td>4.6000</td>
      <td>3.08</td>
      <td>20.0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>822</th>
      <td>Naveen Sarna</td>
      <td>sarna</td>
      <td>professor</td>
      <td>[ECON201, ECON317]</td>
      <td>4.4444</td>
      <td>2.73</td>
      <td>27.0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>207</th>
      <td>Lawrence Washington</td>
      <td>washington_lawrence</td>
      <td>professor</td>
      <td>[MATH456, MATH620, MATH406, MATH808N, MATH220,...</td>
      <td>4.8571</td>
      <td>3.12</td>
      <td>28.0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>727</th>
      <td>Wiseley Wong</td>
      <td>wong_wiseley</td>
      <td>professor</td>
      <td>[MATH141, MATH241H, MATH401, MATH241, MATH475,...</td>
      <td>4.8621</td>
      <td>2.49</td>
      <td>29.0</td>
      <td>0</td>
    </tr>
    <tr>
      <th>209</th>
      <td>Erich Studer-Ellis</td>
      <td>studer-ellis</td>
      <td>professor</td>
      <td>[BMGT230, BMGT230B]</td>
      <td>4.2973</td>
      <td>2.58</td>
      <td>37.0</td>
      <td>-1</td>
    </tr>
    <tr>
      <th>939</th>
      <td>Susan Mazzullo</td>
      <td>mazzullo</td>
      <td>professor</td>
      <td>[STAT100, STAT400, STAT430, STAT401, STAT440, ...</td>
      <td>4.8696</td>
      <td>2.98</td>
      <td>23.0</td>
      <td>-1</td>
    </tr>
    <tr>
      <th>706</th>
      <td>Dionisios Margetis</td>
      <td>margetis</td>
      <td>professor</td>
      <td>[MATH648M, MATH241, MATH424, MATH463, MATH858M...</td>
      <td>4.5581</td>
      <td>2.70</td>
      <td>43.0</td>
      <td>-1</td>
    </tr>
    <tr>
      <th>774</th>
      <td>Robert Bonenberger</td>
      <td>bonenberger</td>
      <td>professor</td>
      <td>[ENES102, ENES220]</td>
      <td>4.3810</td>
      <td>2.62</td>
      <td>21.0</td>
      <td>-2</td>
    </tr>
    <tr>
      <th>124</th>
      <td>Adrianos Papamarcou</td>
      <td>papamarcou</td>
      <td>professor</td>
      <td>[ENEE222, ENEE324, ENEE620, ENEE322, ENEE322H,...</td>
      <td>4.2400</td>
      <td>2.87</td>
      <td>25.0</td>
      <td>-3</td>
    </tr>
    <tr>
      <th>527</th>
      <td>David Yager</td>
      <td>yager</td>
      <td>professor</td>
      <td>[NACS728Q, PSYC301, HONR209O, PSYC407, PSYC606...</td>
      <td>3.8333</td>
      <td>2.48</td>
      <td>30.0</td>
      <td>-3</td>
    </tr>
    <tr>
      <th>84</th>
      <td>Terence Long</td>
      <td>long_terence</td>
      <td>professor</td>
      <td>[MATH213, MATH140, MATH113, MATH115, MATH246, ...</td>
      <td>4.4000</td>
      <td>2.73</td>
      <td>20.0</td>
      <td>-4</td>
    </tr>
    <tr>
      <th>756</th>
      <td>Kendall Williams</td>
      <td>williams_kendall</td>
      <td>professor</td>
      <td>[MATH241, MATH241H, MATH310, MATH274, MATH402,...</td>
      <td>2.8929</td>
      <td>2.47</td>
      <td>28.0</td>
      <td>-4</td>
    </tr>
    <tr>
      <th>496</th>
      <td>Kasso Okoudjou</td>
      <td>okoudjou</td>
      <td>professor</td>
      <td>[MATH141, MATH140, MATH630, MATH631, MATH858G,...</td>
      <td>3.8400</td>
      <td>2.36</td>
      <td>25.0</td>
      <td>-5</td>
    </tr>
    <tr>
      <th>829</th>
      <td>Kevin Calabro</td>
      <td>calabro</td>
      <td>professor</td>
      <td>[ENES100, ENES221, ENES100A, ENES232, ENES499,...</td>
      <td>4.2917</td>
      <td>2.80</td>
      <td>24.0</td>
      <td>-5</td>
    </tr>
    <tr>
      <th>711</th>
      <td>Richard King</td>
      <td>king_richard</td>
      <td>professor</td>
      <td>[MUSC205, MUSC230, HONR209Z, MUSC639H, MUSC320...</td>
      <td>4.4286</td>
      <td>3.08</td>
      <td>21.0</td>
      <td>-5</td>
    </tr>
    <tr>
      <th>50</th>
      <td>Ryan Curtis</td>
      <td>curtis</td>
      <td>professor</td>
      <td>[PSYC100, PSYC420, PSYC334, PSYC798B, HONR219E...</td>
      <td>4.1613</td>
      <td>2.74</td>
      <td>31.0</td>
      <td>-5</td>
    </tr>
    <tr>
      <th>416</th>
      <td>Bryan Eichhorn</td>
      <td>eichhorn</td>
      <td>professor</td>
      <td>[CHEM131, CHEM608B, CHEM602, CHEM401, CHEM271,...</td>
      <td>3.9231</td>
      <td>2.29</td>
      <td>26.0</td>
      <td>-6</td>
    </tr>
    <tr>
      <th>355</th>
      <td>Fawzi Emad</td>
      <td>emad_fawzi</td>
      <td>professor</td>
      <td>[CMSC122, CMSC131, CMSC132, CMSC131H, CMSC250]</td>
      <td>4.4086</td>
      <td>2.41</td>
      <td>93.0</td>
      <td>-6</td>
    </tr>
    <tr>
      <th>676</th>
      <td>William McClenahan</td>
      <td>mcclenahan</td>
      <td>professor</td>
      <td>[BMGT380H, BMGT381, BMGT380, BUSI764, BMGT496,...</td>
      <td>4.1250</td>
      <td>3.10</td>
      <td>24.0</td>
      <td>-6</td>
    </tr>
    <tr>
      <th>495</th>
      <td>Louisa Wu</td>
      <td>wu_louisa</td>
      <td>professor</td>
      <td>[BSCI378H, BSCI416, BSCI410, MOCB899, HLSC322,...</td>
      <td>4.3333</td>
      <td>3.69</td>
      <td>21.0</td>
      <td>-7</td>
    </tr>
    <tr>
      <th>804</th>
      <td>Nathan Manning</td>
      <td>manning_nathan</td>
      <td>professor</td>
      <td>[MATH220, MATH445, MATH140, MATH401, MATH140H,...</td>
      <td>3.4231</td>
      <td>2.01</td>
      <td>26.0</td>
      <td>-7</td>
    </tr>
    <tr>
      <th>411</th>
      <td>Progyan Basu</td>
      <td>basu</td>
      <td>professor</td>
      <td>[BMGT313, BMGT220, BMGT398C, BUAC743, BUSI610,...</td>
      <td>3.9697</td>
      <td>2.44</td>
      <td>66.0</td>
      <td>-7</td>
    </tr>
    <tr>
      <th>982</th>
      <td>John Pease</td>
      <td>pease</td>
      <td>professor</td>
      <td>[SOCY441, SOCY200, SOCY200H, SOCY699T, SOCY653...</td>
      <td>4.1500</td>
      <td>3.00</td>
      <td>20.0</td>
      <td>-7</td>
    </tr>
    <tr>
      <th>465</th>
      <td>Jeff Miller</td>
      <td>miller_jeff</td>
      <td>professor</td>
      <td>[BMGT110, BMGT289I, BMGT372, BMGT110S, BMGT466...</td>
      <td>4.1064</td>
      <td>2.90</td>
      <td>47.0</td>
      <td>-7</td>
    </tr>
    <tr>
      <th>403</th>
      <td>Michael Montague-Smith</td>
      <td>montague-smith</td>
      <td>professor</td>
      <td>[CHEM241, CHEM395, CHEM231, CPSP218L, CHEM399X...</td>
      <td>4.1081</td>
      <td>2.33</td>
      <td>37.0</td>
      <td>-8</td>
    </tr>
    <tr>
      <th>258</th>
      <td>Judd Nelson</td>
      <td>nelson_judd</td>
      <td>professor</td>
      <td>[BSCI105, ENTM788C, BSCI105M, TOXI609]</td>
      <td>4.2424</td>
      <td>2.83</td>
      <td>33.0</td>
      <td>-8</td>
    </tr>
    <tr>
      <th>25</th>
      <td>Ibrahim Ades</td>
      <td>ades_ibrahim</td>
      <td>professor</td>
      <td>[BSCI338P, BSCI433, BSCI330, BSCI338G, BSCI339Q]</td>
      <td>4.1892</td>
      <td>2.80</td>
      <td>37.0</td>
      <td>-8</td>
    </tr>
    <tr>
      <th>985</th>
      <td>Hugh Turner</td>
      <td>turner_hugh</td>
      <td>professor</td>
      <td>[BMGT198F, BMGT372, BMGT110F, BULM758G, BMGT37...</td>
      <td>4.4400</td>
      <td>3.35</td>
      <td>25.0</td>
      <td>-8</td>
    </tr>
    <tr>
      <th>729</th>
      <td>Wojciech Czaja</td>
      <td>czaja</td>
      <td>professor</td>
      <td>[MATH648I, MATH141H, MATH411, MATH648Q, MATH14...</td>
      <td>3.8929</td>
      <td>2.03</td>
      <td>28.0</td>
      <td>-8</td>
    </tr>
    <tr>
      <th>684</th>
      <td>Chandrasekhar Thamire</td>
      <td>thamire</td>
      <td>professor</td>
      <td>[ENES221, ENME371, ENME632, ENPM620, ENES232, ...</td>
      <td>4.2727</td>
      <td>2.93</td>
      <td>22.0</td>
      <td>-8</td>
    </tr>
  </tbody>
</table>
</div>
</div>

</div>

</div>

</div>

</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<p>Ok so it looks like my new measure might be a little bit too harsh, as the mean is -21. On the other hand, it has also reaffirmed to me that at the top of all things teaching at UMD is always Justin Wyss-Gallifent. His score is triple the next-highest score. Looking at the data in this table, it's really interesting to see where different teachers land. As a student who has taken classes with a number of these professors, I notice certain ones that appear lower than I would have thought, and others that appear higher than I would have thought.</p>

</div>
</div>
<div class="jp-Cell-inputWrapper"><div class="jp-InputPrompt jp-InputArea-prompt">
</div><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput " data-mime-type="text/markdown">
<h1 id="Conclusion">Conclusion<a class="anchor-link" href="#Conclusion">&#182;</a></h1><p>Students lead stressful lives, and trying to determine which professors will give the best learning experience is a very tricky task. Consulting different sources of data, such as ratings on PlanetTerp, is one approach to tackling this task. However, as we've seen through this analysis, there are problems with the kind of data that you see on PlanetTerp ratings (and likely with other similar review sites). It does seem to be the case that these sites are dominated by students who receive high marks in the courses they are reviewing, which could lead to biased data that paints an inaccurate picture of which professors will be best. However, it does still seem to be possible to harness the ratings data in a way that combats these biases.</p>
<p>For future research, I believe there is a lot of potential for using grade and rating data to help students. One possibility would be some way for students to see how well they are likely to do in future courses based on their past performance. A big issue that I've encountered as a student is knowing how difficult a courseload will likely be. For example, I might be planning out my schedule for next semester and go on the UMD subreddit to ask if my schedule is manageable. I may get wildly different answers. Moreover, because everyone has different levels of ability, what might be an unmanageable workload for me might be a cakewalk for someone on Reddit responding to my proposed schedule. One way you could combat this would be to have some sort of resource where each student would have their grades uploaded to an account. Then you would have some sort of machine-learning model that predicts future performance based on past performance. So as a CMSC student, if I got an A in CMSC131, a B in CMSC132, and a B- in CMSC216, the model would be able to take in that data and predict how well I'm likely to do in CMSC330 and CMSC351 based on the grades of upperclassmen who also got those same grades in CMSC 131, 132, and 216. This could help give students a better idea of how difficult certain courses and workloads will be. Currently, I don't believe this is possible since grade data would have to be associated with individual student accounts, and that sort of thing would only be available if students voluntarily give it up. But if these kinds of barriers could be overcome, I believe this kind of tool would be very helpful in helping students plan out their academic roadmap.</p>

</div>
</div>
</body>







</html>
