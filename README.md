<!DOCTYPE html>

<html lang="en">
<head><meta charset="utf-8"/>
<meta content="width=device-width, initial-scale=1.0" name="viewport"/>
<title>Assessment_solution</title><script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<style type="text/css">
    pre { line-height: 125%; }
td.linenos .normal { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
span.linenos { color: inherit; background-color: transparent; padding-left: 5px; padding-right: 5px; }
td.linenos .special { color: #000000; background-color: #ffffc0; padding-left: 5px; padding-right: 5px; }
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
.highlight .pm { color: var(--jp-mirror-editor-punctuation-color) } /* Punctuation.Marker */
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

/* tiny scrollbar */

.jp-scrollbar-tiny {
  scrollbar-color: rgba(var(--jp-scrollbar-thumb-color), 0.5) transparent;
  scrollbar-width: thin;
}

/* tiny scrollbar */

.jp-scrollbar-tiny::-webkit-scrollbar,
.jp-scrollbar-tiny::-webkit-scrollbar-corner {
  background-color: transparent;
  height: 4px;
  width: 4px;
}

.jp-scrollbar-tiny::-webkit-scrollbar-thumb {
  background: rgba(var(--jp-scrollbar-thumb-color), 0.5);
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:horizontal {
  border-left: 0 solid transparent;
  border-right: 0 solid transparent;
}

.jp-scrollbar-tiny::-webkit-scrollbar-track:vertical {
  border-top: 0 solid transparent;
  border-bottom: 0 solid transparent;
}

/*
 * Lumino
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

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-Widget {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
}

.lm-Widget.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.lm-AccordionPanel[data-orientation='horizontal'] > .lm-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-CommandPalette {
  display: flex;
  flex-direction: column;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-CommandPalette-search {
  flex: 0 0 auto;
}

.lm-CommandPalette-content {
  flex: 1 1 auto;
  margin: 0;
  padding: 0;
  min-height: 0;
  overflow: auto;
  list-style-type: none;
}

.lm-CommandPalette-header {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-CommandPalette-item {
  display: flex;
  flex-direction: row;
}

.lm-CommandPalette-itemIcon {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemContent {
  flex: 1 1 auto;
  overflow: hidden;
}

.lm-CommandPalette-itemShortcut {
  flex: 0 0 auto;
}

.lm-CommandPalette-itemLabel {
  overflow: hidden;
  white-space: nowrap;
  text-overflow: ellipsis;
}

.lm-close-icon {
  border: 1px solid transparent;
  background-color: transparent;
  position: absolute;
  z-index: 1;
  right: 3%;
  top: 0;
  bottom: 0;
  margin: auto;
  padding: 7px 0;
  display: none;
  vertical-align: middle;
  outline: 0;
  cursor: pointer;
}
.lm-close-icon:after {
  content: 'X';
  display: block;
  width: 15px;
  height: 15px;
  text-align: center;
  color: #000;
  font-weight: normal;
  font-size: 12px;
  cursor: pointer;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-DockPanel {
  z-index: 0;
}

.lm-DockPanel-widget {
  z-index: 0;
}

.lm-DockPanel-tabBar {
  z-index: 1;
}

.lm-DockPanel-handle {
  z-index: 2;
}

.lm-DockPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-DockPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-DockPanel-handle[data-orientation='horizontal'] {
  cursor: ew-resize;
}

.lm-DockPanel-handle[data-orientation='vertical'] {
  cursor: ns-resize;
}

.lm-DockPanel-handle[data-orientation='horizontal']:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-DockPanel-handle[data-orientation='vertical']:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

.lm-DockPanel-overlay {
  z-index: 3;
  box-sizing: border-box;
  pointer-events: none;
}

.lm-DockPanel-overlay.lm-mod-hidden {
  display: none !important;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

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

.lm-Menu-content {
  margin: 0;
  padding: 0;
  display: table;
  list-style-type: none;
}

.lm-Menu-item {
  display: table-row;
}

.lm-Menu-item.lm-mod-hidden,
.lm-Menu-item.lm-mod-collapsed {
  display: none !important;
}

.lm-Menu-itemIcon,
.lm-Menu-itemSubmenuIcon {
  display: table-cell;
  text-align: center;
}

.lm-Menu-itemLabel {
  display: table-cell;
  text-align: left;
}

.lm-Menu-itemShortcut {
  display: table-cell;
  text-align: right;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-MenuBar {
  outline: none;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-MenuBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: row;
  list-style-type: none;
}

.lm-MenuBar-item {
  box-sizing: border-box;
}

.lm-MenuBar-itemIcon,
.lm-MenuBar-itemLabel {
  display: inline-block;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-ScrollBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-ScrollBar[data-orientation='horizontal'] {
  flex-direction: row;
}

.lm-ScrollBar[data-orientation='vertical'] {
  flex-direction: column;
}

.lm-ScrollBar-button {
  box-sizing: border-box;
  flex: 0 0 auto;
}

.lm-ScrollBar-track {
  box-sizing: border-box;
  position: relative;
  overflow: hidden;
  flex: 1 1 auto;
}

.lm-ScrollBar-thumb {
  box-sizing: border-box;
  position: absolute;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-SplitPanel-child {
  z-index: 0;
}

.lm-SplitPanel-handle {
  z-index: 1;
}

.lm-SplitPanel-handle.lm-mod-hidden {
  display: none !important;
}

.lm-SplitPanel-handle:after {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  content: '';
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle {
  cursor: ew-resize;
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle {
  cursor: ns-resize;
}

.lm-SplitPanel[data-orientation='horizontal'] > .lm-SplitPanel-handle:after {
  left: 50%;
  min-width: 8px;
  transform: translateX(-50%);
}

.lm-SplitPanel[data-orientation='vertical'] > .lm-SplitPanel-handle:after {
  top: 50%;
  min-height: 8px;
  transform: translateY(-50%);
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabBar {
  display: flex;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.lm-TabBar[data-orientation='horizontal'] {
  flex-direction: row;
  align-items: flex-end;
}

.lm-TabBar[data-orientation='vertical'] {
  flex-direction: column;
  align-items: flex-end;
}

.lm-TabBar-content {
  margin: 0;
  padding: 0;
  display: flex;
  flex: 1 1 auto;
  list-style-type: none;
}

.lm-TabBar[data-orientation='horizontal'] > .lm-TabBar-content {
  flex-direction: row;
}

.lm-TabBar[data-orientation='vertical'] > .lm-TabBar-content {
  flex-direction: column;
}

.lm-TabBar-tab {
  display: flex;
  flex-direction: row;
  box-sizing: border-box;
  overflow: hidden;
  touch-action: none; /* Disable native Drag/Drop */
}

.lm-TabBar-tabIcon,
.lm-TabBar-tabCloseIcon {
  flex: 0 0 auto;
}

.lm-TabBar-tabLabel {
  flex: 1 1 auto;
  overflow: hidden;
  white-space: nowrap;
}

.lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
}

.lm-TabBar-tab.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar-addButton.lm-mod-hidden {
  display: none !important;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab {
  position: relative;
}

.lm-TabBar.lm-mod-dragging[data-orientation='horizontal'] .lm-TabBar-tab {
  left: 0;
  transition: left 150ms ease;
}

.lm-TabBar.lm-mod-dragging[data-orientation='vertical'] .lm-TabBar-tab {
  top: 0;
  transition: top 150ms ease;
}

.lm-TabBar.lm-mod-dragging .lm-TabBar-tab.lm-mod-dragging {
  transition: none;
}

.lm-TabBar-tabLabel .lm-TabBar-tabInput {
  user-select: all;
  width: 100%;
  box-sizing: border-box;
  background: inherit;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-TabPanel-tabBar {
  z-index: 1;
}

.lm-TabPanel-stackedPanel {
  z-index: 0;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapse {
  display: flex;
  flex-direction: column;
  align-items: stretch;
}

.jp-Collapse-header {
  padding: 1px 12px;
  background-color: var(--jp-layout-color1);
  border-bottom: solid var(--jp-border-width) var(--jp-border-color2);
  color: var(--jp-ui-font-color1);
  cursor: pointer;
  display: flex;
  align-items: center;
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  text-transform: uppercase;
  user-select: none;
}

.jp-Collapser-icon {
  height: 16px;
}

.jp-Collapse-header-collapsed .jp-Collapser-icon {
  transform: rotate(-90deg);
  margin: auto 0;
}

.jp-Collapser-title {
  line-height: 25px;
}

.jp-Collapse-contents {
  padding: 0 12px;
  background-color: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

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
  --jp-icon-add-above: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5MikiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik00Ljc1IDQuOTMwNjZINi42MjVWNi44MDU2NkM2LjYyNSA3LjAxMTkxIDYuNzkzNzUgNy4xODA2NiA3IDcuMTgwNjZDNy4yMDYyNSA3LjE4MDY2IDcuMzc1IDcuMDExOTEgNy4zNzUgNi44MDU2NlY0LjkzMDY2SDkuMjVDOS40NTYyNSA0LjkzMDY2IDkuNjI1IDQuNzYxOTEgOS42MjUgNC41NTU2NkM5LjYyNSA0LjM0OTQxIDkuNDU2MjUgNC4xODA2NiA5LjI1IDQuMTgwNjZINy4zNzVWMi4zMDU2NkM3LjM3NSAyLjA5OTQxIDcuMjA2MjUgMS45MzA2NiA3IDEuOTMwNjZDNi43OTM3NSAxLjkzMDY2IDYuNjI1IDIuMDk5NDEgNi42MjUgMi4zMDU2NlY0LjE4MDY2SDQuNzVDNC41NDM3NSA0LjE4MDY2IDQuMzc1IDQuMzQ5NDEgNC4zNzUgNC41NTU2NkM0LjM3NSA0Ljc2MTkxIDQuNTQzNzUgNC45MzA2NiA0Ljc1IDQuOTMwNjZaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC43Ii8+CjwvZz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTExLjUgOS41VjExLjVMMi41IDExLjVWOS41TDExLjUgOS41Wk0xMiA4QzEyLjU1MjMgOCAxMyA4LjQ0NzcyIDEzIDlWMTJDMTMgMTIuNTUyMyAxMi41NTIzIDEzIDEyIDEzTDIgMTNDMS40NDc3MiAxMyAxIDEyLjU1MjMgMSAxMlY5QzEgOC40NDc3MiAxLjQ0NzcxIDggMiA4TDEyIDhaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5MiI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KC0xIDAgMCAxIDEwIDEuNTU1NjYpIi8+CjwvY2xpcFBhdGg+CjwvZGVmcz4KPC9zdmc+Cg==);
  --jp-icon-add-below: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPGcgY2xpcC1wYXRoPSJ1cmwoI2NsaXAwXzEzN18xOTQ5OCkiPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGQ9Ik05LjI1IDEwLjA2OTNMNy4zNzUgMTAuMDY5M0w3LjM3NSA4LjE5NDM0QzcuMzc1IDcuOTg4MDkgNy4yMDYyNSA3LjgxOTM0IDcgNy44MTkzNEM2Ljc5Mzc1IDcuODE5MzQgNi42MjUgNy45ODgwOSA2LjYyNSA4LjE5NDM0TDYuNjI1IDEwLjA2OTNMNC43NSAxMC4wNjkzQzQuNTQzNzUgMTAuMDY5MyA0LjM3NSAxMC4yMzgxIDQuMzc1IDEwLjQ0NDNDNC4zNzUgMTAuNjUwNiA0LjU0Mzc1IDEwLjgxOTMgNC43NSAxMC44MTkzTDYuNjI1IDEwLjgxOTNMNi42MjUgMTIuNjk0M0M2LjYyNSAxMi45MDA2IDYuNzkzNzUgMTMuMDY5MyA3IDEzLjA2OTNDNy4yMDYyNSAxMy4wNjkzIDcuMzc1IDEyLjkwMDYgNy4zNzUgMTIuNjk0M0w3LjM3NSAxMC44MTkzTDkuMjUgMTAuODE5M0M5LjQ1NjI1IDEwLjgxOTMgOS42MjUgMTAuNjUwNiA5LjYyNSAxMC40NDQzQzkuNjI1IDEwLjIzODEgOS40NTYyNSAxMC4wNjkzIDkuMjUgMTAuMDY5M1oiIGZpbGw9IiM2MTYxNjEiIHN0cm9rZT0iIzYxNjE2MSIgc3Ryb2tlLXdpZHRoPSIwLjciLz4KPC9nPgo8cGF0aCBjbGFzcz0ianAtaWNvbjMiIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMi41IDUuNUwyLjUgMy41TDExLjUgMy41TDExLjUgNS41TDIuNSA1LjVaTTIgN0MxLjQ0NzcyIDcgMSA2LjU1MjI4IDEgNkwxIDNDMSAyLjQ0NzcyIDEuNDQ3NzIgMiAyIDJMMTIgMkMxMi41NTIzIDIgMTMgMi40NDc3MiAxMyAzTDEzIDZDMTMgNi41NTIyOSAxMi41NTIzIDcgMTIgN0wyIDdaIiBmaWxsPSIjNjE2MTYxIi8+CjxkZWZzPgo8Y2xpcFBhdGggaWQ9ImNsaXAwXzEzN18xOTQ5OCI+CjxyZWN0IGNsYXNzPSJqcC1pY29uMyIgd2lkdGg9IjYiIGhlaWdodD0iNiIgZmlsbD0id2hpdGUiIHRyYW5zZm9ybT0ibWF0cml4KDEgMS43NDg0NmUtMDcgMS43NDg0NmUtMDcgLTEgNCAxMy40NDQzKSIvPgo8L2NsaXBQYXRoPgo8L2RlZnM+Cjwvc3ZnPgo=);
  --jp-icon-add: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDEzaC02djZoLTJ2LTZINXYtMmg2VjVoMnY2aDZ2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bell: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE2IDE2IiB2ZXJzaW9uPSIxLjEiPgogICA8cGF0aCBjbGFzcz0ianAtaWNvbjIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzMzMzMzIgogICAgICBkPSJtOCAwLjI5Yy0xLjQgMC0yLjcgMC43My0zLjYgMS44LTEuMiAxLjUtMS40IDMuNC0xLjUgNS4yLTAuMTggMi4yLTAuNDQgNC0yLjMgNS4zbDAuMjggMS4zaDVjMC4wMjYgMC42NiAwLjMyIDEuMSAwLjcxIDEuNSAwLjg0IDAuNjEgMiAwLjYxIDIuOCAwIDAuNTItMC40IDAuNi0xIDAuNzEtMS41aDVsMC4yOC0xLjNjLTEuOS0wLjk3LTIuMi0zLjMtMi4zLTUuMy0wLjEzLTEuOC0wLjI2LTMuNy0xLjUtNS4yLTAuODUtMS0yLjItMS44LTMuNi0xLjh6bTAgMS40YzAuODggMCAxLjkgMC41NSAyLjUgMS4zIDAuODggMS4xIDEuMSAyLjcgMS4yIDQuNCAwLjEzIDEuNyAwLjIzIDMuNiAxLjMgNS4yaC0xMGMxLjEtMS42IDEuMi0zLjQgMS4zLTUuMiAwLjEzLTEuNyAwLjMtMy4zIDEuMi00LjQgMC41OS0wLjcyIDEuNi0xLjMgMi41LTEuM3ptLTAuNzQgMTJoMS41Yy0wLjAwMTUgMC4yOCAwLjAxNSAwLjc5LTAuNzQgMC43OS0wLjczIDAuMDAxNi0wLjcyLTAuNTMtMC43NC0wLjc5eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-bug-dot: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiPgogICAgICAgIDxwYXRoIGZpbGwtcnVsZT0iZXZlbm9kZCIgY2xpcC1ydWxlPSJldmVub2RkIiBkPSJNMTcuMTkgOEgyMFYxMEgxNy45MUMxNy45NiAxMC4zMyAxOCAxMC42NiAxOCAxMVYxMkgyMFYxNEgxOC41SDE4VjE0LjAyNzVDMTUuNzUgMTQuMjc2MiAxNCAxNi4xODM3IDE0IDE4LjVDMTQgMTkuMjA4IDE0LjE2MzUgMTkuODc3OSAxNC40NTQ5IDIwLjQ3MzlDMTMuNzA2MyAyMC44MTE3IDEyLjg3NTcgMjEgMTIgMjFDOS43OCAyMSA3Ljg1IDE5Ljc5IDYuODEgMThINFYxNkg2LjA5QzYuMDQgMTUuNjcgNiAxNS4zNCA2IDE1VjE0SDRWMTJINlYxMUM2IDEwLjY2IDYuMDQgMTAuMzMgNi4wOSAxMEg0VjhINi44MUM3LjI2IDcuMjIgNy44OCA2LjU1IDguNjIgNi4wNEw3IDQuNDFMOC40MSAzTDEwLjU5IDUuMTdDMTEuMDQgNS4wNiAxMS41MSA1IDEyIDVDMTIuNDkgNSAxMi45NiA1LjA2IDEzLjQyIDUuMTdMMTUuNTkgM0wxNyA0LjQxTDE1LjM3IDYuMDRDMTYuMTIgNi41NSAxNi43NCA3LjIyIDE3LjE5IDhaTTEwIDE2SDE0VjE0SDEwVjE2Wk0xMCAxMkgxNFYxMEgxMFYxMloiIGZpbGw9IiM2MTYxNjEiLz4KICAgICAgICA8cGF0aCBkPSJNMjIgMTguNUMyMiAyMC40MzMgMjAuNDMzIDIyIDE4LjUgMjJDMTYuNTY3IDIyIDE1IDIwLjQzMyAxNSAxOC41QzE1IDE2LjU2NyAxNi41NjcgMTUgMTguNSAxNUMyMC40MzMgMTUgMjIgMTYuNTY3IDIyIDE4LjVaIiBmaWxsPSIjNjE2MTYxIi8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-bug: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yMCA4aC0yLjgxYy0uNDUtLjc4LTEuMDctMS40NS0xLjgyLTEuOTZMMTcgNC40MSAxNS41OSAzbC0yLjE3IDIuMTdDMTIuOTYgNS4wNiAxMi40OSA1IDEyIDVjLS40OSAwLS45Ni4wNi0xLjQxLjE3TDguNDEgMyA3IDQuNDFsMS42MiAxLjYzQzcuODggNi41NSA3LjI2IDcuMjIgNi44MSA4SDR2MmgyLjA5Yy0uMDUuMzMtLjA5LjY2LS4wOSAxdjFINHYyaDJ2MWMwIC4zNC4wNC42Ny4wOSAxSDR2MmgyLjgxYzEuMDQgMS43OSAyLjk3IDMgNS4xOSAzczQuMTUtMS4yMSA1LjE5LTNIMjB2LTJoLTIuMDljLjA1LS4zMy4wOS0uNjYuMDktMXYtMWgydi0yaC0ydi0xYzAtLjM0LS4wNC0uNjctLjA5LTFIMjBWOHptLTYgOGgtNHYtMmg0djJ6bTAtNGgtNHYtMmg0djJ6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-build: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE0LjkgMTcuNDVDMTYuMjUgMTcuNDUgMTcuMzUgMTYuMzUgMTcuMzUgMTVDMTcuMzUgMTMuNjUgMTYuMjUgMTIuNTUgMTQuOSAxMi41NUMxMy41NCAxMi41NSAxMi40NSAxMy42NSAxMi40NSAxNUMxMi40NSAxNi4zNSAxMy41NCAxNy40NSAxNC45IDE3LjQ1Wk0yMC4xIDE1LjY4TDIxLjU4IDE2Ljg0QzIxLjcxIDE2Ljk1IDIxLjc1IDE3LjEzIDIxLjY2IDE3LjI5TDIwLjI2IDE5LjcxQzIwLjE3IDE5Ljg2IDIwIDE5LjkyIDE5LjgzIDE5Ljg2TDE4LjA5IDE5LjE2QzE3LjczIDE5LjQ0IDE3LjMzIDE5LjY3IDE2LjkxIDE5Ljg1TDE2LjY0IDIxLjdDMTYuNjIgMjEuODcgMTYuNDcgMjIgMTYuMyAyMkgxMy41QzEzLjMyIDIyIDEzLjE4IDIxLjg3IDEzLjE1IDIxLjdMMTIuODkgMTkuODVDMTIuNDYgMTkuNjcgMTIuMDcgMTkuNDQgMTEuNzEgMTkuMTZMOS45NjAwMiAxOS44NkM5LjgxMDAyIDE5LjkyIDkuNjIwMDIgMTkuODYgOS41NDAwMiAxOS43MUw4LjE0MDAyIDE3LjI5QzguMDUwMDIgMTcuMTMgOC4wOTAwMiAxNi45NSA4LjIyMDAyIDE2Ljg0TDkuNzAwMDIgMTUuNjhMOS42NTAwMSAxNUw5LjcwMDAyIDE0LjMxTDguMjIwMDIgMTMuMTZDOC4wOTAwMiAxMy4wNSA4LjA1MDAyIDEyLjg2IDguMTQwMDIgMTIuNzFMOS41NDAwMiAxMC4yOUM5LjYyMDAyIDEwLjEzIDkuODEwMDIgMTAuMDcgOS45NjAwMiAxMC4xM0wxMS43MSAxMC44NEMxMi4wNyAxMC41NiAxMi40NiAxMC4zMiAxMi44OSAxMC4xNUwxMy4xNSA4LjI4OTk4QzEzLjE4IDguMTI5OTggMTMuMzIgNy45OTk5OCAxMy41IDcuOTk5OThIMTYuM0MxNi40NyA3Ljk5OTk4IDE2LjYyIDguMTI5OTggMTYuNjQgOC4yODk5OEwxNi45MSAxMC4xNUMxNy4zMyAxMC4zMiAxNy43MyAxMC41NiAxOC4wOSAxMC44NEwxOS44MyAxMC4xM0MyMCAxMC4wNyAyMC4xNyAxMC4xMyAyMC4yNiAxMC4yOUwyMS42NiAxMi43MUMyMS43NSAxMi44NiAyMS43MSAxMy4wNSAyMS41OCAxMy4xNkwyMC4xIDE0LjMxTDIwLjE1IDE1TDIwLjEgMTUuNjhaIi8+CiAgICA8cGF0aCBkPSJNNy4zMjk2NiA3LjQ0NDU0QzguMDgzMSA3LjAwOTU0IDguMzM5MzIgNi4wNTMzMiA3LjkwNDMyIDUuMjk5ODhDNy40NjkzMiA0LjU0NjQzIDYuNTA4MSA0LjI4MTU2IDUuNzU0NjYgNC43MTY1NkM1LjM5MTc2IDQuOTI2MDggNS4xMjY5NSA1LjI3MTE4IDUuMDE4NDkgNS42NzU5NEM0LjkxMDA0IDYuMDgwNzEgNC45NjY4MiA2LjUxMTk4IDUuMTc2MzQgNi44NzQ4OEM1LjYxMTM0IDcuNjI4MzIgNi41NzYyMiA3Ljg3OTU0IDcuMzI5NjYgNy40NDQ1NFpNOS42NTcxOCA0Ljc5NTkzTDEwLjg2NzIgNC45NTE3OUMxMC45NjI4IDQuOTc3NDEgMTEuMDQwMiA1LjA3MTMzIDExLjAzODIgNS4xODc5M0wxMS4wMzg4IDYuOTg4OTNDMTEuMDQ1NSA3LjEwMDU0IDEwLjk2MTYgNy4xOTUxOCAxMC44NTUgNy4yMTA1NEw5LjY2MDAxIDcuMzgwODNMOS4yMzkxNSA4LjEzMTg4TDkuNjY5NjEgOS4yNTc0NUM5LjcwNzI5IDkuMzYyNzEgOS42NjkzNCA5LjQ3Njk5IDkuNTc0MDggOS41MzE5OUw4LjAxNTIzIDEwLjQzMkM3LjkxMTMxIDEwLjQ5MiA3Ljc5MzM3IDEwLjQ2NzcgNy43MjEwNSAxMC4zODI0TDYuOTg3NDggOS40MzE4OEw2LjEwOTMxIDkuNDMwODNMNS4zNDcwNCAxMC4zOTA1QzUuMjg5MDkgMTAuNDcwMiA1LjE3MzgzIDEwLjQ5MDUgNS4wNzE4NyAxMC40MzM5TDMuNTEyNDUgOS41MzI5M0MzLjQxMDQ5IDkuNDc2MzMgMy4zNzY0NyA5LjM1NzQxIDMuNDEwNzUgOS4yNTY3OUwzLjg2MzQ3IDguMTQwOTNMMy42MTc0OSA3Ljc3NDg4TDMuNDIzNDcgNy4zNzg4M0wyLjIzMDc1IDcuMjEyOTdDMi4xMjY0NyA3LjE5MjM1IDIuMDQwNDkgNy4xMDM0MiAyLjA0MjQ1IDYuOTg2ODJMMi4wNDE4NyA1LjE4NTgyQzIuMDQzODMgNS4wNjkyMiAyLjExOTA5IDQuOTc5NTggMi4yMTcwNCA0Ljk2OTIyTDMuNDIwNjUgNC43OTM5M0wzLjg2NzQ5IDQuMDI3ODhMMy40MTEwNSAyLjkxNzMxQzMuMzczMzcgMi44MTIwNCAzLjQxMTMxIDIuNjk3NzYgMy41MTUyMyAyLjYzNzc2TDUuMDc0MDggMS43Mzc3NkM1LjE2OTM0IDEuNjgyNzYgNS4yODcyOSAxLjcwNzA0IDUuMzU5NjEgMS43OTIzMUw2LjExOTE1IDIuNzI3ODhMNi45ODAwMSAyLjczODkzTDcuNzI0OTYgMS43ODkyMkM3Ljc5MTU2IDEuNzA0NTggNy45MTU0OCAxLjY3OTIyIDguMDA4NzkgMS43NDA4Mkw5LjU2ODIxIDIuNjQxODJDOS42NzAxNyAyLjY5ODQyIDkuNzEyODUgMi44MTIzNCA5LjY4NzIzIDIuOTA3OTdMOS4yMTcxOCA0LjAzMzgzTDkuNDYzMTYgNC4zOTk4OEw5LjY1NzE4IDQuNzk1OTNaIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iOS45LDEzLjYgMy42LDcuNCA0LjQsNi42IDkuOSwxMi4yIDE1LjQsNi43IDE2LjEsNy40ICIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNS45TDksOS43bDMuOC0zLjhsMS4yLDEuMmwtNC45LDVsLTQuOS01TDUuMiw1Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-caret-down: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik01LjIsNy41TDksMTEuMmwzLjgtMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-left: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik0xMC44LDEyLjhMNy4xLDlsMy44LTMuOGwwLDcuNkgxMC44eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-right: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiIHNoYXBlLXJlbmRlcmluZz0iZ2VvbWV0cmljUHJlY2lzaW9uIj4KICAgIDxwYXRoIGQ9Ik03LjIsNS4yTDEwLjksOWwtMy44LDMuOFY1LjJINy4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-caret-up-empty-thin: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwb2x5Z29uIGNsYXNzPSJzdDEiIHBvaW50cz0iMTUuNCwxMy4zIDkuOSw3LjcgNC40LDEzLjIgMy42LDEyLjUgOS45LDYuMyAxNi4xLDEyLjYgIi8+Cgk8L2c+Cjwvc3ZnPgo=);
  --jp-icon-caret-up: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSIgc2hhcGUtcmVuZGVyaW5nPSJnZW9tZXRyaWNQcmVjaXNpb24iPgoJCTxwYXRoIGQ9Ik01LjIsMTAuNUw5LDYuOGwzLjgsMy44SDUuMnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-case-sensitive: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWFjY2VudDIiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTcuNiw4aDAuOWwzLjUsOGgtMS4xTDEwLDE0SDZsLTAuOSwySDRMNy42LDh6IE04LDkuMUw2LjQsMTNoMy4yTDgsOS4xeiIvPgogICAgPHBhdGggZD0iTTE2LjYsOS44Yy0wLjIsMC4xLTAuNCwwLjEtMC43LDAuMWMtMC4yLDAtMC40LTAuMS0wLjYtMC4yYy0wLjEtMC4xLTAuMi0wLjQtMC4yLTAuNyBjLTAuMywwLjMtMC42LDAuNS0wLjksMC43Yy0wLjMsMC4xLTAuNywwLjItMS4xLDAuMmMtMC4zLDAtMC41LDAtMC43LTAuMWMtMC4yLTAuMS0wLjQtMC4yLTAuNi0wLjNjLTAuMi0wLjEtMC4zLTAuMy0wLjQtMC41IGMtMC4xLTAuMi0wLjEtMC40LTAuMS0wLjdjMC0wLjMsMC4xLTAuNiwwLjItMC44YzAuMS0wLjIsMC4zLTAuNCwwLjQtMC41QzEyLDcsMTIuMiw2LjksMTIuNSw2LjhjMC4yLTAuMSwwLjUtMC4xLDAuNy0wLjIgYzAuMy0wLjEsMC41LTAuMSwwLjctMC4xYzAuMiwwLDAuNC0wLjEsMC42LTAuMWMwLjIsMCwwLjMtMC4xLDAuNC0wLjJjMC4xLTAuMSwwLjItMC4yLDAuMi0wLjRjMC0xLTEuMS0xLTEuMy0xIGMtMC40LDAtMS40LDAtMS40LDEuMmgtMC45YzAtMC40LDAuMS0wLjcsMC4yLTFjMC4xLTAuMiwwLjMtMC40LDAuNS0wLjZjMC4yLTAuMiwwLjUtMC4zLDAuOC0wLjNDMTMuMyw0LDEzLjYsNCwxMy45LDQgYzAuMywwLDAuNSwwLDAuOCwwLjFjMC4zLDAsMC41LDAuMSwwLjcsMC4yYzAuMiwwLjEsMC40LDAuMywwLjUsMC41QzE2LDUsMTYsNS4yLDE2LDUuNnYyLjljMCwwLjIsMCwwLjQsMCwwLjUgYzAsMC4xLDAuMSwwLjIsMC4zLDAuMmMwLjEsMCwwLjIsMCwwLjMsMFY5Ljh6IE0xNS4yLDYuOWMtMS4yLDAuNi0zLjEsMC4yLTMuMSwxLjRjMCwxLjQsMy4xLDEsMy4xLTAuNVY2Ljl6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik05IDE2LjE3TDQuODMgMTJsLTEuNDIgMS40MUw5IDE5IDIxIDdsLTEuNDEtMS40MXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-circle-empty: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDJDNi40NyAyIDIgNi40NyAyIDEyczQuNDcgMTAgMTAgMTAgMTAtNC40NyAxMC0xMFMxNy41MyAyIDEyIDJ6bTAgMThjLTQuNDEgMC04LTMuNTktOC04czMuNTktOCA4LTggOCAzLjU5IDggOC0zLjU5IDgtOCA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-circle: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iOSIgY3k9IjkiIHI9IjgiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-clear: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8bWFzayBpZD0iZG9udXRIb2xlIj4KICAgIDxyZWN0IHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgZmlsbD0id2hpdGUiIC8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSI4IiBmaWxsPSJibGFjayIvPgogIDwvbWFzaz4KCiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxyZWN0IGhlaWdodD0iMTgiIHdpZHRoPSIyIiB4PSIxMSIgeT0iMyIgdHJhbnNmb3JtPSJyb3RhdGUoMzE1LCAxMiwgMTIpIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIxMCIgbWFzaz0idXJsKCNkb251dEhvbGUpIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-close: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1ub25lIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIGpwLWljb24zLWhvdmVyIiBmaWxsPSJub25lIj4KICAgIDxjaXJjbGUgY3g9IjEyIiBjeT0iMTIiIHI9IjExIi8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIGpwLWljb24tYWNjZW50Mi1ob3ZlciIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMTkgNi40MUwxNy41OSA1IDEyIDEwLjU5IDYuNDEgNSA1IDYuNDEgMTAuNTkgMTIgNSAxNy41OSA2LjQxIDE5IDEyIDEzLjQxIDE3LjU5IDE5IDE5IDE3LjU5IDEzLjQxIDEyeiIvPgogIDwvZz4KCiAgPGcgY2xhc3M9ImpwLWljb24tbm9uZSBqcC1pY29uLWJ1c3kiIGZpbGw9Im5vbmUiPgogICAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code-check: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBzaGFwZS1yZW5kZXJpbmc9Imdlb21ldHJpY1ByZWNpc2lvbiI+CiAgICA8cGF0aCBkPSJNNi41OSwzLjQxTDIsOEw2LjU5LDEyLjZMOCwxMS4xOEw0LjgyLDhMOCw0LjgyTDYuNTksMy40MU0xMi40MSwzLjQxTDExLDQuODJMMTQuMTgsOEwxMSwxMS4xOEwxMi40MSwxMi42TDE3LDhMMTIuNDEsMy40MU0yMS41OSwxMS41OUwxMy41LDE5LjY4TDkuODMsMTZMOC40MiwxNy40MUwxMy41LDIyLjVMMjMsMTNMMjEuNTksMTEuNTlaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-code: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTExLjQgMTguNkw2LjggMTRMMTEuNCA5LjRMMTAgOEw0IDE0TDEwIDIwTDExLjQgMTguNlpNMTYuNiAxOC42TDIxLjIgMTRMMTYuNiA5LjRMMTggOEwyNCAxNEwxOCAyMEwxNi42IDE4LjZWMTguNloiLz4KCTwvZz4KPC9zdmc+Cg==);
  --jp-icon-collapse-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNNiAxM3YyaDh2LTJ6IiAvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-console: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwMCAyMDAiPgogIDxnIGNsYXNzPSJqcC1jb25zb2xlLWljb24tYmFja2dyb3VuZC1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMjg4RDEiPgogICAgPHBhdGggZD0iTTIwIDE5LjhoMTYwdjE1OS45SDIweiIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtY29uc29sZS1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIj4KICAgIDxwYXRoIGQ9Ik0xMDUgMTI3LjNoNDB2MTIuOGgtNDB6TTUxLjEgNzdMNzQgOTkuOWwtMjMuMyAyMy4zIDEwLjUgMTAuNSAyMy4zLTIzLjNMOTUgOTkuOSA4NC41IDg5LjQgNjEuNiA2Ni41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copy: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTExLjksMUgzLjJDMi40LDEsMS43LDEuNywxLjcsMi41djEwLjJoMS41VjIuNWg4LjdWMXogTTE0LjEsMy45aC04Yy0wLjgsMC0xLjUsMC43LTEuNSwxLjV2MTAuMmMwLDAuOCwwLjcsMS41LDEuNSwxLjVoOCBjMC44LDAsMS41LTAuNywxLjUtMS41VjUuNEMxNS41LDQuNiwxNC45LDMuOSwxNC4xLDMuOXogTTE0LjEsMTUuNWgtOFY1LjRoOFYxNS41eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-copyright: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGVuYWJsZS1iYWNrZ3JvdW5kPSJuZXcgMCAwIDI0IDI0IiBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCI+CiAgPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0xMS44OCw5LjE0YzEuMjgsMC4wNiwxLjYxLDEuMTUsMS42MywxLjY2aDEuNzljLTAuMDgtMS45OC0xLjQ5LTMuMTktMy40NS0zLjE5QzkuNjQsNy42MSw4LDksOCwxMi4xNCBjMCwxLjk0LDAuOTMsNC4yNCwzLjg0LDQuMjRjMi4yMiwwLDMuNDEtMS42NSwzLjQ0LTIuOTVoLTEuNzljLTAuMDMsMC41OS0wLjQ1LDEuMzgtMS42MywxLjQ0QzEwLjU1LDE0LjgzLDEwLDEzLjgxLDEwLDEyLjE0IEMxMCw5LjI1LDExLjI4LDkuMTYsMTEuODgsOS4xNHogTTEyLDJDNi40OCwyLDIsNi40OCwyLDEyczQuNDgsMTAsMTAsMTBzMTAtNC40OCwxMC0xMFMxNy41MiwyLDEyLDJ6IE0xMiwyMGMtNC40MSwwLTgtMy41OS04LTggczMuNTktOCw4LThzOCwzLjU5LDgsOFMxNi40MSwyMCwxMiwyMHoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-cut: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkuNjQgNy42NGMuMjMtLjUuMzYtMS4wNS4zNi0xLjY0IDAtMi4yMS0xLjc5LTQtNC00UzIgMy43OSAyIDZzMS43OSA0IDQgNGMuNTkgMCAxLjE0LS4xMyAxLjY0LS4zNkwxMCAxMmwtMi4zNiAyLjM2QzcuMTQgMTQuMTMgNi41OSAxNCA2IDE0Yy0yLjIxIDAtNCAxLjc5LTQgNHMxLjc5IDQgNCA0IDQtMS43OSA0LTRjMC0uNTktLjEzLTEuMTQtLjM2LTEuNjRMMTIgMTRsNyA3aDN2LTFMOS42NCA3LjY0ek02IDhjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTAgMTJjLTEuMSAwLTItLjg5LTItMnMuOS0yIDItMiAyIC44OSAyIDItLjkgMi0yIDJ6bTYtNy41Yy0uMjggMC0uNS0uMjItLjUtLjVzLjIyLS41LjUtLjUuNS4yMi41LjUtLjIyLjUtLjUuNXpNMTkgM2wtNiA2IDIgMiA3LTdWM3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-delete: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2cHgiIGhlaWdodD0iMTZweCI+CiAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIiAvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjI2MjYyIiBkPSJNNiAxOWMwIDEuMS45IDIgMiAyaDhjMS4xIDAgMi0uOSAyLTJWN0g2djEyek0xOSA0aC0zLjVsLTEtMWgtNWwtMSAxSDV2MmgxNFY0eiIgLz4KPC9zdmc+Cg==);
  --jp-icon-download: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE5IDloLTRWM0g5djZINWw3IDcgNy03ek01IDE4djJoMTR2LTJINXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-duplicate: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBmaWxsLXJ1bGU9ImV2ZW5vZGQiIGNsaXAtcnVsZT0iZXZlbm9kZCIgZD0iTTIuNzk5OTggMC44NzVIOC44OTU4MkM5LjIwMDYxIDAuODc1IDkuNDQ5OTggMS4xMzkxNCA5LjQ0OTk4IDEuNDYxOThDOS40NDk5OCAxLjc4NDgyIDkuMjAwNjEgMi4wNDg5NiA4Ljg5NTgyIDIuMDQ4OTZIMy4zNTQxNUMzLjA0OTM2IDIuMDQ4OTYgMi43OTk5OCAyLjMxMzEgMi43OTk5OCAyLjYzNTk0VjkuNjc5NjlDMi43OTk5OCAxMC4wMDI1IDIuNTUwNjEgMTAuMjY2NyAyLjI0NTgyIDEwLjI2NjdDMS45NDEwMyAxMC4yNjY3IDEuNjkxNjUgMTAuMDAyNSAxLjY5MTY1IDkuNjc5NjlWMi4wNDg5NkMxLjY5MTY1IDEuNDAzMjggMi4xOTA0IDAuODc1IDIuNzk5OTggMC44NzVaTTUuMzY2NjUgMTEuOVY0LjU1SDExLjA4MzNWMTEuOUg1LjM2NjY1Wk00LjE0MTY1IDQuMTQxNjdDNC4xNDE2NSAzLjY5MDYzIDQuNTA3MjggMy4zMjUgNC45NTgzMiAzLjMyNUgxMS40OTE3QzExLjk0MjcgMy4zMjUgMTIuMzA4MyAzLjY5MDYzIDEyLjMwODMgNC4xNDE2N1YxMi4zMDgzQzEyLjMwODMgMTIuNzU5NCAxMS45NDI3IDEzLjEyNSAxMS40OTE3IDEzLjEyNUg0Ljk1ODMyQzQuNTA3MjggMTMuMTI1IDQuMTQxNjUgMTIuNzU5NCA0LjE0MTY1IDEyLjMwODNWNC4xNDE2N1oiIGZpbGw9IiM2MTYxNjEiLz4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNOS40MzU3NCA4LjI2NTA3SDguMzY0MzFWOS4zMzY1QzguMzY0MzEgOS40NTQzNSA4LjI2Nzg4IDkuNTUwNzggOC4xNTAwMiA5LjU1MDc4QzguMDMyMTcgOS41NTA3OCA3LjkzNTc0IDkuNDU0MzUgNy45MzU3NCA5LjMzNjVWOC4yNjUwN0g2Ljg2NDMxQzYuNzQ2NDUgOC4yNjUwNyA2LjY1MDAyIDguMTY4NjQgNi42NTAwMiA4LjA1MDc4QzYuNjUwMDIgNy45MzI5MiA2Ljc0NjQ1IDcuODM2NSA2Ljg2NDMxIDcuODM2NUg3LjkzNTc0VjYuNzY1MDdDNy45MzU3NCA2LjY0NzIxIDguMDMyMTcgNi41NTA3OCA4LjE1MDAyIDYuNTUwNzhDOC4yNjc4OCA2LjU1MDc4IDguMzY0MzEgNi42NDcyMSA4LjM2NDMxIDYuNzY1MDdWNy44MzY1SDkuNDM1NzRDOS41NTM2IDcuODM2NSA5LjY1MDAyIDcuOTMyOTIgOS42NTAwMiA4LjA1MDc4QzkuNjUwMDIgOC4xNjg2NCA5LjU1MzYgOC4yNjUwNyA5LjQzNTc0IDguMjY1MDdaIiBmaWxsPSIjNjE2MTYxIiBzdHJva2U9IiM2MTYxNjEiIHN0cm9rZS13aWR0aD0iMC41Ii8+Cjwvc3ZnPgo=);
  --jp-icon-edit: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMgMTcuMjVWMjFoMy43NUwxNy44MSA5Ljk0bC0zLjc1LTMuNzVMMyAxNy4yNXpNMjAuNzEgNy4wNGMuMzktLjM5LjM5LTEuMDIgMC0xLjQxbC0yLjM0LTIuMzRjLS4zOS0uMzktMS4wMi0uMzktMS40MSAwbC0xLjgzIDEuODMgMy43NSAzLjc1IDEuODMtMS44M3oiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-ellipses: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPGNpcmNsZSBjeD0iNSIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxMiIgY3k9IjEyIiByPSIyIi8+CiAgICA8Y2lyY2xlIGN4PSIxOSIgY3k9IjEyIiByPSIyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-error: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj48Y2lyY2xlIGN4PSIxMiIgY3k9IjE5IiByPSIyIi8+PHBhdGggZD0iTTEwIDNoNHYxMmgtNHoiLz48L2c+CjxwYXRoIGZpbGw9Im5vbmUiIGQ9Ik0wIDBoMjR2MjRIMHoiLz4KPC9zdmc+Cg==);
  --jp-icon-expand-all: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTggMmMxIDAgMTEgMCAxMiAwczIgMSAyIDJjMCAxIDAgMTEgMCAxMnMwIDItMiAyQzIwIDE0IDIwIDQgMjAgNFMxMCA0IDYgNGMwLTIgMS0yIDItMnoiIC8+CiAgICAgICAgPHBhdGgKICAgICAgICAgICAgZD0iTTE4IDhjMC0xLTEtMi0yLTJTNSA2IDQgNnMtMiAxLTIgMmMwIDEgMCAxMSAwIDEyczEgMiAyIDJjMSAwIDExIDAgMTIgMHMyLTEgMi0yYzAtMSAwLTExIDAtMTJ6bS0yIDB2MTJINFY4eiIgLz4KICAgICAgICA8cGF0aCBkPSJNMTEgMTBIOXYzSDZ2MmgzdjNoMnYtM2gzdi0yaC0zeiIgLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-extension: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwLjUgMTFIMTlWN2MwLTEuMS0uOS0yLTItMmgtNFYzLjVDMTMgMi4xMiAxMS44OCAxIDEwLjUgMVM4IDIuMTIgOCAzLjVWNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAydjMuOEgzLjVjMS40OSAwIDIuNyAxLjIxIDIuNyAyLjdzLTEuMjEgMi43LTIuNyAyLjdIMlYyMGMwIDEuMS45IDIgMiAyaDMuOHYtMS41YzAtMS40OSAxLjIxLTIuNyAyLjctMi43IDEuNDkgMCAyLjcgMS4yMSAyLjcgMi43VjIySDE3YzEuMSAwIDItLjkgMi0ydi00aDEuNWMxLjM4IDAgMi41LTEuMTIgMi41LTIuNVMyMS44OCAxMSAyMC41IDExeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-fast-forward: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTQgMThsOC41LTZMNCA2djEyem05LTEydjEybDguNS02TDEzIDZ6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-file-upload: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTkgMTZoNnYtNmg0bC03LTctNyA3aDR6bS00IDJoMTR2Mkg1eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-file: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuMyA4LjJsLTUuNS01LjVjLS4zLS4zLS43LS41LTEuMi0uNUgzLjljLS44LjEtMS42LjktMS42IDEuOHYxNC4xYzAgLjkuNyAxLjYgMS42IDEuNmgxNC4yYy45IDAgMS42LS43IDEuNi0xLjZWOS40Yy4xLS41LS4xLS45LS40LTEuMnptLTUuOC0zLjNsMy40IDMuNmgtMy40VjQuOXptMy45IDEyLjdINC43Yy0uMSAwLS4yIDAtLjItLjJWNC43YzAtLjIuMS0uMy4yLS4zaDcuMnY0LjRzMCAuOC4zIDEuMWMuMy4zIDEuMS4zIDEuMS4zaDQuM3Y3LjJzLS4xLjItLjIuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-filter-dot: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgogIDxnIGNsYXNzPSJqcC1pY29uLWRvdCIgZmlsbD0iI0ZGRiI+CiAgICA8Y2lyY2xlIGN4PSIxOCIgY3k9IjE3IiByPSIzIj48L2NpcmNsZT4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-filter-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEwIDE4aDR2LTJoLTR2MnpNMyA2djJoMThWNkgzem0zIDdoMTJ2LTJINnYyeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-filter: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiNGRkYiPgogICAgPHBhdGggZD0iTTE0LDEyVjE5Ljg4QzE0LjA0LDIwLjE4IDEzLjk0LDIwLjUgMTMuNzEsMjAuNzFDMTMuMzIsMjEuMSAxMi42OSwyMS4xIDEyLjMsMjAuNzFMMTAuMjksMTguN0MxMC4wNiwxOC40NyA5Ljk2LDE4LjE2IDEwLDE3Ljg3VjEySDkuOTdMNC4yMSw0LjYyQzMuODcsNC4xOSAzLjk1LDMuNTYgNC4zOCwzLjIyQzQuNTcsMy4wOCA0Ljc4LDMgNSwzVjNIMTlWM0MxOS4yMiwzIDE5LjQzLDMuMDggMTkuNjIsMy4yMkMyMC4wNSwzLjU2IDIwLjEzLDQuMTkgMTkuNzksNC42MkwxNC4wMywxMkgxNFoiIC8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-folder-favorite: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgwVjB6IiBmaWxsPSJub25lIi8+PHBhdGggY2xhc3M9ImpwLWljb24zIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxNjE2MSIgZD0iTTIwIDZoLThsLTItMkg0Yy0xLjEgMC0yIC45LTIgMnYxMmMwIDEuMS45IDIgMiAyaDE2YzEuMSAwIDItLjkgMi0yVjhjMC0xLjEtLjktMi0yLTJ6bS0yLjA2IDExTDE1IDE1LjI4IDEyLjA2IDE3bC43OC0zLjMzLTIuNTktMi4yNCAzLjQxLS4yOUwxNSA4bDEuMzQgMy4xNCAzLjQxLjI5LTIuNTkgMi4yNC43OCAzLjMzeiIvPgo8L3N2Zz4K);
  --jp-icon-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY4YzAtMS4xLS45LTItMi0yaC04bC0yLTJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-home: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjRweCIgdmlld0JveD0iMCAwIDI0IDI0IiB3aWR0aD0iMjRweCIgZmlsbD0iIzAwMDAwMCI+CiAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPjxwYXRoIGNsYXNzPSJqcC1pY29uMyBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xMCAyMHYtNmg0djZoNXYtOGgzTDEyIDMgMiAxMmgzdjh6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-html5: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uMCBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiMwMDAiIGQ9Ik0xMDguNCAwaDIzdjIyLjhoMjEuMlYwaDIzdjY5aC0yM1Y0NmgtMjF2MjNoLTIzLjJNMjA2IDIzaC0yMC4zVjBoNjMuN3YyM0gyMjl2NDZoLTIzbTUzLjUtNjloMjQuMWwxNC44IDI0LjNMMzEzLjIgMGgyNC4xdjY5aC0yM1YzNC44bC0xNi4xIDI0LjgtMTYuMS0yNC44VjY5aC0yMi42bTg5LjItNjloMjN2NDYuMmgzMi42VjY5aC01NS42Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2U0NGQyNiIgZD0iTTEwNy42IDQ3MWwtMzMtMzcwLjRoMzYyLjhsLTMzIDM3MC4yTDI1NS43IDUxMiIvPgogIDxwYXRoIGNsYXNzPSJqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNmMTY1MjkiIGQ9Ik0yNTYgNDgwLjVWMTMxaDE0OC4zTDM3NiA0NDciLz4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNlYmViZWIiIGQ9Ik0xNDIgMTc2LjNoMTE0djQ1LjRoLTY0LjJsNC4yIDQ2LjVoNjB2NDUuM0gxNTQuNG0yIDIyLjhIMjAybDMuMiAzNi4zIDUwLjggMTMuNnY0Ny40bC05My4yLTI2Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZS1pbnZlcnNlIiBmaWxsPSIjZmZmIiBkPSJNMzY5LjYgMTc2LjNIMjU1Ljh2NDUuNGgxMDkuNm0tNC4xIDQ2LjVIMjU1Ljh2NDUuNGg1NmwtNS4zIDU5LTUwLjcgMTMuNnY0Ny4ybDkzLTI1LjgiLz4KPC9zdmc+Cg==);
  --jp-icon-image: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1icmFuZDQganAtaWNvbi1zZWxlY3RhYmxlLWludmVyc2UiIGZpbGw9IiNGRkYiIGQ9Ik0yLjIgMi4yaDE3LjV2MTcuNUgyLjJ6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzNGNTFCNSIgZD0iTTIuMiAyLjJ2MTcuNWgxNy41bC4xLTE3LjVIMi4yem0xMi4xIDIuMmMxLjIgMCAyLjIgMSAyLjIgMi4ycy0xIDIuMi0yLjIgMi4yLTIuMi0xLTIuMi0yLjIgMS0yLjIgMi4yLTIuMnpNNC40IDE3LjZsMy4zLTguOCAzLjMgNi42IDIuMi0zLjIgNC40IDUuNEg0LjR6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-info: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUwLjk3OCA1MC45NzgiPgoJPGcgY2xhc3M9ImpwLWljb24zIiBmaWxsPSIjNjE2MTYxIj4KCQk8cGF0aCBkPSJNNDMuNTIsNy40NThDMzguNzExLDIuNjQ4LDMyLjMwNywwLDI1LjQ4OSwwQzE4LjY3LDAsMTIuMjY2LDIuNjQ4LDcuNDU4LDcuNDU4CgkJCWMtOS45NDMsOS45NDEtOS45NDMsMjYuMTE5LDAsMzYuMDYyYzQuODA5LDQuODA5LDExLjIxMiw3LjQ1NiwxOC4wMzEsNy40NThjMCwwLDAuMDAxLDAsMC4wMDIsMAoJCQljNi44MTYsMCwxMy4yMjEtMi42NDgsMTguMDI5LTcuNDU4YzQuODA5LTQuODA5LDcuNDU3LTExLjIxMiw3LjQ1Ny0xOC4wM0M1MC45NzcsMTguNjcsNDguMzI4LDEyLjI2Niw0My41Miw3LjQ1OHoKCQkJIE00Mi4xMDYsNDIuMTA1Yy00LjQzMiw0LjQzMS0xMC4zMzIsNi44NzItMTYuNjE1LDYuODcyaC0wLjAwMmMtNi4yODUtMC4wMDEtMTIuMTg3LTIuNDQxLTE2LjYxNy02Ljg3MgoJCQljLTkuMTYyLTkuMTYzLTkuMTYyLTI0LjA3MSwwLTMzLjIzM0MxMy4zMDMsNC40NCwxOS4yMDQsMiwyNS40ODksMmM2LjI4NCwwLDEyLjE4NiwyLjQ0LDE2LjYxNyw2Ljg3MgoJCQljNC40MzEsNC40MzEsNi44NzEsMTAuMzMyLDYuODcxLDE2LjYxN0M0OC45NzcsMzEuNzcyLDQ2LjUzNiwzNy42NzUsNDIuMTA2LDQyLjEwNXoiLz4KCQk8cGF0aCBkPSJNMjMuNTc4LDMyLjIxOGMtMC4wMjMtMS43MzQsMC4xNDMtMy4wNTksMC40OTYtMy45NzJjMC4zNTMtMC45MTMsMS4xMS0xLjk5NywyLjI3Mi0zLjI1MwoJCQljMC40NjgtMC41MzYsMC45MjMtMS4wNjIsMS4zNjctMS41NzVjMC42MjYtMC43NTMsMS4xMDQtMS40NzgsMS40MzYtMi4xNzVjMC4zMzEtMC43MDcsMC40OTUtMS41NDEsMC40OTUtMi41CgkJCWMwLTEuMDk2LTAuMjYtMi4wODgtMC43NzktMi45NzljLTAuNTY1LTAuODc5LTEuNTAxLTEuMzM2LTIuODA2LTEuMzY5Yy0xLjgwMiwwLjA1Ny0yLjk4NSwwLjY2Ny0zLjU1LDEuODMyCgkJCWMtMC4zMDEsMC41MzUtMC41MDMsMS4xNDEtMC42MDcsMS44MTRjLTAuMTM5LDAuNzA3LTAuMjA3LDEuNDMyLTAuMjA3LDIuMTc0aC0yLjkzN2MtMC4wOTEtMi4yMDgsMC40MDctNC4xMTQsMS40OTMtNS43MTkKCQkJYzEuMDYyLTEuNjQsMi44NTUtMi40ODEsNS4zNzgtMi41MjdjMi4xNiwwLjAyMywzLjg3NCwwLjYwOCw1LjE0MSwxLjc1OGMxLjI3OCwxLjE2LDEuOTI5LDIuNzY0LDEuOTUsNC44MTEKCQkJYzAsMS4xNDItMC4xMzcsMi4xMTEtMC40MSwyLjkxMWMtMC4zMDksMC44NDUtMC43MzEsMS41OTMtMS4yNjgsMi4yNDNjLTAuNDkyLDAuNjUtMS4wNjgsMS4zMTgtMS43MywyLjAwMgoJCQljLTAuNjUsMC42OTctMS4zMTMsMS40NzktMS45ODcsMi4zNDZjLTAuMjM5LDAuMzc3LTAuNDI5LDAuNzc3LTAuNTY1LDEuMTk5Yy0wLjE2LDAuOTU5LTAuMjE3LDEuOTUxLTAuMTcxLDIuOTc5CgkJCUMyNi41ODksMzIuMjE4LDIzLjU3OCwzMi4yMTgsMjMuNTc4LDMyLjIxOHogTTIzLjU3OCwzOC4yMnYtMy40ODRoMy4wNzZ2My40ODRIMjMuNTc4eiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-inspector: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaW5zcGVjdG9yLWljb24tY29sb3IganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNEg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMThjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY2YzAtMS4xLS45LTItMi0yem0tNSAxNEg0di00aDExdjR6bTAtNUg0VjloMTF2NHptNSA1aC00VjloNHY5eiIvPgo8L3N2Zz4K);
  --jp-icon-json: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtanNvbi1pY29uLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0Y5QTgyNSI+CiAgICA8cGF0aCBkPSJNMjAuMiAxMS44Yy0xLjYgMC0xLjcuNS0xLjcgMSAwIC40LjEuOS4xIDEuMy4xLjUuMS45LjEgMS4zIDAgMS43LTEuNCAyLjMtMy41IDIuM2gtLjl2LTEuOWguNWMxLjEgMCAxLjQgMCAxLjQtLjggMC0uMyAwLS42LS4xLTEgMC0uNC0uMS0uOC0uMS0xLjIgMC0xLjMgMC0xLjggMS4zLTItMS4zLS4yLTEuMy0uNy0xLjMtMiAwLS40LjEtLjguMS0xLjIuMS0uNC4xLS43LjEtMSAwLS44LS40LS43LTEuNC0uOGgtLjVWNC4xaC45YzIuMiAwIDMuNS43IDMuNSAyLjMgMCAuNC0uMS45LS4xIDEuMy0uMS41LS4xLjktLjEgMS4zIDAgLjUuMiAxIDEuNyAxdjEuOHpNMS44IDEwLjFjMS42IDAgMS43LS41IDEuNy0xIDAtLjQtLjEtLjktLjEtMS4zLS4xLS41LS4xLS45LS4xLTEuMyAwLTEuNiAxLjQtMi4zIDMuNS0yLjNoLjl2MS45aC0uNWMtMSAwLTEuNCAwLTEuNC44IDAgLjMgMCAuNi4xIDEgMCAuMi4xLjYuMSAxIDAgMS4zIDAgMS44LTEuMyAyQzYgMTEuMiA2IDExLjcgNiAxM2MwIC40LS4xLjgtLjEgMS4yLS4xLjMtLjEuNy0uMSAxIDAgLjguMy44IDEuNC44aC41djEuOWgtLjljLTIuMSAwLTMuNS0uNi0zLjUtMi4zIDAtLjQuMS0uOS4xLTEuMy4xLS41LjEtLjkuMS0xLjMgMC0uNS0uMi0xLTEuNy0xdi0xLjl6Ii8+CiAgICA8Y2lyY2xlIGN4PSIxMSIgY3k9IjEzLjgiIHI9IjIuMSIvPgogICAgPGNpcmNsZSBjeD0iMTEiIGN5PSI4LjIiIHI9IjIuMSIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-julia: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDMyNSAzMDAiPgogIDxnIGNsYXNzPSJqcC1icmFuZDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjY2IzYzMzIj4KICAgIDxwYXRoIGQ9Ik0gMTUwLjg5ODQzOCAyMjUgQyAxNTAuODk4NDM4IDI2Ni40MjE4NzUgMTE3LjMyMDMxMiAzMDAgNzUuODk4NDM4IDMwMCBDIDM0LjQ3NjU2MiAzMDAgMC44OTg0MzggMjY2LjQyMTg3NSAwLjg5ODQzOCAyMjUgQyAwLjg5ODQzOCAxODMuNTc4MTI1IDM0LjQ3NjU2MiAxNTAgNzUuODk4NDM4IDE1MCBDIDExNy4zMjAzMTIgMTUwIDE1MC44OTg0MzggMTgzLjU3ODEyNSAxNTAuODk4NDM4IDIyNSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzM4OTgyNiI+CiAgICA8cGF0aCBkPSJNIDIzNy41IDc1IEMgMjM3LjUgMTE2LjQyMTg3NSAyMDMuOTIxODc1IDE1MCAxNjIuNSAxNTAgQyAxMjEuMDc4MTI1IDE1MCA4Ny41IDExNi40MjE4NzUgODcuNSA3NSBDIDg3LjUgMzMuNTc4MTI1IDEyMS4wNzgxMjUgMCAxNjIuNSAwIEMgMjAzLjkyMTg3NSAwIDIzNy41IDMzLjU3ODEyNSAyMzcuNSA3NSIvPgogIDwvZz4KICA8ZyBjbGFzcz0ianAtYnJhbmQwIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzk1NThiMiI+CiAgICA8cGF0aCBkPSJNIDMyNC4xMDE1NjIgMjI1IEMgMzI0LjEwMTU2MiAyNjYuNDIxODc1IDI5MC41MjM0MzggMzAwIDI0OS4xMDE1NjIgMzAwIEMgMjA3LjY3OTY4OCAzMDAgMTc0LjEwMTU2MiAyNjYuNDIxODc1IDE3NC4xMDE1NjIgMjI1IEMgMTc0LjEwMTU2MiAxODMuNTc4MTI1IDIwNy42Nzk2ODggMTUwIDI0OS4xMDE1NjIgMTUwIEMgMjkwLjUyMzQzOCAxNTAgMzI0LjEwMTU2MiAxODMuNTc4MTI1IDMyNC4xMDE1NjIgMjI1Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-jupyter-favicon: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTUyIiBoZWlnaHQ9IjE2NSIgdmlld0JveD0iMCAwIDE1MiAxNjUiIHZlcnNpb249IjEuMSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgPGcgY2xhc3M9ImpwLWp1cHl0ZXItaWNvbi1jb2xvciIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA3ODk0NywgMTEwLjU4MjkyNykiIGQ9Ik03NS45NDIyODQyLDI5LjU4MDQ1NjEgQzQzLjMwMjM5NDcsMjkuNTgwNDU2MSAxNC43OTY3ODMyLDE3LjY1MzQ2MzQgMCwwIEM1LjUxMDgzMjExLDE1Ljg0MDY4MjkgMTUuNzgxNTM4OSwyOS41NjY3NzMyIDI5LjM5MDQ5NDcsMzkuMjc4NDE3MSBDNDIuOTk5Nyw0OC45ODk4NTM3IDU5LjI3MzcsNTQuMjA2NzgwNSA3NS45NjA1Nzg5LDU0LjIwNjc4MDUgQzkyLjY0NzQ1NzksNTQuMjA2NzgwNSAxMDguOTIxNDU4LDQ4Ljk4OTg1MzcgMTIyLjUzMDY2MywzOS4yNzg0MTcxIEMxMzYuMTM5NDUzLDI5LjU2Njc3MzIgMTQ2LjQxMDI4NCwxNS44NDA2ODI5IDE1MS45MjExNTgsMCBDMTM3LjA4Nzg2OCwxNy42NTM0NjM0IDEwOC41ODI1ODksMjkuNTgwNDU2MSA3NS45NDIyODQyLDI5LjU4MDQ1NjEgTDc1Ljk0MjI4NDIsMjkuNTgwNDU2MSBaIiAvPgogICAgPHBhdGggdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMzczNjgsIDAuNzA0ODc4KSIgZD0iTTc1Ljk3ODQ1NzksMjQuNjI2NDA3MyBDMTA4LjYxODc2MywyNC42MjY0MDczIDEzNy4xMjQ0NTgsMzYuNTUzNDQxNSAxNTEuOTIxMTU4LDU0LjIwNjc4MDUgQzE0Ni40MTAyODQsMzguMzY2MjIyIDEzNi4xMzk0NTMsMjQuNjQwMTMxNyAxMjIuNTMwNjYzLDE0LjkyODQ4NzggQzEwOC45MjE0NTgsNS4yMTY4NDM5IDkyLjY0NzQ1NzksMCA3NS45NjA1Nzg5LDAgQzU5LjI3MzcsMCA0Mi45OTk3LDUuMjE2ODQzOSAyOS4zOTA0OTQ3LDE0LjkyODQ4NzggQzE1Ljc4MTUzODksMjQuNjQwMTMxNyA1LjUxMDgzMjExLDM4LjM2NjIyMiAwLDU0LjIwNjc4MDUgQzE0LjgzMzA4MTYsMzYuNTg5OTI5MyA0My4zMzg1Njg0LDI0LjYyNjQwNzMgNzUuOTc4NDU3OSwyNC42MjY0MDczIEw3NS45Nzg0NTc5LDI0LjYyNjQwNzMgWiIgLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-jupyter: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzkiIGhlaWdodD0iNTEiIHZpZXdCb3g9IjAgMCAzOSA1MSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgtMTYzOCAtMjI4MSkiPgogICAgIDxnIGNsYXNzPSJqcC1qdXB5dGVyLWljb24tY29sb3IiIGZpbGw9IiNGMzc3MjYiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5Ljc0IDIzMTEuOTgpIiBkPSJNIDE4LjI2NDYgNy4xMzQxMUMgMTAuNDE0NSA3LjEzNDExIDMuNTU4NzIgNC4yNTc2IDAgMEMgMS4zMjUzOSAzLjgyMDQgMy43OTU1NiA3LjEzMDgxIDcuMDY4NiA5LjQ3MzAzQyAxMC4zNDE3IDExLjgxNTIgMTQuMjU1NyAxMy4wNzM0IDE4LjI2OSAxMy4wNzM0QyAyMi4yODIzIDEzLjA3MzQgMjYuMTk2MyAxMS44MTUyIDI5LjQ2OTQgOS40NzMwM0MgMzIuNzQyNCA3LjEzMDgxIDM1LjIxMjYgMy44MjA0IDM2LjUzOCAwQyAzMi45NzA1IDQuMjU3NiAyNi4xMTQ4IDcuMTM0MTEgMTguMjY0NiA3LjEzNDExWiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM5LjczIDIyODUuNDgpIiBkPSJNIDE4LjI3MzMgNS45MzkzMUMgMjYuMTIzNSA1LjkzOTMxIDMyLjk3OTMgOC44MTU4MyAzNi41MzggMTMuMDczNEMgMzUuMjEyNiA5LjI1MzAzIDMyLjc0MjQgNS45NDI2MiAyOS40Njk0IDMuNjAwNEMgMjYuMTk2MyAxLjI1ODE4IDIyLjI4MjMgMCAxOC4yNjkgMEMgMTQuMjU1NyAwIDEwLjM0MTcgMS4yNTgxOCA3LjA2ODYgMy42MDA0QyAzLjc5NTU2IDUuOTQyNjIgMS4zMjUzOSA5LjI1MzAzIDAgMTMuMDczNEMgMy41Njc0NSA4LjgyNDYzIDEwLjQyMzIgNS45MzkzMSAxOC4yNzMzIDUuOTM5MzFaIi8+CiAgICA8L2c+CiAgICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjY5LjMgMjI4MS4zMSkiIGQ9Ik0gNS44OTM1MyAyLjg0NEMgNS45MTg4OSAzLjQzMTY1IDUuNzcwODUgNC4wMTM2NyA1LjQ2ODE1IDQuNTE2NDVDIDUuMTY1NDUgNS4wMTkyMiA0LjcyMTY4IDUuNDIwMTUgNC4xOTI5OSA1LjY2ODUxQyAzLjY2NDMgNS45MTY4OCAzLjA3NDQ0IDYuMDAxNTEgMi40OTgwNSA1LjkxMTcxQyAxLjkyMTY2IDUuODIxOSAxLjM4NDYzIDUuNTYxNyAwLjk1NDg5OCA1LjE2NDAxQyAwLjUyNTE3IDQuNzY2MzMgMC4yMjIwNTYgNC4yNDkwMyAwLjA4MzkwMzcgMy42Nzc1N0MgLTAuMDU0MjQ4MyAzLjEwNjExIC0wLjAyMTIzIDIuNTA2MTcgMC4xNzg3ODEgMS45NTM2NEMgMC4zNzg3OTMgMS40MDExIDAuNzM2ODA5IDAuOTIwODE3IDEuMjA3NTQgMC41NzM1MzhDIDEuNjc4MjYgMC4yMjYyNTkgMi4yNDA1NSAwLjAyNzU5MTkgMi44MjMyNiAwLjAwMjY3MjI5QyAzLjYwMzg5IC0wLjAzMDcxMTUgNC4zNjU3MyAwLjI0OTc4OSA0Ljk0MTQyIDAuNzgyNTUxQyA1LjUxNzExIDEuMzE1MzEgNS44NTk1NiAyLjA1Njc2IDUuODkzNTMgMi44NDRaIi8+CiAgICAgIDxwYXRoIHRyYW5zZm9ybT0idHJhbnNsYXRlKDE2MzkuOCAyMzIzLjgxKSIgZD0iTSA3LjQyNzg5IDMuNTgzMzhDIDcuNDYwMDggNC4zMjQzIDcuMjczNTUgNS4wNTgxOSA2Ljg5MTkzIDUuNjkyMTNDIDYuNTEwMzEgNi4zMjYwNyA1Ljk1MDc1IDYuODMxNTYgNS4yODQxMSA3LjE0NDZDIDQuNjE3NDcgNy40NTc2MyAzLjg3MzcxIDcuNTY0MTQgMy4xNDcwMiA3LjQ1MDYzQyAyLjQyMDMyIDcuMzM3MTIgMS43NDMzNiA3LjAwODcgMS4yMDE4NCA2LjUwNjk1QyAwLjY2MDMyOCA2LjAwNTIgMC4yNzg2MSA1LjM1MjY4IDAuMTA1MDE3IDQuNjMyMDJDIC0wLjA2ODU3NTcgMy45MTEzNSAtMC4wMjYyMzYxIDMuMTU0OTQgMC4yMjY2NzUgMi40NTg1NkMgMC40Nzk1ODcgMS43NjIxNyAwLjkzMTY5NyAxLjE1NzEzIDEuNTI1NzYgMC43MjAwMzNDIDIuMTE5ODMgMC4yODI5MzUgMi44MjkxNCAwLjAzMzQzOTUgMy41NjM4OSAwLjAwMzEzMzQ0QyA0LjU0NjY3IC0wLjAzNzQwMzMgNS41MDUyOSAwLjMxNjcwNiA2LjIyOTYxIDAuOTg3ODM1QyA2Ljk1MzkzIDEuNjU4OTYgNy4zODQ4NCAyLjU5MjM1IDcuNDI3ODkgMy41ODMzOEwgNy40Mjc4OSAzLjU4MzM4WiIvPgogICAgICA8cGF0aCB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxNjM4LjM2IDIyODYuMDYpIiBkPSJNIDIuMjc0NzEgNC4zOTYyOUMgMS44NDM2MyA0LjQxNTA4IDEuNDE2NzEgNC4zMDQ0NSAxLjA0Nzk5IDQuMDc4NDNDIDAuNjc5MjY4IDMuODUyNCAwLjM4NTMyOCAzLjUyMTE0IDAuMjAzMzcxIDMuMTI2NTZDIDAuMDIxNDEzNiAyLjczMTk4IC0wLjA0MDM3OTggMi4yOTE4MyAwLjAyNTgxMTYgMS44NjE4MUMgMC4wOTIwMDMxIDEuNDMxOCAwLjI4MzIwNCAxLjAzMTI2IDAuNTc1MjEzIDAuNzEwODgzQyAwLjg2NzIyMiAwLjM5MDUxIDEuMjQ2OTEgMC4xNjQ3MDggMS42NjYyMiAwLjA2MjA1OTJDIDIuMDg1NTMgLTAuMDQwNTg5NyAyLjUyNTYxIC0wLjAxNTQ3MTQgMi45MzA3NiAwLjEzNDIzNUMgMy4zMzU5MSAwLjI4Mzk0MSAzLjY4NzkyIDAuNTUxNTA1IDMuOTQyMjIgMC45MDMwNkMgNC4xOTY1MiAxLjI1NDYyIDQuMzQxNjkgMS42NzQzNiA0LjM1OTM1IDIuMTA5MTZDIDQuMzgyOTkgMi42OTEwNyA0LjE3Njc4IDMuMjU4NjkgMy43ODU5NyAzLjY4NzQ2QyAzLjM5NTE2IDQuMTE2MjQgMi44NTE2NiA0LjM3MTE2IDIuMjc0NzEgNC4zOTYyOUwgMi4yNzQ3MSA0LjM5NjI5WiIvPgogICAgPC9nPgogIDwvZz4+Cjwvc3ZnPgo=);
  --jp-icon-jupyterlab-wordmark: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyMDAiIHZpZXdCb3g9IjAgMCAxODYwLjggNDc1Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0RTRFNEUiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDQ4MC4xMzY0MDEsIDY0LjI3MTQ5MykiPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC4wMDAwMDAsIDU4Ljg3NTU2NikiPgogICAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgwLjA4NzYwMywgMC4xNDAyOTQpIj4KICAgICAgICA8cGF0aCBkPSJNLTQyNi45LDE2OS44YzAsNDguNy0zLjcsNjQuNy0xMy42LDc2LjRjLTEwLjgsMTAtMjUsMTUuNS0zOS43LDE1LjVsMy43LDI5IGMyMi44LDAuMyw0NC44LTcuOSw2MS45LTIzLjFjMTcuOC0xOC41LDI0LTQ0LjEsMjQtODMuM1YwSC00Mjd2MTcwLjFMLTQyNi45LDE2OS44TC00MjYuOSwxNjkuOHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMTU1LjA0NTI5NiwgNTYuODM3MTA0KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuNTYyNDUzLCAxLjc5OTg0MikiPgogICAgICAgIDxwYXRoIGQ9Ik0tMzEyLDE0OGMwLDIxLDAsMzkuNSwxLjcsNTUuNGgtMzEuOGwtMi4xLTMzLjNoLTAuOGMtNi43LDExLjYtMTYuNCwyMS4zLTI4LDI3LjkgYy0xMS42LDYuNi0yNC44LDEwLTM4LjIsOS44Yy0zMS40LDAtNjktMTcuNy02OS04OVYwaDM2LjR2MTEyLjdjMCwzOC43LDExLjYsNjQuNyw0NC42LDY0LjdjMTAuMy0wLjIsMjAuNC0zLjUsMjguOS05LjQgYzguNS01LjksMTUuMS0xNC4zLDE4LjktMjMuOWMyLjItNi4xLDMuMy0xMi41LDMuMy0xOC45VjAuMmgzNi40VjE0OEgtMzEyTC0zMTIsMTQ4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgzOTAuMDEzMzIyLCA1My40Nzk2MzgpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS43MDY0NTgsIDAuMjMxNDI1KSI+CiAgICAgICAgPHBhdGggZD0iTS00NzguNiw3MS40YzAtMjYtMC44LTQ3LTEuNy02Ni43aDMyLjdsMS43LDM0LjhoMC44YzcuMS0xMi41LDE3LjUtMjIuOCwzMC4xLTI5LjcgYzEyLjUtNywyNi43LTEwLjMsNDEtOS44YzQ4LjMsMCw4NC43LDQxLjcsODQuNywxMDMuM2MwLDczLjEtNDMuNywxMDkuMi05MSwxMDkuMmMtMTIuMSwwLjUtMjQuMi0yLjItMzUtNy44IGMtMTAuOC01LjYtMTkuOS0xMy45LTI2LjYtMjQuMmgtMC44VjI5MWgtMzZ2LTIyMEwtNDc4LjYsNzEuNEwtNDc4LjYsNzEuNHogTS00NDIuNiwxMjUuNmMwLjEsNS4xLDAuNiwxMC4xLDEuNywxNS4xIGMzLDEyLjMsOS45LDIzLjMsMTkuOCwzMS4xYzkuOSw3LjgsMjIuMSwxMi4xLDM0LjcsMTIuMWMzOC41LDAsNjAuNy0zMS45LDYwLjctNzguNWMwLTQwLjctMjEuMS03NS42LTU5LjUtNzUuNiBjLTEyLjksMC40LTI1LjMsNS4xLTM1LjMsMTMuNGMtOS45LDguMy0xNi45LDE5LjctMTkuNiwzMi40Yy0xLjUsNC45LTIuMywxMC0yLjUsMTUuMVYxMjUuNkwtNDQyLjYsMTI1LjZMLTQ0Mi42LDEyNS42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSg2MDYuNzQwNzI2LCA1Ni44MzcxMDQpIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMC43NTEyMjYsIDEuOTg5Mjk5KSI+CiAgICAgICAgPHBhdGggZD0iTS00NDAuOCwwbDQzLjcsMTIwLjFjNC41LDEzLjQsOS41LDI5LjQsMTIuOCw0MS43aDAuOGMzLjctMTIuMiw3LjktMjcuNywxMi44LTQyLjQgbDM5LjctMTE5LjJoMzguNUwtMzQ2LjksMTQ1Yy0yNiw2OS43LTQzLjcsMTA1LjQtNjguNiwxMjcuMmMtMTIuNSwxMS43LTI3LjksMjAtNDQuNiwyMy45bC05LjEtMzEuMSBjMTEuNy0zLjksMjIuNS0xMC4xLDMxLjgtMTguMWMxMy4yLTExLjEsMjMuNy0yNS4yLDMwLjYtNDEuMmMxLjUtMi44LDIuNS01LjcsMi45LTguOGMtMC4zLTMuMy0xLjItNi42LTIuNS05LjdMLTQ4MC4yLDAuMSBoMzkuN0wtNDQwLjgsMEwtNDQwLjgsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoODIyLjc0ODEwNCwgMC4wMDAwMDApIj4KICAgICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoMS40NjQwNTAsIDAuMzc4OTE0KSI+CiAgICAgICAgPHBhdGggZD0iTS00MTMuNywwdjU4LjNoNTJ2MjguMmgtNTJWMTk2YzAsMjUsNywzOS41LDI3LjMsMzkuNWM3LjEsMC4xLDE0LjItMC43LDIxLjEtMi41IGwxLjcsMjcuN2MtMTAuMywzLjctMjEuMyw1LjQtMzIuMiw1Yy03LjMsMC40LTE0LjYtMC43LTIxLjMtMy40Yy02LjgtMi43LTEyLjktNi44LTE3LjktMTIuMWMtMTAuMy0xMC45LTE0LjEtMjktMTQuMS01Mi45IFY4Ni41aC0zMVY1OC4zaDMxVjkuNkwtNDEzLjcsMEwtNDEzLjcsMHoiLz4KICAgICAgPC9nPgogICAgPC9nPgogICAgPGcgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOTc0LjQzMzI4NiwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDAuOTkwMDM0LCAwLjYxMDMzOSkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDQ1LjgsMTEzYzAuOCw1MCwzMi4yLDcwLjYsNjguNiw3MC42YzE5LDAuNiwzNy45LTMsNTUuMy0xMC41bDYuMiwyNi40IGMtMjAuOSw4LjktNDMuNSwxMy4xLTY2LjIsMTIuNmMtNjEuNSwwLTk4LjMtNDEuMi05OC4zLTEwMi41Qy00ODAuMiw0OC4yLTQ0NC43LDAtMzg2LjUsMGM2NS4yLDAsODIuNyw1OC4zLDgyLjcsOTUuNyBjLTAuMSw1LjgtMC41LDExLjUtMS4yLDE3LjJoLTE0MC42SC00NDUuOEwtNDQ1LjgsMTEzeiBNLTMzOS4yLDg2LjZjMC40LTIzLjUtOS41LTYwLjEtNTAuNC02MC4xIGMtMzYuOCwwLTUyLjgsMzQuNC01NS43LDYwLjFILTMzOS4yTC0zMzkuMiw4Ni42TC0zMzkuMiw4Ni42eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgICA8ZyB0cmFuc2Zvcm09InRyYW5zbGF0ZSgxMjAxLjk2MTA1OCwgNTMuNDc5NjM4KSI+CiAgICAgIDxnIHRyYW5zZm9ybT0idHJhbnNsYXRlKDEuMTc5NjQwLCAwLjcwNTA2OCkiPgogICAgICAgIDxwYXRoIGQ9Ik0tNDc4LjYsNjhjMC0yMy45LTAuNC00NC41LTEuNy02My40aDMxLjhsMS4yLDM5LjloMS43YzkuMS0yNy4zLDMxLTQ0LjUsNTUuMy00NC41IGMzLjUtMC4xLDcsMC40LDEwLjMsMS4ydjM0LjhjLTQuMS0wLjktOC4yLTEuMy0xMi40LTEuMmMtMjUuNiwwLTQzLjcsMTkuNy00OC43LDQ3LjRjLTEsNS43LTEuNiwxMS41LTEuNywxNy4ydjEwOC4zaC0zNlY2OCBMLTQ3OC42LDY4eiIvPgogICAgICA8L2c+CiAgICA8L2c+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi13YXJuMCIgZmlsbD0iI0YzNzcyNiI+CiAgICA8cGF0aCBkPSJNMTM1Mi4zLDMyNi4yaDM3VjI4aC0zN1YzMjYuMnogTTE2MDQuOCwzMjYuMmMtMi41LTEzLjktMy40LTMxLjEtMy40LTQ4Ljd2LTc2IGMwLTQwLjctMTUuMS04My4xLTc3LjMtODMuMWMtMjUuNiwwLTUwLDcuMS02Ni44LDE4LjFsOC40LDI0LjRjMTQuMy05LjIsMzQtMTUuMSw1My0xNS4xYzQxLjYsMCw0Ni4yLDMwLjIsNDYuMiw0N3Y0LjIgYy03OC42LTAuNC0xMjIuMywyNi41LTEyMi4zLDc1LjZjMCwyOS40LDIxLDU4LjQsNjIuMiw1OC40YzI5LDAsNTAuOS0xNC4zLDYyLjItMzAuMmgxLjNsMi45LDI1LjZIMTYwNC44eiBNMTU2NS43LDI1Ny43IGMwLDMuOC0wLjgsOC0yLjEsMTEuOGMtNS45LDE3LjItMjIuNywzNC00OS4yLDM0Yy0xOC45LDAtMzQuOS0xMS4zLTM0LjktMzUuM2MwLTM5LjUsNDUuOC00Ni42LDg2LjItNDUuOFYyNTcuN3ogTTE2OTguNSwzMjYuMiBsMS43LTMzLjZoMS4zYzE1LjEsMjYuOSwzOC43LDM4LjIsNjguMSwzOC4yYzQ1LjQsMCw5MS4yLTM2LjEsOTEuMi0xMDguOGMwLjQtNjEuNy0zNS4zLTEwMy43LTg1LjctMTAzLjcgYy0zMi44LDAtNTYuMywxNC43LTY5LjMsMzcuNGgtMC44VjI4aC0zNi42djI0NS43YzAsMTguMS0wLjgsMzguNi0xLjcsNTIuNUgxNjk4LjV6IE0xNzA0LjgsMjA4LjJjMC01LjksMS4zLTEwLjksMi4xLTE1LjEgYzcuNi0yOC4xLDMxLjEtNDUuNCw1Ni4zLTQ1LjRjMzkuNSwwLDYwLjUsMzQuOSw2MC41LDc1LjZjMCw0Ni42LTIzLjEsNzguMS02MS44LDc4LjFjLTI2LjksMC00OC4zLTE3LjYtNTUuNS00My4zIGMtMC44LTQuMi0xLjctOC44LTEuNy0xMy40VjIwOC4yeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzYxNjE2MSIgZD0iTTE1IDlIOXY2aDZWOXptLTIgNGgtMnYtMmgydjJ6bTgtMlY5aC0yVjdjMC0xLjEtLjktMi0yLTJoLTJWM2gtMnYyaC0yVjNIOXYySDdjLTEuMSAwLTIgLjktMiAydjJIM3YyaDJ2MkgzdjJoMnYyYzAgMS4xLjkgMiAyIDJoMnYyaDJ2LTJoMnYyaDJ2LTJoMmMxLjEgMCAyLS45IDItMnYtMmgydi0yaC0ydi0yaDJ6bS00IDZIN1Y3aDEwdjEweiIvPgo8L3N2Zz4K);
  --jp-icon-keyboard: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMjAgNUg0Yy0xLjEgMC0xLjk5LjktMS45OSAyTDIgMTdjMCAxLjEuOSAyIDIgMmgxNmMxLjEgMCAyLS45IDItMlY3YzAtMS4xLS45LTItMi0yem0tOSAzaDJ2MmgtMlY4em0wIDNoMnYyaC0ydi0yek04IDhoMnYySDhWOHptMCAzaDJ2Mkg4di0yem0tMSAySDV2LTJoMnYyem0wLTNINVY4aDJ2MnptOSA3SDh2LTJoOHYyem0wLTRoLTJ2LTJoMnYyem0wLTNoLTJWOGgydjJ6bTMgM2gtMnYtMmgydjJ6bTAtM2gtMlY4aDJ2MnoiLz4KPC9zdmc+Cg==);
  --jp-icon-launch: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMzIgMzIiIHdpZHRoPSIzMiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik0yNiwyOEg2YTIuMDAyNywyLjAwMjcsMCwwLDEtMi0yVjZBMi4wMDI3LDIuMDAyNywwLDAsMSw2LDRIMTZWNkg2VjI2SDI2VjE2aDJWMjZBMi4wMDI3LDIuMDAyNywwLDAsMSwyNiwyOFoiLz4KICAgIDxwb2x5Z29uIHBvaW50cz0iMjAgMiAyMCA0IDI2LjU4NiA0IDE4IDEyLjU4NiAxOS40MTQgMTQgMjggNS40MTQgMjggMTIgMzAgMTIgMzAgMiAyMCAyIi8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-launcher: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkgMTlINVY1aDdWM0g1YTIgMiAwIDAwLTIgMnYxNGEyIDIgMCAwMDIgMmgxNGMxLjEgMCAyLS45IDItMnYtN2gtMnY3ek0xNCAzdjJoMy41OWwtOS44MyA5LjgzIDEuNDEgMS40MUwxOSA2LjQxVjEwaDJWM2gtN3oiLz4KPC9zdmc+Cg==);
  --jp-icon-line-form: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGZpbGw9IndoaXRlIiBkPSJNNS44OCA0LjEyTDEzLjc2IDEybC03Ljg4IDcuODhMOCAyMmwxMC0xMEw4IDJ6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-link: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTMuOSAxMmMwLTEuNzEgMS4zOS0zLjEgMy4xLTMuMWg0VjdIN2MtMi43NiAwLTUgMi4yNC01IDVzMi4yNCA1IDUgNWg0di0xLjlIN2MtMS43MSAwLTMuMS0xLjM5LTMuMS0zLjF6TTggMTNoOHYtMkg4djJ6bTktNmgtNHYxLjloNGMxLjcxIDAgMy4xIDEuMzkgMy4xIDMuMXMtMS4zOSAzLjEtMy4xIDMuMWgtNFYxN2g0YzIuNzYgMCA1LTIuMjQgNS01cy0yLjI0LTUtNS01eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-list: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xOSA1djE0SDVWNWgxNG0xLjEtMkgzLjljLS41IDAtLjkuNC0uOS45djE2LjJjMCAuNC40LjkuOS45aDE2LjJjLjQgMCAuOS0uNS45LS45VjMuOWMwLS41LS41LS45LS45LS45ek0xMSA3aDZ2MmgtNlY3em0wIDRoNnYyaC02di0yem0wIDRoNnYyaC02ek03IDdoMnYySDd6bTAgNGgydjJIN3ptMCA0aDJ2Mkg3eiIvPgo8L3N2Zz4K);
  --jp-icon-markdown: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDAganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjN0IxRkEyIiBkPSJNNSAxNC45aDEybC02LjEgNnptOS40LTYuOGMwLTEuMy0uMS0yLjktLjEtNC41LS40IDEuNC0uOSAyLjktMS4zIDQuM2wtMS4zIDQuM2gtMkw4LjUgNy45Yy0uNC0xLjMtLjctMi45LTEtNC4zLS4xIDEuNi0uMSAzLjItLjIgNC42TDcgMTIuNEg0LjhsLjctMTFoMy4zTDEwIDVjLjQgMS4yLjcgMi43IDEgMy45LjMtMS4yLjctMi42IDEtMy45bDEuMi0zLjdoMy4zbC42IDExaC0yLjRsLS4zLTQuMnoiLz4KPC9zdmc+Cg==);
  --jp-icon-move-down: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMTIuNDcxIDcuNTI4OTlDMTIuNzYzMiA3LjIzNjg0IDEyLjc2MzIgNi43NjMxNiAxMi40NzEgNi40NzEwMVY2LjQ3MTAxQzEyLjE3OSA2LjE3OTA1IDExLjcwNTcgNi4xNzg4NCAxMS40MTM1IDYuNDcwNTRMNy43NSAxMC4xMjc1VjEuNzVDNy43NSAxLjMzNTc5IDcuNDE0MjEgMSA3IDFWMUM2LjU4NTc5IDEgNi4yNSAxLjMzNTc5IDYuMjUgMS43NVYxMC4xMjc1TDIuNTk3MjYgNi40NjgyMkMyLjMwMzM4IDYuMTczODEgMS44MjY0MSA2LjE3MzU5IDEuNTMyMjYgNi40Njc3NFY2LjQ2Nzc0QzEuMjM4MyA2Ljc2MTcgMS4yMzgzIDcuMjM4MyAxLjUzMjI2IDcuNTMyMjZMNi4yOTI4OSAxMi4yOTI5QzYuNjgzNDIgMTIuNjgzNCA3LjMxNjU4IDEyLjY4MzQgNy43MDcxMSAxMi4yOTI5TDEyLjQ3MSA3LjUyODk5WiIgZmlsbD0iIzYxNjE2MSIvPgo8L3N2Zz4K);
  --jp-icon-move-up: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTQiIGhlaWdodD0iMTQiIHZpZXdCb3g9IjAgMCAxNCAxNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPHBhdGggY2xhc3M9ImpwLWljb24zIiBkPSJNMS41Mjg5OSA2LjQ3MTAxQzEuMjM2ODQgNi43NjMxNiAxLjIzNjg0IDcuMjM2ODQgMS41Mjg5OSA3LjUyODk5VjcuNTI4OTlDMS44MjA5NSA3LjgyMDk1IDIuMjk0MjYgNy44MjExNiAyLjU4NjQ5IDcuNTI5NDZMNi4yNSAzLjg3MjVWMTIuMjVDNi4yNSAxMi42NjQyIDYuNTg1NzkgMTMgNyAxM1YxM0M3LjQxNDIxIDEzIDcuNzUgMTIuNjY0MiA3Ljc1IDEyLjI1VjMuODcyNUwxMS40MDI3IDcuNTMxNzhDMTEuNjk2NiA3LjgyNjE5IDEyLjE3MzYgNy44MjY0MSAxMi40Njc3IDcuNTMyMjZWNy41MzIyNkMxMi43NjE3IDcuMjM4MyAxMi43NjE3IDYuNzYxNyAxMi40Njc3IDYuNDY3NzRMNy43MDcxMSAxLjcwNzExQzcuMzE2NTggMS4zMTY1OCA2LjY4MzQyIDEuMzE2NTggNi4yOTI4OSAxLjcwNzExTDEuNTI4OTkgNi40NzEwMVoiIGZpbGw9IiM2MTYxNjEiLz4KPC9zdmc+Cg==);
  --jp-icon-new-folder: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIwIDZoLThsLTItMkg0Yy0xLjExIDAtMS45OS44OS0xLjk5IDJMMiAxOGMwIDEuMTEuODkgMiAyIDJoMTZjMS4xMSAwIDItLjg5IDItMlY4YzAtMS4xMS0uODktMi0yLTJ6bS0xIDhoLTN2M2gtMnYtM2gtM3YtMmgzVjloMnYzaDN2MnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-not-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI1IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMTkgMTcuMTg0NCAyLjk2OTY4IDE0LjMwMzIgMS44NjA5NCAxMS40NDA5WiIvPgogICAgPHBhdGggY2xhc3M9ImpwLWljb24yIiBzdHJva2U9IiMzMzMzMzMiIHN0cm9rZS13aWR0aD0iMiIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOS4zMTU5MiA5LjMyMDMxKSIgZD0iTTcuMzY4NDIgMEwwIDcuMzY0NzkiLz4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDkuMzE1OTIgMTYuNjgzNikgc2NhbGUoMSAtMSkiIGQ9Ik03LjM2ODQyIDBMMCA3LjM2NDc5Ii8+Cjwvc3ZnPgo=);
  --jp-icon-notebook: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtbm90ZWJvb2staWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiNFRjZDMDAiPgogICAgPHBhdGggZD0iTTE4LjcgMy4zdjE1LjRIMy4zVjMuM2gxNS40bTEuNS0xLjVIMS44djE4LjNoMTguM2wuMS0xOC4zeiIvPgogICAgPHBhdGggZD0iTTE2LjUgMTYuNWwtNS40LTQuMy01LjYgNC4zdi0xMWgxMXoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-numbering: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjIiIGhlaWdodD0iMjIiIHZpZXdCb3g9IjAgMCAyOCAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTQgMTlINlYxOS41SDVWMjAuNUg2VjIxSDRWMjJIN1YxOEg0VjE5Wk01IDEwSDZWNkg0VjdINVYxMFpNNCAxM0g1LjhMNCAxNS4xVjE2SDdWMTVINS4yTDcgMTIuOVYxMkg0VjEzWk05IDdWOUgyM1Y3SDlaTTkgMjFIMjNWMTlIOVYyMVpNOSAxNUgyM1YxM0g5VjE1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-offline-bolt: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyIDIuMDJjLTUuNTEgMC05Ljk4IDQuNDctOS45OCA5Ljk4czQuNDcgOS45OCA5Ljk4IDkuOTggOS45OC00LjQ3IDkuOTgtOS45OFMxNy41MSAyLjAyIDEyIDIuMDJ6TTExLjQ4IDIwdi02LjI2SDhMMTMgNHY2LjI2aDMuMzVMMTEuNDggMjB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-palette: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE4IDEzVjIwSDRWNkg5LjAyQzkuMDcgNS4yOSA5LjI0IDQuNjIgOS41IDRINEMyLjkgNCAyIDQuOSAyIDZWMjBDMiAyMS4xIDIuOSAyMiA0IDIySDE4QzE5LjEgMjIgMjAgMjEuMSAyMCAyMFYxNUwxOCAxM1pNMTkuMyA4Ljg5QzE5Ljc0IDguMTkgMjAgNy4zOCAyMCA2LjVDMjAgNC4wMSAxNy45OSAyIDE1LjUgMkMxMy4wMSAyIDExIDQuMDEgMTEgNi41QzExIDguOTkgMTMuMDEgMTEgMTUuNDkgMTFDMTYuMzcgMTEgMTcuMTkgMTAuNzQgMTcuODggMTAuM0wyMSAxMy40MkwyMi40MiAxMkwxOS4zIDguODlaTTE1LjUgOUMxNC4xMiA5IDEzIDcuODggMTMgNi41QzEzIDUuMTIgMTQuMTIgNCAxNS41IDRDMTYuODggNCAxOCA1LjEyIDE4IDYuNUMxOCA3Ljg4IDE2Ljg4IDkgMTUuNSA5WiIvPgogICAgPHBhdGggZmlsbC1ydWxlPSJldmVub2RkIiBjbGlwLXJ1bGU9ImV2ZW5vZGQiIGQ9Ik00IDZIOS4wMTg5NEM5LjAwNjM5IDYuMTY1MDIgOSA2LjMzMTc2IDkgNi41QzkgOC44MTU3NyAxMC4yMTEgMTAuODQ4NyAxMi4wMzQzIDEySDlWMTRIMTZWMTIuOTgxMUMxNi41NzAzIDEyLjkzNzcgMTcuMTIgMTIuODIwNyAxNy42Mzk2IDEyLjYzOTZMMTggMTNWMjBINFY2Wk04IDhINlYxMEg4VjhaTTYgMTJIOFYxNEg2VjEyWk04IDE2SDZWMThIOFYxNlpNOSAxNkgxNlYxOEg5VjE2WiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-paste: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE5IDJoLTQuMThDMTQuNC44NCAxMy4zIDAgMTIgMGMtMS4zIDAtMi40Ljg0LTIuODIgMkg1Yy0xLjEgMC0yIC45LTIgMnYxNmMwIDEuMS45IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjRjMC0xLjEtLjktMi0yLTJ6bS03IDBjLjU1IDAgMSAuNDUgMSAxcy0uNDUgMS0xIDEtMS0uNDUtMS0xIC40NS0xIDEtMXptNyAxOEg1VjRoMnYzaDEwVjRoMnYxNnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-pdf: url(data:image/svg+xml;base64,PHN2ZwogICB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyMiAyMiIgd2lkdGg9IjE2Ij4KICAgIDxwYXRoIHRyYW5zZm9ybT0icm90YXRlKDQ1KSIgY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI0ZGMkEyQSIKICAgICAgIGQ9Im0gMjIuMzQ0MzY5LC0zLjAxNjM2NDIgaCA1LjYzODYwNCB2IDEuNTc5MjQzMyBoIC0zLjU0OTIyNyB2IDEuNTA4NjkyOTkgaCAzLjMzNzU3NiBWIDEuNjUwODE1NCBoIC0zLjMzNzU3NiB2IDMuNDM1MjYxMyBoIC0yLjA4OTM3NyB6IG0gLTcuMTM2NDQ0LDEuNTc5MjQzMyB2IDQuOTQzOTU0MyBoIDAuNzQ4OTIgcSAxLjI4MDc2MSwwIDEuOTUzNzAzLC0wLjYzNDk1MzUgMC42NzgzNjksLTAuNjM0OTUzNSAwLjY3ODM2OSwtMS44NDUxNjQxIDAsLTEuMjA0NzgzNTUgLTAuNjcyOTQyLC0xLjgzNDMxMDExIC0wLjY3Mjk0MiwtMC42Mjk1MjY1OSAtMS45NTkxMywtMC42Mjk1MjY1OSB6IG0gLTIuMDg5Mzc3LC0xLjU3OTI0MzMgaCAyLjIwMzM0MyBxIDEuODQ1MTY0LDAgMi43NDYwMzksMC4yNjU5MjA3IDAuOTA2MzAxLDAuMjYwNDkzNyAxLjU1MjEwOCwwLjg5MDAyMDMgMC41Njk4MywwLjU0ODEyMjMgMC44NDY2MDUsMS4yNjQ0ODAwNiAwLjI3Njc3NCwwLjcxNjM1NzgxIDAuMjc2Nzc0LDEuNjIyNjU4OTQgMCwwLjkxNzE1NTEgLTAuMjc2Nzc0LDEuNjM4OTM5OSAtMC4yNzY3NzUsMC43MTYzNTc4IC0wLjg0NjYwNSwxLjI2NDQ4IC0wLjY1MTIzNCwwLjYyOTUyNjYgLTEuNTYyOTYyLDAuODk1NDQ3MyAtMC45MTE3MjgsMC4yNjA0OTM3IC0yLjczNTE4NSwwLjI2MDQ5MzcgaCAtMi4yMDMzNDMgeiBtIC04LjE0NTg1NjUsMCBoIDMuNDY3ODIzIHEgMS41NDY2ODE2LDAgMi4zNzE1Nzg1LDAuNjg5MjIzIDAuODMwMzI0LDAuNjgzNzk2MSAwLjgzMDMyNCwxLjk1MzcwMzE0IDAsMS4yNzUzMzM5NyAtMC44MzAzMjQsMS45NjQ1NTcwNiBRIDkuOTg3MTk2MSwyLjI3NDkxNSA4LjQ0MDUxNDUsMi4yNzQ5MTUgSCA3LjA2MjA2ODQgViA1LjA4NjA3NjcgSCA0Ljk3MjY5MTUgWiBtIDIuMDg5Mzc2OSwxLjUxNDExOTkgdiAyLjI2MzAzOTQzIGggMS4xNTU5NDEgcSAwLjYwNzgxODgsMCAwLjkzODg2MjksLTAuMjkzMDU1NDcgMC4zMzEwNDQxLC0wLjI5ODQ4MjQxIDAuMzMxMDQ0MSwtMC44NDExNzc3MiAwLC0wLjU0MjY5NTMxIC0wLjMzMTA0NDEsLTAuODM1NzUwNzQgLTAuMzMxMDQ0MSwtMC4yOTMwNTU1IC0wLjkzODg2MjksLTAuMjkzMDU1NSB6IgovPgo8L3N2Zz4K);
  --jp-icon-python: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iLTEwIC0xMCAxMzEuMTYxMzYxNjk0MzM1OTQgMTMyLjM4ODk5OTkzODk2NDg0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMzA2OTk4IiBkPSJNIDU0LjkxODc4NSw5LjE5Mjc0MjFlLTQgQyA1MC4zMzUxMzIsMC4wMjIyMTcyNyA0NS45NTc4NDYsMC40MTMxMzY5NyA0Mi4xMDYyODUsMS4wOTQ2NjkzIDMwLjc2MDA2OSwzLjA5OTE3MzEgMjguNzAwMDM2LDcuMjk0NzcxNCAyOC43MDAwMzUsMTUuMDMyMTY5IHYgMTAuMjE4NzUgaCAyNi44MTI1IHYgMy40MDYyNSBoIC0yNi44MTI1IC0xMC4wNjI1IGMgLTcuNzkyNDU5LDAgLTE0LjYxNTc1ODgsNC42ODM3MTcgLTE2Ljc0OTk5OTgsMTMuNTkzNzUgLTIuNDYxODE5OTgsMTAuMjEyOTY2IC0yLjU3MTAxNTA4LDE2LjU4NjAyMyAwLDI3LjI1IDEuOTA1OTI4Myw3LjkzNzg1MiA2LjQ1NzU0MzIsMTMuNTkzNzQ4IDE0LjI0OTk5OTgsMTMuNTkzNzUgaCA5LjIxODc1IHYgLTEyLjI1IGMgMCwtOC44NDk5MDIgNy42NTcxNDQsLTE2LjY1NjI0OCAxNi43NSwtMTYuNjU2MjUgaCAyNi43ODEyNSBjIDcuNDU0OTUxLDAgMTMuNDA2MjUzLC02LjEzODE2NCAxMy40MDYyNSwtMTMuNjI1IHYgLTI1LjUzMTI1IGMgMCwtNy4yNjYzMzg2IC02LjEyOTk4LC0xMi43MjQ3NzcxIC0xMy40MDYyNSwtMTMuOTM3NDk5NyBDIDY0LjI4MTU0OCwwLjMyNzk0Mzk3IDU5LjUwMjQzOCwtMC4wMjAzNzkwMyA1NC45MTg3ODUsOS4xOTI3NDIxZS00IFogbSAtMTQuNSw4LjIxODc1MDEyNTc5IGMgMi43Njk1NDcsMCA1LjAzMTI1LDIuMjk4NjQ1NiA1LjAzMTI1LDUuMTI0OTk5NiAtMmUtNiwyLjgxNjMzNiAtMi4yNjE3MDMsNS4wOTM3NSAtNS4wMzEyNSw1LjA5Mzc1IC0yLjc3OTQ3NiwtMWUtNiAtNS4wMzEyNSwtMi4yNzc0MTUgLTUuMDMxMjUsLTUuMDkzNzUgLTEwZS03LC0yLjgyNjM1MyAyLjI1MTc3NCwtNS4xMjQ5OTk2IDUuMDMxMjUsLTUuMTI0OTk5NiB6Ii8+CiAgPHBhdGggY2xhc3M9ImpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iI2ZmZDQzYiIgZD0ibSA4NS42Mzc1MzUsMjguNjU3MTY5IHYgMTEuOTA2MjUgYyAwLDkuMjMwNzU1IC03LjgyNTg5NSwxNi45OTk5OTkgLTE2Ljc1LDE3IGggLTI2Ljc4MTI1IGMgLTcuMzM1ODMzLDAgLTEzLjQwNjI0OSw2LjI3ODQ4MyAtMTMuNDA2MjUsMTMuNjI1IHYgMjUuNTMxMjQ3IGMgMCw3LjI2NjM0NCA2LjMxODU4OCwxMS41NDAzMjQgMTMuNDA2MjUsMTMuNjI1MDA0IDguNDg3MzMxLDIuNDk1NjEgMTYuNjI2MjM3LDIuOTQ2NjMgMjYuNzgxMjUsMCA2Ljc1MDE1NSwtMS45NTQzOSAxMy40MDYyNTMsLTUuODg3NjEgMTMuNDA2MjUsLTEzLjYyNTAwNCBWIDg2LjUwMDkxOSBoIC0yNi43ODEyNSB2IC0zLjQwNjI1IGggMjYuNzgxMjUgMTMuNDA2MjU0IGMgNy43OTI0NjEsMCAxMC42OTYyNTEsLTUuNDM1NDA4IDEzLjQwNjI0MSwtMTMuNTkzNzUgMi43OTkzMywtOC4zOTg4ODYgMi42ODAyMiwtMTYuNDc1Nzc2IDAsLTI3LjI1IC0xLjkyNTc4LC03Ljc1NzQ0MSAtNS42MDM4NywtMTMuNTkzNzUgLTEzLjQwNjI0MSwtMTMuNTkzNzUgeiBtIC0xNS4wNjI1LDY0LjY1NjI1IGMgMi43Nzk0NzgsM2UtNiA1LjAzMTI1LDIuMjc3NDE3IDUuMDMxMjUsNS4wOTM3NDcgLTJlLTYsMi44MjYzNTQgLTIuMjUxNzc1LDUuMTI1MDA0IC01LjAzMTI1LDUuMTI1MDA0IC0yLjc2OTU1LDAgLTUuMDMxMjUsLTIuMjk4NjUgLTUuMDMxMjUsLTUuMTI1MDA0IDJlLTYsLTIuODE2MzMgMi4yNjE2OTcsLTUuMDkzNzQ3IDUuMDMxMjUsLTUuMDkzNzQ3IHoiLz4KPC9zdmc+Cg==);
  --jp-icon-r-kernel: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjE5NkYzIiBkPSJNNC40IDIuNWMxLjItLjEgMi45LS4zIDQuOS0uMyAyLjUgMCA0LjEuNCA1LjIgMS4zIDEgLjcgMS41IDEuOSAxLjUgMy41IDAgMi0xLjQgMy41LTIuOSA0LjEgMS4yLjQgMS43IDEuNiAyLjIgMyAuNiAxLjkgMSAzLjkgMS4zIDQuNmgtMy44Yy0uMy0uNC0uOC0xLjctMS4yLTMuN3MtMS4yLTIuNi0yLjYtMi42aC0uOXY2LjRINC40VjIuNXptMy43IDYuOWgxLjRjMS45IDAgMi45LS45IDIuOS0yLjNzLTEtMi4zLTIuOC0yLjNjLS43IDAtMS4zIDAtMS42LjJ2NC41aC4xdi0uMXoiLz4KPC9zdmc+Cg==);
  --jp-icon-react: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMTUwIDE1MCA1NDEuOSAyOTUuMyI+CiAgPGcgY2xhc3M9ImpwLWljb24tYnJhbmQyIGpwLWljb24tc2VsZWN0YWJsZSIgZmlsbD0iIzYxREFGQiI+CiAgICA8cGF0aCBkPSJNNjY2LjMgMjk2LjVjMC0zMi41LTQwLjctNjMuMy0xMDMuMS04Mi40IDE0LjQtNjMuNiA4LTExNC4yLTIwLjItMTMwLjQtNi41LTMuOC0xNC4xLTUuNi0yMi40LTUuNnYyMi4zYzQuNiAwIDguMy45IDExLjQgMi42IDEzLjYgNy44IDE5LjUgMzcuNSAxNC45IDc1LjctMS4xIDkuNC0yLjkgMTkuMy01LjEgMjkuNC0xOS42LTQuOC00MS04LjUtNjMuNS0xMC45LTEzLjUtMTguNS0yNy41LTM1LjMtNDEuNi01MCAzMi42LTMwLjMgNjMuMi00Ni45IDg0LTQ2LjlWNzhjLTI3LjUgMC02My41IDE5LjYtOTkuOSA1My42LTM2LjQtMzMuOC03Mi40LTUzLjItOTkuOS01My4ydjIyLjNjMjAuNyAwIDUxLjQgMTYuNSA4NCA0Ni42LTE0IDE0LjctMjggMzEuNC00MS4zIDQ5LjktMjIuNiAyLjQtNDQgNi4xLTYzLjYgMTEtMi4zLTEwLTQtMTkuNy01LjItMjktNC43LTM4LjIgMS4xLTY3LjkgMTQuNi03NS44IDMtMS44IDYuOS0yLjYgMTEuNS0yLjZWNzguNWMtOC40IDAtMTYgMS44LTIyLjYgNS42LTI4LjEgMTYuMi0zNC40IDY2LjctMTkuOSAxMzAuMS02Mi4yIDE5LjItMTAyLjcgNDkuOS0xMDIuNyA4Mi4zIDAgMzIuNSA0MC43IDYzLjMgMTAzLjEgODIuNC0xNC40IDYzLjYtOCAxMTQuMiAyMC4yIDEzMC40IDYuNSAzLjggMTQuMSA1LjYgMjIuNSA1LjYgMjcuNSAwIDYzLjUtMTkuNiA5OS45LTUzLjYgMzYuNCAzMy44IDcyLjQgNTMuMiA5OS45IDUzLjIgOC40IDAgMTYtMS44IDIyLjYtNS42IDI4LjEtMTYuMiAzNC40LTY2LjcgMTkuOS0xMzAuMSA2Mi0xOS4xIDEwMi41LTQ5LjkgMTAyLjUtODIuM3ptLTEzMC4yLTY2LjdjLTMuNyAxMi45LTguMyAyNi4yLTEzLjUgMzkuNS00LjEtOC04LjQtMTYtMTMuMS0yNC00LjYtOC05LjUtMTUuOC0xNC40LTIzLjQgMTQuMiAyLjEgMjcuOSA0LjcgNDEgNy45em0tNDUuOCAxMDYuNWMtNy44IDEzLjUtMTUuOCAyNi4zLTI0LjEgMzguMi0xNC45IDEuMy0zMCAyLTQ1LjIgMi0xNS4xIDAtMzAuMi0uNy00NS0xLjktOC4zLTExLjktMTYuNC0yNC42LTI0LjItMzgtNy42LTEzLjEtMTQuNS0yNi40LTIwLjgtMzkuOCA2LjItMTMuNCAxMy4yLTI2LjggMjAuNy0zOS45IDcuOC0xMy41IDE1LjgtMjYuMyAyNC4xLTM4LjIgMTQuOS0xLjMgMzAtMiA0NS4yLTIgMTUuMSAwIDMwLjIuNyA0NSAxLjkgOC4zIDExLjkgMTYuNCAyNC42IDI0LjIgMzggNy42IDEzLjEgMTQuNSAyNi40IDIwLjggMzkuOC02LjMgMTMuNC0xMy4yIDI2LjgtMjAuNyAzOS45em0zMi4zLTEzYzUuNCAxMy40IDEwIDI2LjggMTMuOCAzOS44LTEzLjEgMy4yLTI2LjkgNS45LTQxLjIgOCA0LjktNy43IDkuOC0xNS42IDE0LjQtMjMuNyA0LjYtOCA4LjktMTYuMSAxMy0yNC4xek00MjEuMiA0MzBjLTkuMy05LjYtMTguNi0yMC4zLTI3LjgtMzIgOSAuNCAxOC4yLjcgMjcuNS43IDkuNCAwIDE4LjctLjIgMjcuOC0uNy05IDExLjctMTguMyAyMi40LTI3LjUgMzJ6bS03NC40LTU4LjljLTE0LjItMi4xLTI3LjktNC43LTQxLTcuOSAzLjctMTIuOSA4LjMtMjYuMiAxMy41LTM5LjUgNC4xIDggOC40IDE2IDEzLjEgMjQgNC43IDggOS41IDE1LjggMTQuNCAyMy40ek00MjAuNyAxNjNjOS4zIDkuNiAxOC42IDIwLjMgMjcuOCAzMi05LS40LTE4LjItLjctMjcuNS0uNy05LjQgMC0xOC43LjItMjcuOC43IDktMTEuNyAxOC4zLTIyLjQgMjcuNS0zMnptLTc0IDU4LjljLTQuOSA3LjctOS44IDE1LjYtMTQuNCAyMy43LTQuNiA4LTguOSAxNi0xMyAyNC01LjQtMTMuNC0xMC0yNi44LTEzLjgtMzkuOCAxMy4xLTMuMSAyNi45LTUuOCA0MS4yLTcuOXptLTkwLjUgMTI1LjJjLTM1LjQtMTUuMS01OC4zLTM0LjktNTguMy01MC42IDAtMTUuNyAyMi45LTM1LjYgNTguMy01MC42IDguNi0zLjcgMTgtNyAyNy43LTEwLjEgNS43IDE5LjYgMTMuMiA0MCAyMi41IDYwLjktOS4yIDIwLjgtMTYuNiA0MS4xLTIyLjIgNjAuNi05LjktMy4xLTE5LjMtNi41LTI4LTEwLjJ6TTMxMCA0OTBjLTEzLjYtNy44LTE5LjUtMzcuNS0xNC45LTc1LjcgMS4xLTkuNCAyLjktMTkuMyA1LjEtMjkuNCAxOS42IDQuOCA0MSA4LjUgNjMuNSAxMC45IDEzLjUgMTguNSAyNy41IDM1LjMgNDEuNiA1MC0zMi42IDMwLjMtNjMuMiA0Ni45LTg0IDQ2LjktNC41LS4xLTguMy0xLTExLjMtMi43em0yMzcuMi03Ni4yYzQuNyAzOC4yLTEuMSA2Ny45LTE0LjYgNzUuOC0zIDEuOC02LjkgMi42LTExLjUgMi42LTIwLjcgMC01MS40LTE2LjUtODQtNDYuNiAxNC0xNC43IDI4LTMxLjQgNDEuMy00OS45IDIyLjYtMi40IDQ0LTYuMSA2My42LTExIDIuMyAxMC4xIDQuMSAxOS44IDUuMiAyOS4xem0zOC41LTY2LjdjLTguNiAzLjctMTggNy0yNy43IDEwLjEtNS43LTE5LjYtMTMuMi00MC0yMi41LTYwLjkgOS4yLTIwLjggMTYuNi00MS4xIDIyLjItNjAuNiA5LjkgMy4xIDE5LjMgNi41IDI4LjEgMTAuMiAzNS40IDE1LjEgNTguMyAzNC45IDU4LjMgNTAuNi0uMSAxNS43LTIzIDM1LjYtNTguNCA1MC42ek0zMjAuOCA3OC40eiIvPgogICAgPGNpcmNsZSBjeD0iNDIwLjkiIGN5PSIyOTYuNSIgcj0iNDUuNyIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-redo: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgd2lkdGg9IjE2Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgICA8cGF0aCBkPSJNMCAwaDI0djI0SDB6IiBmaWxsPSJub25lIi8+PHBhdGggZD0iTTE4LjQgMTAuNkMxNi41NSA4Ljk5IDE0LjE1IDggMTEuNSA4Yy00LjY1IDAtOC41OCAzLjAzLTkuOTYgNy4yMkwzLjkgMTZjMS4wNS0zLjE5IDQuMDUtNS41IDcuNi01LjUgMS45NSAwIDMuNzMuNzIgNS4xMiAxLjg4TDEzIDE2aDlWN2wtMy42IDMuNnoiLz4KICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-refresh: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDE4IDE4Ij4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTkgMTMuNWMtMi40OSAwLTQuNS0yLjAxLTQuNS00LjVTNi41MSA0LjUgOSA0LjVjMS4yNCAwIDIuMzYuNTIgMy4xNyAxLjMzTDEwIDhoNVYzbC0xLjc2IDEuNzZDMTIuMTUgMy42OCAxMC42NiAzIDkgMyA1LjY5IDMgMy4wMSA1LjY5IDMuMDEgOVM1LjY5IDE1IDkgMTVjMi45NyAwIDUuNDMtMi4xNiA1LjktNWgtMS41MmMtLjQ2IDItMi4yNCAzLjUtNC4zOCAzLjV6Ii8+CiAgICA8L2c+Cjwvc3ZnPgo=);
  --jp-icon-regex: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KICA8ZyBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiM0MTQxNDEiPgogICAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiAgPC9nPgoKICA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiBmaWxsPSIjRkZGIj4KICAgIDxjaXJjbGUgY2xhc3M9InN0MiIgY3g9IjUuNSIgY3k9IjE0LjUiIHI9IjEuNSIvPgogICAgPHJlY3QgeD0iMTIiIHk9IjQiIGNsYXNzPSJzdDIiIHdpZHRoPSIxIiBoZWlnaHQ9IjgiLz4KICAgIDxyZWN0IHg9IjguNSIgeT0iNy41IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjg2NiAtMC41IDAuNSAwLjg2NiAtMi4zMjU1IDcuMzIxOSkiIGNsYXNzPSJzdDIiIHdpZHRoPSI4IiBoZWlnaHQ9IjEiLz4KICAgIDxyZWN0IHg9IjEyIiB5PSI0IiB0cmFuc2Zvcm09Im1hdHJpeCgwLjUgLTAuODY2IDAuODY2IDAuNSAtMC42Nzc5IDE0LjgyNTIpIiBjbGFzcz0ic3QyIiB3aWR0aD0iMSIgaGVpZ2h0PSI4Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-run: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTggNXYxNGwxMS03eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-running: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDUxMiA1MTIiPgogIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICA8cGF0aCBkPSJNMjU2IDhDMTE5IDggOCAxMTkgOCAyNTZzMTExIDI0OCAyNDggMjQ4IDI0OC0xMTEgMjQ4LTI0OFMzOTMgOCAyNTYgOHptOTYgMzI4YzAgOC44LTcuMiAxNi0xNiAxNkgxNzZjLTguOCAwLTE2LTcuMi0xNi0xNlYxNzZjMC04LjggNy4yLTE2IDE2LTE2aDE2MGM4LjggMCAxNiA3LjIgMTYgMTZ2MTYweiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-save: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTE3IDNINWMtMS4xMSAwLTIgLjktMiAydjE0YzAgMS4xLjg5IDIgMiAyaDE0YzEuMSAwIDItLjkgMi0yVjdsLTQtNHptLTUgMTZjLTEuNjYgMC0zLTEuMzQtMy0zczEuMzQtMyAzLTMgMyAxLjM0IDMgMy0xLjM0IDMtMyAzem0zLTEwSDVWNWgxMHY0eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-search: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMTggMTgiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjEsMTAuOWgtMC43bC0wLjItMC4yYzAuOC0wLjksMS4zLTIuMiwxLjMtMy41YzAtMy0yLjQtNS40LTUuNC01LjRTMS44LDQuMiwxLjgsNy4xczIuNCw1LjQsNS40LDUuNCBjMS4zLDAsMi41LTAuNSwzLjUtMS4zbDAuMiwwLjJ2MC43bDQuMSw0LjFsMS4yLTEuMkwxMi4xLDEwLjl6IE03LjEsMTAuOWMtMi4xLDAtMy43LTEuNy0zLjctMy43czEuNy0zLjcsMy43LTMuN3MzLjcsMS43LDMuNywzLjcgUzkuMiwxMC45LDcuMSwxMC45eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-settings: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIiBkPSJNMTkuNDMgMTIuOThjLjA0LS4zMi4wNy0uNjQuMDctLjk4cy0uMDMtLjY2LS4wNy0uOThsMi4xMS0xLjY1Yy4xOS0uMTUuMjQtLjQyLjEyLS42NGwtMi0zLjQ2Yy0uMTItLjIyLS4zOS0uMy0uNjEtLjIybC0yLjQ5IDFjLS41Mi0uNC0xLjA4LS43My0xLjY5LS45OGwtLjM4LTIuNjVBLjQ4OC40ODggMCAwMDE0IDJoLTRjLS4yNSAwLS40Ni4xOC0uNDkuNDJsLS4zOCAyLjY1Yy0uNjEuMjUtMS4xNy41OS0xLjY5Ljk4bC0yLjQ5LTFjLS4yMy0uMDktLjQ5IDAtLjYxLjIybC0yIDMuNDZjLS4xMy4yMi0uMDcuNDkuMTIuNjRsMi4xMSAxLjY1Yy0uMDQuMzItLjA3LjY1LS4wNy45OHMuMDMuNjYuMDcuOThsLTIuMTEgMS42NWMtLjE5LjE1LS4yNC40Mi0uMTIuNjRsMiAzLjQ2Yy4xMi4yMi4zOS4zLjYxLjIybDIuNDktMWMuNTIuNCAxLjA4LjczIDEuNjkuOThsLjM4IDIuNjVjLjAzLjI0LjI0LjQyLjQ5LjQyaDRjLjI1IDAgLjQ2LS4xOC40OS0uNDJsLjM4LTIuNjVjLjYxLS4yNSAxLjE3LS41OSAxLjY5LS45OGwyLjQ5IDFjLjIzLjA5LjQ5IDAgLjYxLS4yMmwyLTMuNDZjLjEyLS4yMi4wNy0uNDktLjEyLS42NGwtMi4xMS0xLjY1ek0xMiAxNS41Yy0xLjkzIDAtMy41LTEuNTctMy41LTMuNXMxLjU3LTMuNSAzLjUtMy41IDMuNSAxLjU3IDMuNSAzLjUtMS41NyAzLjUtMy41IDMuNXoiLz4KPC9zdmc+Cg==);
  --jp-icon-share: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTSAxOCAyIEMgMTYuMzU0OTkgMiAxNSAzLjM1NDk5MDQgMTUgNSBDIDE1IDUuMTkwOTUyOSAxNS4wMjE3OTEgNS4zNzcxMjI0IDE1LjA1NjY0MSA1LjU1ODU5MzggTCA3LjkyMTg3NSA5LjcyMDcwMzEgQyA3LjM5ODUzOTkgOS4yNzc4NTM5IDYuNzMyMDc3MSA5IDYgOSBDIDQuMzU0OTkwNCA5IDMgMTAuMzU0OTkgMyAxMiBDIDMgMTMuNjQ1MDEgNC4zNTQ5OTA0IDE1IDYgMTUgQyA2LjczMjA3NzEgMTUgNy4zOTg1Mzk5IDE0LjcyMjE0NiA3LjkyMTg3NSAxNC4yNzkyOTcgTCAxNS4wNTY2NDEgMTguNDM5NDUzIEMgMTUuMDIxNTU1IDE4LjYyMTUxNCAxNSAxOC44MDgzODYgMTUgMTkgQyAxNSAyMC42NDUwMSAxNi4zNTQ5OSAyMiAxOCAyMiBDIDE5LjY0NTAxIDIyIDIxIDIwLjY0NTAxIDIxIDE5IEMgMjEgMTcuMzU0OTkgMTkuNjQ1MDEgMTYgMTggMTYgQyAxNy4yNjc0OCAxNiAxNi42MDE1OTMgMTYuMjc5MzI4IDE2LjA3ODEyNSAxNi43MjI2NTYgTCA4Ljk0MzM1OTQgMTIuNTU4NTk0IEMgOC45NzgyMDk1IDEyLjM3NzEyMiA5IDEyLjE5MDk1MyA5IDEyIEMgOSAxMS44MDkwNDcgOC45NzgyMDk1IDExLjYyMjg3OCA4Ljk0MzM1OTQgMTEuNDQxNDA2IEwgMTYuMDc4MTI1IDcuMjc5Mjk2OSBDIDE2LjYwMTQ2IDcuNzIyMTQ2MSAxNy4yNjc5MjMgOCAxOCA4IEMgMTkuNjQ1MDEgOCAyMSA2LjY0NTAwOTYgMjEgNSBDIDIxIDMuMzU0OTkwNCAxOS42NDUwMSAyIDE4IDIgeiBNIDE4IDQgQyAxOC41NjQxMjkgNCAxOSA0LjQzNTg3MDYgMTkgNSBDIDE5IDUuNTY0MTI5NCAxOC41NjQxMjkgNiAxOCA2IEMgMTcuNDM1ODcxIDYgMTcgNS41NjQxMjk0IDE3IDUgQyAxNyA0LjQzNTg3MDYgMTcuNDM1ODcxIDQgMTggNCB6IE0gNiAxMSBDIDYuNTY0MTI5NCAxMSA3IDExLjQzNTg3MSA3IDEyIEMgNyAxMi41NjQxMjkgNi41NjQxMjk0IDEzIDYgMTMgQyA1LjQzNTg3MDYgMTMgNSAxMi41NjQxMjkgNSAxMiBDIDUgMTEuNDM1ODcxIDUuNDM1ODcwNiAxMSA2IDExIHogTSAxOCAxOCBDIDE4LjU2NDEyOSAxOCAxOSAxOC40MzU4NzEgMTkgMTkgQyAxOSAxOS41NjQxMjkgMTguNTY0MTI5IDIwIDE4IDIwIEMgMTcuNDM1ODcxIDIwIDE3IDE5LjU2NDEyOSAxNyAxOSBDIDE3IDE4LjQzNTg3MSAxNy40MzU4NzEgMTggMTggMTggeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-spreadsheet: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8cGF0aCBjbGFzcz0ianAtaWNvbi1jb250cmFzdDEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNENBRjUwIiBkPSJNMi4yIDIuMnYxNy42aDE3LjZWMi4ySDIuMnptMTUuNCA3LjdoLTUuNVY0LjRoNS41djUuNXpNOS45IDQuNHY1LjVINC40VjQuNGg1LjV6bS01LjUgNy43aDUuNXY1LjVINC40di01LjV6bTcuNyA1LjV2LTUuNWg1LjV2NS41aC01LjV6Ii8+Cjwvc3ZnPgo=);
  --jp-icon-stop: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik02IDZoMTJ2MTJINnoiLz4KICAgIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tab: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTIxIDNIM2MtMS4xIDAtMiAuOS0yIDJ2MTRjMCAxLjEuOSAyIDIgMmgxOGMxLjEgMCAyLS45IDItMlY1YzAtMS4xLS45LTItMi0yem0wIDE2SDNWNWgxMHY0aDh2MTB6Ii8+CiAgPC9nPgo8L3N2Zz4K);
  --jp-icon-table-rows: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMSw4SDNWNGgxOFY4eiBNMjEsMTBIM3Y0aDE4VjEweiBNMjEsMTZIM3Y0aDE4VjE2eiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-tag: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjgiIGhlaWdodD0iMjgiIHZpZXdCb3g9IjAgMCA0MyAyOCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KCTxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CgkJPHBhdGggZD0iTTI4LjgzMzIgMTIuMzM0TDMyLjk5OTggMTYuNTAwN0wzNy4xNjY1IDEyLjMzNEgyOC44MzMyWiIvPgoJCTxwYXRoIGQ9Ik0xNi4yMDk1IDIxLjYxMDRDMTUuNjg3MyAyMi4xMjk5IDE0Ljg0NDMgMjIuMTI5OSAxNC4zMjQ4IDIxLjYxMDRMNi45ODI5IDE0LjcyNDVDNi41NzI0IDE0LjMzOTQgNi4wODMxMyAxMy42MDk4IDYuMDQ3ODYgMTMuMDQ4MkM1Ljk1MzQ3IDExLjUyODggNi4wMjAwMiA4LjYxOTQ0IDYuMDY2MjEgNy4wNzY5NUM2LjA4MjgxIDYuNTE0NzcgNi41NTU0OCA2LjA0MzQ3IDcuMTE4MDQgNi4wMzA1NUM5LjA4ODYzIDUuOTg0NzMgMTMuMjYzOCA1LjkzNTc5IDEzLjY1MTggNi4zMjQyNUwyMS43MzY5IDEzLjYzOUMyMi4yNTYgMTQuMTU4NSAyMS43ODUxIDE1LjQ3MjQgMjEuMjYyIDE1Ljk5NDZMMTYuMjA5NSAyMS42MTA0Wk05Ljc3NTg1IDguMjY1QzkuMzM1NTEgNy44MjU2NiA4LjYyMzUxIDcuODI1NjYgOC4xODI4IDguMjY1QzcuNzQzNDYgOC43MDU3MSA3Ljc0MzQ2IDkuNDE3MzMgOC4xODI4IDkuODU2NjdDOC42MjM4MiAxMC4yOTY0IDkuMzM1ODIgMTAuMjk2NCA5Ljc3NTg1IDkuODU2NjdDMTAuMjE1NiA5LjQxNzMzIDEwLjIxNTYgOC43MDUzMyA5Ljc3NTg1IDguMjY1WiIvPgoJPC9nPgo8L3N2Zz4K);
  --jp-icon-terminal: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0IiA+CiAgICA8cmVjdCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1iYWNrZ3JvdW5kLWNvbG9yIGpwLWljb24tc2VsZWN0YWJsZSIgd2lkdGg9IjIwIiBoZWlnaHQ9IjIwIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSgyIDIpIiBmaWxsPSIjMzMzMzMzIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtdGVybWluYWwtaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUtaW52ZXJzZSIgZD0iTTUuMDU2NjQgOC43NjE3MkM1LjA1NjY0IDguNTk3NjYgNS4wMzEyNSA4LjQ1MzEyIDQuOTgwNDcgOC4zMjgxMkM0LjkzMzU5IDguMTk5MjIgNC44NTU0NyA4LjA4MjAzIDQuNzQ2MDkgNy45NzY1NkM0LjY0MDYyIDcuODcxMDkgNC41IDcuNzc1MzkgNC4zMjQyMiA3LjY4OTQ1QzQuMTUyMzQgNy41OTk2MSAzLjk0MzM2IDcuNTExNzIgMy42OTcyNyA3LjQyNTc4QzMuMzAyNzMgNy4yODUxNiAyLjk0MzM2IDcuMTM2NzIgMi42MTkxNCA2Ljk4MDQ3QzIuMjk0OTIgNi44MjQyMiAyLjAxNzU4IDYuNjQyNTggMS43ODcxMSA2LjQzNTU1QzEuNTYwNTUgNi4yMjg1MiAxLjM4NDc3IDUuOTg4MjggMS4yNTk3NyA1LjcxNDg0QzEuMTM0NzcgNS40Mzc1IDEuMDcyMjcgNS4xMDkzOCAxLjA3MjI3IDQuNzMwNDdDMS4wNzIyNyA0LjM5ODQ0IDEuMTI4OTEgNC4wOTU3IDEuMjQyMTkgMy44MjIyN0MxLjM1NTQ3IDMuNTQ0OTIgMS41MTU2MiAzLjMwNDY5IDEuNzIyNjYgMy4xMDE1NkMxLjkyOTY5IDIuODk4NDQgMi4xNzk2OSAyLjczNDM3IDIuNDcyNjYgMi42MDkzOEMyLjc2NTYyIDIuNDg0MzggMy4wOTE4IDIuNDA0MyAzLjQ1MTE3IDIuMzY5MTRWMS4xMDkzOEg0LjM4ODY3VjIuMzgwODZDNC43NDAyMyAyLjQyNzczIDUuMDU2NjQgMi41MjM0NCA1LjMzNzg5IDIuNjY3OTdDNS42MTkxNCAyLjgxMjUgNS44NTc0MiAzLjAwMTk1IDYuMDUyNzMgMy4yMzYzM0M2LjI1MTk1IDMuNDY2OCA2LjQwNDMgMy43NDAyMyA2LjUwOTc3IDQuMDU2NjRDNi42MTkxNCA0LjM2OTE0IDYuNjczODMgNC43MjA3IDYuNjczODMgNS4xMTEzM0g1LjA0NDkyQzUuMDQ0OTIgNC42Mzg2NyA0LjkzNzUgNC4yODEyNSA0LjcyMjY2IDQuMDM5MDZDNC41MDc4MSAzLjc5Mjk3IDQuMjE2OCAzLjY2OTkyIDMuODQ5NjEgMy42Njk5MkMzLjY1MDM5IDMuNjY5OTIgMy40NzY1NiAzLjY5NzI3IDMuMzI4MTIgMy43NTE5NUMzLjE4MzU5IDMuODAyNzMgMy4wNjQ0NSAzLjg3Njk1IDIuOTcwNyAzLjk3NDYxQzIuODc2OTUgNC4wNjgzNiAyLjgwNjY0IDQuMTc5NjkgMi43NTk3NyA0LjMwODU5QzIuNzE2OCA0LjQzNzUgMi42OTUzMSA0LjU3ODEyIDIuNjk1MzEgNC43MzA0N0MyLjY5NTMxIDQuODgyODEgMi43MTY4IDUuMDE5NTMgMi43NTk3NyA1LjE0MDYyQzIuODA2NjQgNS4yNTc4MSAyLjg4MjgxIDUuMzY3MTkgMi45ODgyOCA1LjQ2ODc1QzMuMDk3NjYgNS41NzAzMSAzLjI0MDIzIDUuNjY3OTcgMy40MTYwMiA1Ljc2MTcyQzMuNTkxOCA1Ljg1MTU2IDMuODEwNTUgNS45NDMzNiA0LjA3MjI3IDYuMDM3MTFDNC40NjY4IDYuMTg1NTUgNC44MjQyMiA2LjMzOTg0IDUuMTQ0NTMgNi41QzUuNDY0ODQgNi42NTYyNSA1LjczODI4IDYuODM5ODQgNS45NjQ4NCA3LjA1MDc4QzYuMTk1MzEgNy4yNTc4MSA2LjM3MTA5IDcuNSA2LjQ5MjE5IDcuNzc3MzRDNi42MTcxOSA4LjA1MDc4IDYuNjc5NjkgOC4zNzUgNi42Nzk2OSA4Ljc1QzYuNjc5NjkgOS4wOTM3NSA2LjYyMzA1IDkuNDA0MyA2LjUwOTc3IDkuNjgxNjRDNi4zOTY0OCA5Ljk1NTA4IDYuMjM0MzggMTAuMTkxNCA2LjAyMzQ0IDEwLjM5MDZDNS44MTI1IDEwLjU4OTggNS41NTg1OSAxMC43NSA1LjI2MTcyIDEwLjg3MTFDNC45NjQ4NCAxMC45ODgzIDQuNjMyODEgMTEuMDY0NSA0LjI2NTYyIDExLjA5OTZWMTIuMjQ4SDMuMzMzOThWMTEuMDk5NkMzLjAwMTk1IDExLjA2ODQgMi42Nzk2OSAxMC45OTYxIDIuMzY3MTkgMTAuODgyOEMyLjA1NDY5IDEwLjc2NTYgMS43NzczNCAxMC41OTc3IDEuNTM1MTYgMTAuMzc4OUMxLjI5Njg4IDEwLjE2MDIgMS4xMDU0NyA5Ljg4NDc3IDAuOTYwOTM4IDkuNTUyNzNDMC44MTY0MDYgOS4yMTY4IDAuNzQ0MTQxIDguODE0NDUgMC43NDQxNDEgOC4zNDU3SDIuMzc4OTFDMi4zNzg5MSA4LjYyNjk1IDIuNDE5OTIgOC44NjMyOCAyLjUwMTk1IDkuMDU0NjlDMi41ODM5OCA5LjI0MjE5IDIuNjg5NDUgOS4zOTI1OCAyLjgxODM2IDkuNTA1ODZDMi45NTExNyA5LjYxNTIzIDMuMTAxNTYgOS42OTMzNiAzLjI2OTUzIDkuNzQwMjNDMy40Mzc1IDkuNzg3MTEgMy42MDkzOCA5LjgxMDU1IDMuNzg1MTYgOS44MTA1NUM0LjIwMzEyIDkuODEwNTUgNC41MTk1MyA5LjcxMjg5IDQuNzM0MzggOS41MTc1OEM0Ljk0OTIyIDkuMzIyMjcgNS4wNTY2NCA5LjA3MDMxIDUuMDU2NjQgOC43NjE3MlpNMTMuNDE4IDEyLjI3MTVIOC4wNzQyMlYxMUgxMy40MThWMTIuMjcxNVoiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDMuOTUyNjQgNikiIGZpbGw9IndoaXRlIi8+Cjwvc3ZnPgo=);
  --jp-icon-text-editor: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8cGF0aCBjbGFzcz0ianAtdGV4dC1lZGl0b3ItaWNvbi1jb2xvciBqcC1pY29uLXNlbGVjdGFibGUiIGZpbGw9IiM2MTYxNjEiIGQ9Ik0xNSAxNUgzdjJoMTJ2LTJ6bTAtOEgzdjJoMTJWN3pNMyAxM2gxOHYtMkgzdjJ6bTAgOGgxOHYtMkgzdjJ6TTMgM3YyaDE4VjNIM3oiLz4KPC9zdmc+Cg==);
  --jp-icon-toc: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0Ij4KICA8ZyBjbGFzcz0ianAtaWNvbjMganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjNjE2MTYxIj4KICAgIDxwYXRoIGQ9Ik03LDVIMjFWN0g3VjVNNywxM1YxMUgyMVYxM0g3TTQsNC41QTEuNSwxLjUgMCAwLDEgNS41LDZBMS41LDEuNSAwIDAsMSA0LDcuNUExLjUsMS41IDAgMCwxIDIuNSw2QTEuNSwxLjUgMCAwLDEgNCw0LjVNNCwxMC41QTEuNSwxLjUgMCAwLDEgNS41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMy41QTEuNSwxLjUgMCAwLDEgMi41LDEyQTEuNSwxLjUgMCAwLDEgNCwxMC41TTcsMTlWMTdIMjFWMTlIN000LDE2LjVBMS41LDEuNSAwIDAsMSA1LjUsMThBMS41LDEuNSAwIDAsMSA0LDE5LjVBMS41LDEuNSAwIDAsMSAyLjUsMThBMS41LDEuNSAwIDAsMSA0LDE2LjVaIiAvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-tree-view: url(data:image/svg+xml;base64,PHN2ZyBoZWlnaHQ9IjI0IiB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICAgIDxnIGNsYXNzPSJqcC1pY29uMyIgZmlsbD0iIzYxNjE2MSI+CiAgICAgICAgPHBhdGggZD0iTTAgMGgyNHYyNEgweiIgZmlsbD0ibm9uZSIvPgogICAgICAgIDxwYXRoIGQ9Ik0yMiAxMVYzaC03djNIOVYzSDJ2OGg3VjhoMnYxMGg0djNoN3YtOGgtN3YzaC0yVjhoMnYzeiIvPgogICAgPC9nPgo8L3N2Zz4K);
  --jp-icon-trusted: url(data:image/svg+xml;base64,PHN2ZyBmaWxsPSJub25lIiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDI0IDI1Ij4KICAgIDxwYXRoIGNsYXNzPSJqcC1pY29uMiIgc3Ryb2tlPSIjMzMzMzMzIiBzdHJva2Utd2lkdGg9IjIiIHRyYW5zZm9ybT0idHJhbnNsYXRlKDIgMykiIGQ9Ik0xLjg2MDk0IDExLjQ0MDlDMC44MjY0NDggOC43NzAyNyAwLjg2Mzc3OSA2LjA1NzY0IDEuMjQ5MDcgNC4xOTkzMkMyLjQ4MjA2IDMuOTMzNDcgNC4wODA2OCAzLjQwMzQ3IDUuNjAxMDIgMi44NDQ5QzcuMjM1NDkgMi4yNDQ0IDguODU2NjYgMS41ODE1IDkuOTg3NiAxLjA5NTM5QzExLjA1OTcgMS41ODM0MSAxMi42MDk0IDIuMjQ0NCAxNC4yMTggMi44NDMzOUMxNS43NTAzIDMuNDEzOTQgMTcuMzk5NSAzLjk1MjU4IDE4Ljc1MzkgNC4yMTM4NUMxOS4xMzY0IDYuMDcxNzcgMTkuMTcwOSA4Ljc3NzIyIDE4LjEzOSAxMS40NDA5QzE3LjAzMDMgMTQuMzAzMiAxNC42NjY4IDE3LjE4NDQgOS45OTk5OSAxOC45MzU0QzUuMzMzMiAxNy4xODQ0IDIuOTY5NjggMTQuMzAzMiAxLjg2MDk0IDExLjQ0MDlaIi8+CiAgICA8cGF0aCBjbGFzcz0ianAtaWNvbjIiIGZpbGw9IiMzMzMzMzMiIHN0cm9rZT0iIzMzMzMzMyIgdHJhbnNmb3JtPSJ0cmFuc2xhdGUoOCA5Ljg2NzE5KSIgZD0iTTIuODYwMTUgNC44NjUzNUwwLjcyNjU0OSAyLjk5OTU5TDAgMy42MzA0NUwyLjg2MDE1IDYuMTMxNTdMOCAwLjYzMDg3Mkw3LjI3ODU3IDBMMi44NjAxNSA0Ljg2NTM1WiIvPgo8L3N2Zz4K);
  --jp-icon-undo: url(data:image/svg+xml;base64,PHN2ZyB2aWV3Qm94PSIwIDAgMjQgMjQiIHdpZHRoPSIxNiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTEyLjUgOGMtMi42NSAwLTUuMDUuOTktNi45IDIuNkwyIDd2OWg5bC0zLjYyLTMuNjJjMS4zOS0xLjE2IDMuMTYtMS44OCA1LjEyLTEuODggMy41NCAwIDYuNTUgMi4zMSA3LjYgNS41bDIuMzctLjc4QzIxLjA4IDExLjAzIDE3LjE1IDggMTIuNSA4eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-user: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMTYiIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KICA8ZyBjbGFzcz0ianAtaWNvbjMiIGZpbGw9IiM2MTYxNjEiPgogICAgPHBhdGggZD0iTTE2IDdhNCA0IDAgMTEtOCAwIDQgNCAwIDAxOCAwek0xMiAxNGE3IDcgMCAwMC03IDdoMTRhNyA3IDAgMDAtNy03eiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-users: url(data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZlcnNpb249IjEuMSIgdmlld0JveD0iMCAwIDM2IDI0IiB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgogPGcgY2xhc3M9ImpwLWljb24zIiB0cmFuc2Zvcm09Im1hdHJpeCgxLjczMjcgMCAwIDEuNzMyNyAtMy42MjgyIC4wOTk1NzcpIiBmaWxsPSIjNjE2MTYxIj4KICA8cGF0aCB0cmFuc2Zvcm09Im1hdHJpeCgxLjUsMCwwLDEuNSwwLC02KSIgZD0ibTEyLjE4NiA3LjUwOThjLTEuMDUzNSAwLTEuOTc1NyAwLjU2NjUtMi40Nzg1IDEuNDEwMiAwLjc1MDYxIDAuMzEyNzcgMS4zOTc0IDAuODI2NDggMS44NzMgMS40NzI3aDMuNDg2M2MwLTEuNTkyLTEuMjg4OS0yLjg4MjgtMi44ODA5LTIuODgyOHoiLz4KICA8cGF0aCBkPSJtMjAuNDY1IDIuMzg5NWEyLjE4ODUgMi4xODg1IDAgMCAxLTIuMTg4NCAyLjE4ODUgMi4xODg1IDIuMTg4NSAwIDAgMS0yLjE4ODUtMi4xODg1IDIuMTg4NSAyLjE4ODUgMCAwIDEgMi4xODg1LTIuMTg4NSAyLjE4ODUgMi4xODg1IDAgMCAxIDIuMTg4NCAyLjE4ODV6Ii8+CiAgPHBhdGggdHJhbnNmb3JtPSJtYXRyaXgoMS41LDAsMCwxLjUsMCwtNikiIGQ9Im0zLjU4OTggOC40MjE5Yy0xLjExMjYgMC0yLjAxMzcgMC45MDExMS0yLjAxMzcgMi4wMTM3aDIuODE0NWMwLjI2Nzk3LTAuMzczMDkgMC41OTA3LTAuNzA0MzUgMC45NTg5OC0wLjk3ODUyLTAuMzQ0MzMtMC42MTY4OC0xLjAwMzEtMS4wMzUyLTEuNzU5OC0xLjAzNTJ6Ii8+CiAgPHBhdGggZD0ibTYuOTE1NCA0LjYyM2ExLjUyOTQgMS41Mjk0IDAgMCAxLTEuNTI5NCAxLjUyOTQgMS41Mjk0IDEuNTI5NCAwIDAgMS0xLjUyOTQtMS41Mjk0IDEuNTI5NCAxLjUyOTQgMCAwIDEgMS41Mjk0LTEuNTI5NCAxLjUyOTQgMS41Mjk0IDAgMCAxIDEuNTI5NCAxLjUyOTR6Ii8+CiAgPHBhdGggZD0ibTYuMTM1IDEzLjUzNWMwLTMuMjM5MiAyLjYyNTktNS44NjUgNS44NjUtNS44NjUgMy4yMzkyIDAgNS44NjUgMi42MjU5IDUuODY1IDUuODY1eiIvPgogIDxjaXJjbGUgY3g9IjEyIiBjeT0iMy43Njg1IiByPSIyLjk2ODUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-vega: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbjEganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjMjEyMTIxIj4KICAgIDxwYXRoIGQ9Ik0xMC42IDUuNGwyLjItMy4ySDIuMnY3LjNsNC02LjZ6Ii8+CiAgICA8cGF0aCBkPSJNMTUuOCAyLjJsLTQuNCA2LjZMNyA2LjNsLTQuOCA4djUuNWgxNy42VjIuMmgtNHptLTcgMTUuNEg1LjV2LTQuNGgzLjN2NC40em00LjQgMEg5LjhWOS44aDMuNHY3Ljh6bTQuNCAwaC0zLjRWNi41aDMuNHYxMS4xeiIvPgogIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-word: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIwIDIwIj4KIDxnIGNsYXNzPSJqcC1pY29uMiIgZmlsbD0iIzQxNDE0MSI+CiAgPHJlY3QgeD0iMiIgeT0iMiIgd2lkdGg9IjE2IiBoZWlnaHQ9IjE2Ii8+CiA8L2c+CiA8ZyBjbGFzcz0ianAtaWNvbi1hY2NlbnQyIiB0cmFuc2Zvcm09InRyYW5zbGF0ZSguNDMgLjA0MDEpIiBmaWxsPSIjZmZmIj4KICA8cGF0aCBkPSJtNC4xNCA4Ljc2cTAuMDY4Mi0xLjg5IDIuNDItMS44OSAxLjE2IDAgMS42OCAwLjQyIDAuNTY3IDAuNDEgMC41NjcgMS4xNnYzLjQ3cTAgMC40NjIgMC41MTQgMC40NjIgMC4xMDMgMCAwLjItMC4wMjMxdjAuNzE0cS0wLjM5OSAwLjEwMy0wLjY1MSAwLjEwMy0wLjQ1MiAwLTAuNjkzLTAuMjItMC4yMzEtMC4yLTAuMjg0LTAuNjYyLTAuOTU2IDAuODcyLTIgMC44NzItMC45MDMgMC0xLjQ3LTAuNDcyLTAuNTI1LTAuNDcyLTAuNTI1LTEuMjYgMC0wLjI2MiAwLjA0NTItMC40NzIgMC4wNTY3LTAuMjIgMC4xMTYtMC4zNzggMC4wNjgyLTAuMTY4IDAuMjMxLTAuMzA0IDAuMTU4LTAuMTQ3IDAuMjYyLTAuMjQyIDAuMTE2LTAuMDkxNCAwLjM2OC0wLjE2OCAwLjI2Mi0wLjA5MTQgMC4zOTktMC4xMjYgMC4xMzYtMC4wNDUyIDAuNDcyLTAuMTAzIDAuMzM2LTAuMDU3OCAwLjUwNC0wLjA3OTggMC4xNTgtMC4wMjMxIDAuNTY3LTAuMDc5OCAwLjU1Ni0wLjA2ODIgMC43NzctMC4yMjEgMC4yMi0wLjE1MiAwLjIyLTAuNDQxdi0wLjI1MnEwLTAuNDMtMC4zNTctMC42NjItMC4zMzYtMC4yMzEtMC45NzYtMC4yMzEtMC42NjIgMC0wLjk5OCAwLjI2Mi0wLjMzNiAwLjI1Mi0wLjM5OSAwLjc5OHptMS44OSAzLjY4cTAuNzg4IDAgMS4yNi0wLjQxIDAuNTA0LTAuNDIgMC41MDQtMC45MDN2LTEuMDVxLTAuMjg0IDAuMTM2LTAuODYxIDAuMjMxLTAuNTY3IDAuMDkxNC0wLjk4NyAwLjE1OC0wLjQyIDAuMDY4Mi0wLjc2NiAwLjMyNi0wLjMzNiAwLjI1Mi0wLjMzNiAwLjcwNHQwLjMwNCAwLjcwNCAwLjg2MSAwLjI1MnoiIHN0cm9rZS13aWR0aD0iMS4wNSIvPgogIDxwYXRoIGQ9Im0xMCA0LjU2aDAuOTQ1djMuMTVxMC42NTEtMC45NzYgMS44OS0wLjk3NiAxLjE2IDAgMS44OSAwLjg0IDAuNjgyIDAuODQgMC42ODIgMi4zMSAwIDEuNDctMC43MDQgMi40Mi0wLjcwNCAwLjg4Mi0xLjg5IDAuODgyLTEuMjYgMC0xLjg5LTEuMDJ2MC43NjZoLTAuODV6bTIuNjIgMy4wNHEtMC43NDYgMC0xLjE2IDAuNjQtMC40NTIgMC42My0wLjQ1MiAxLjY4IDAgMS4wNSAwLjQ1MiAxLjY4dDEuMTYgMC42M3EwLjc3NyAwIDEuMjYtMC42MyAwLjQ5NC0wLjY0IDAuNDk0LTEuNjggMC0xLjA1LTAuNDcyLTEuNjgtMC40NjItMC42NC0xLjI2LTAuNjR6IiBzdHJva2Utd2lkdGg9IjEuMDUiLz4KICA8cGF0aCBkPSJtMi43MyAxNS44IDEzLjYgMC4wMDgxYzAuMDA2OSAwIDAtMi42IDAtMi42IDAtMC4wMDc4LTEuMTUgMC0xLjE1IDAtMC4wMDY5IDAtMC4wMDgzIDEuNS0wLjAwODMgMS41LTJlLTMgLTAuMDAxNC0xMS4zLTAuMDAxNC0xMS4zLTAuMDAxNGwtMC4wMDU5Mi0xLjVjMC0wLjAwNzgtMS4xNyAwLjAwMTMtMS4xNyAwLjAwMTN6IiBzdHJva2Utd2lkdGg9Ii45NzUiLz4KIDwvZz4KPC9zdmc+Cg==);
  --jp-icon-yaml: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxNiIgdmlld0JveD0iMCAwIDIyIDIyIj4KICA8ZyBjbGFzcz0ianAtaWNvbi1jb250cmFzdDIganAtaWNvbi1zZWxlY3RhYmxlIiBmaWxsPSIjRDgxQjYwIj4KICAgIDxwYXRoIGQ9Ik03LjIgMTguNnYtNS40TDMgNS42aDMuM2wxLjQgMy4xYy4zLjkuNiAxLjYgMSAyLjUuMy0uOC42LTEuNiAxLTIuNWwxLjQtMy4xaDMuNGwtNC40IDcuNnY1LjVsLTIuOS0uMXoiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxNi41IiByPSIyLjEiLz4KICAgIDxjaXJjbGUgY2xhc3M9InN0MCIgY3g9IjE3LjYiIGN5PSIxMSIgcj0iMi4xIi8+CiAgPC9nPgo8L3N2Zz4K);
}

/* Icon CSS class declarations */

.jp-AddAboveIcon {
  background-image: var(--jp-icon-add-above);
}

.jp-AddBelowIcon {
  background-image: var(--jp-icon-add-below);
}

.jp-AddIcon {
  background-image: var(--jp-icon-add);
}

.jp-BellIcon {
  background-image: var(--jp-icon-bell);
}

.jp-BugDotIcon {
  background-image: var(--jp-icon-bug-dot);
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

.jp-CodeCheckIcon {
  background-image: var(--jp-icon-code-check);
}

.jp-CodeIcon {
  background-image: var(--jp-icon-code);
}

.jp-CollapseAllIcon {
  background-image: var(--jp-icon-collapse-all);
}

.jp-ConsoleIcon {
  background-image: var(--jp-icon-console);
}

.jp-CopyIcon {
  background-image: var(--jp-icon-copy);
}

.jp-CopyrightIcon {
  background-image: var(--jp-icon-copyright);
}

.jp-CutIcon {
  background-image: var(--jp-icon-cut);
}

.jp-DeleteIcon {
  background-image: var(--jp-icon-delete);
}

.jp-DownloadIcon {
  background-image: var(--jp-icon-download);
}

.jp-DuplicateIcon {
  background-image: var(--jp-icon-duplicate);
}

.jp-EditIcon {
  background-image: var(--jp-icon-edit);
}

.jp-EllipsesIcon {
  background-image: var(--jp-icon-ellipses);
}

.jp-ErrorIcon {
  background-image: var(--jp-icon-error);
}

.jp-ExpandAllIcon {
  background-image: var(--jp-icon-expand-all);
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

.jp-FilterDotIcon {
  background-image: var(--jp-icon-filter-dot);
}

.jp-FilterIcon {
  background-image: var(--jp-icon-filter);
}

.jp-FilterListIcon {
  background-image: var(--jp-icon-filter-list);
}

.jp-FolderFavoriteIcon {
  background-image: var(--jp-icon-folder-favorite);
}

.jp-FolderIcon {
  background-image: var(--jp-icon-folder);
}

.jp-HomeIcon {
  background-image: var(--jp-icon-home);
}

.jp-Html5Icon {
  background-image: var(--jp-icon-html5);
}

.jp-ImageIcon {
  background-image: var(--jp-icon-image);
}

.jp-InfoIcon {
  background-image: var(--jp-icon-info);
}

.jp-InspectorIcon {
  background-image: var(--jp-icon-inspector);
}

.jp-JsonIcon {
  background-image: var(--jp-icon-json);
}

.jp-JuliaIcon {
  background-image: var(--jp-icon-julia);
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

.jp-LaunchIcon {
  background-image: var(--jp-icon-launch);
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

.jp-MarkdownIcon {
  background-image: var(--jp-icon-markdown);
}

.jp-MoveDownIcon {
  background-image: var(--jp-icon-move-down);
}

.jp-MoveUpIcon {
  background-image: var(--jp-icon-move-up);
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

.jp-NumberingIcon {
  background-image: var(--jp-icon-numbering);
}

.jp-OfflineBoltIcon {
  background-image: var(--jp-icon-offline-bolt);
}

.jp-PaletteIcon {
  background-image: var(--jp-icon-palette);
}

.jp-PasteIcon {
  background-image: var(--jp-icon-paste);
}

.jp-PdfIcon {
  background-image: var(--jp-icon-pdf);
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

.jp-RedoIcon {
  background-image: var(--jp-icon-redo);
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

.jp-ShareIcon {
  background-image: var(--jp-icon-share);
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

.jp-TableRowsIcon {
  background-image: var(--jp-icon-table-rows);
}

.jp-TagIcon {
  background-image: var(--jp-icon-tag);
}

.jp-TerminalIcon {
  background-image: var(--jp-icon-terminal);
}

.jp-TextEditorIcon {
  background-image: var(--jp-icon-text-editor);
}

.jp-TocIcon {
  background-image: var(--jp-icon-toc);
}

.jp-TreeViewIcon {
  background-image: var(--jp-icon-tree-view);
}

.jp-TrustedIcon {
  background-image: var(--jp-icon-trusted);
}

.jp-UndoIcon {
  background-image: var(--jp-icon-undo);
}

.jp-UserIcon {
  background-image: var(--jp-icon-user);
}

.jp-UsersIcon {
  background-image: var(--jp-icon-users);
}

.jp-VegaIcon {
  background-image: var(--jp-icon-vega);
}

.jp-WordIcon {
  background-image: var(--jp-icon-word);
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

.lm-TabBar .lm-TabBar-addButton {
  align-items: center;
  display: flex;
  padding: 4px;
  padding-bottom: 5px;
  margin-right: 1px;
  background-color: var(--jp-layout-color2);
}

.lm-TabBar .lm-TabBar-addButton:hover {
  background-color: var(--jp-layout-color1);
}

.lm-DockPanel-tabBar .lm-TabBar-tab {
  width: var(--jp-private-horizontal-tab-width);
}

.lm-DockPanel-tabBar .lm-TabBar-content {
  flex: unset;
}

.lm-DockPanel-tabBar[data-orientation='horizontal'] {
  flex: 1 1 auto;
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

.jp-icon-dot[fill] {
  fill: var(--jp-warn-color0);
}

.jp-jupyter-icon-color[fill] {
  fill: var(--jp-jupyter-icon-color, var(--jp-warn-color0));
}

.jp-notebook-icon-color[fill] {
  fill: var(--jp-notebook-icon-color, var(--jp-warn-color0));
}

.jp-json-icon-color[fill] {
  fill: var(--jp-json-icon-color, var(--jp-warn-color1));
}

.jp-console-icon-color[fill] {
  fill: var(--jp-console-icon-color, white);
}

.jp-console-icon-background-color[fill] {
  fill: var(--jp-console-icon-background-color, var(--jp-brand-color1));
}

.jp-terminal-icon-color[fill] {
  fill: var(--jp-terminal-icon-color, var(--jp-layout-color2));
}

.jp-terminal-icon-background-color[fill] {
  fill: var(
    --jp-terminal-icon-background-color,
    var(--jp-inverse-layout-color2)
  );
}

.jp-text-editor-icon-color[fill] {
  fill: var(--jp-text-editor-icon-color, var(--jp-inverse-layout-color3));
}

.jp-inspector-icon-color[fill] {
  fill: var(--jp-inspector-icon-color, var(--jp-inverse-layout-color3));
}

/* CSS for icons in selected filebrowser listing items */
.jp-DirListing-item.jp-mod-selected .jp-icon-selectable[fill] {
  fill: #fff;
}

.jp-DirListing-item.jp-mod-selected .jp-icon-selectable-inverse[fill] {
  fill: var(--jp-brand-color1);
}

/* stylelint-disable selector-max-class, selector-max-compound-selectors */

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

/* stylelint-enable selector-max-class, selector-max-compound-selectors */

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

.jp-icon-hoverShow:not(:hover) .jp-icon-hoverShow-content {
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

.jp-IFrame {
  width: 100%;
  height: 100%;
}

.jp-IFrame > iframe {
  border: none;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-IFrame {
  position: relative;
}

body.lm-mod-override-cursor .jp-IFrame::before {
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

.jp-HoverBox {
  position: fixed;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-FormGroup-content fieldset {
  border: none;
  padding: 0;
  min-width: 0;
  width: 100%;
}

/* stylelint-disable selector-max-type */

.jp-FormGroup-content fieldset .jp-inputFieldWrapper input,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper select,
.jp-FormGroup-content fieldset .jp-inputFieldWrapper textarea {
  font-size: var(--jp-content-font-size2);
  border-color: var(--jp-input-border-color);
  border-style: solid;
  border-radius: var(--jp-border-radius);
  border-width: 1px;
  padding: 6px 8px;
  background: none;
  color: var(--jp-ui-font-color0);
  height: inherit;
}

.jp-FormGroup-content fieldset input[type='checkbox'] {
  position: relative;
  top: 2px;
  margin-left: 0;
}

.jp-FormGroup-content button.jp-mod-styled {
  cursor: pointer;
}

.jp-FormGroup-content .checkbox label {
  cursor: pointer;
  font-size: var(--jp-content-font-size1);
}

.jp-FormGroup-content .jp-root > fieldset > legend {
  display: none;
}

.jp-FormGroup-content .jp-root > fieldset > p {
  display: none;
}

/** copy of `input.jp-mod-styled:focus` style */
.jp-FormGroup-content fieldset input:focus,
.jp-FormGroup-content fieldset select:focus {
  -moz-outline-radius: unset;
  outline: var(--jp-border-width) solid var(--md-blue-500);
  outline-offset: -1px;
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-FormGroup-content fieldset input:hover:not(:focus),
.jp-FormGroup-content fieldset select:hover:not(:focus) {
  background-color: var(--jp-border-color2);
}

/* stylelint-enable selector-max-type */

.jp-FormGroup-content .checkbox .field-description {
  /* Disable default description field for checkbox:
   because other widgets do not have description fields,
   we add descriptions to each widget on the field level.
  */
  display: none;
}

.jp-FormGroup-content #root__description {
  display: none;
}

.jp-FormGroup-content .jp-modifiedIndicator {
  width: 5px;
  background-color: var(--jp-brand-color2);
  margin-top: 0;
  margin-left: calc(var(--jp-private-settingeditor-modifier-indent) * -1);
  flex-shrink: 0;
}

.jp-FormGroup-content .jp-modifiedIndicator.jp-errorIndicator {
  background-color: var(--jp-error-color0);
  margin-right: 0.5em;
}

/* RJSF ARRAY style */

.jp-arrayFieldWrapper legend {
  font-size: var(--jp-content-font-size2);
  color: var(--jp-ui-font-color0);
  flex-basis: 100%;
  padding: 4px 0;
  font-weight: var(--jp-content-heading-font-weight);
  border-bottom: 1px solid var(--jp-border-color2);
}

.jp-arrayFieldWrapper .field-description {
  padding: 4px 0;
  white-space: pre-wrap;
}

.jp-arrayFieldWrapper .array-item {
  width: 100%;
  border: 1px solid var(--jp-border-color2);
  border-radius: 4px;
  margin: 4px;
}

.jp-ArrayOperations {
  display: flex;
  margin-left: 8px;
}

.jp-ArrayOperationsButton {
  margin: 2px;
}

.jp-ArrayOperationsButton .jp-icon3[fill] {
  fill: var(--jp-ui-font-color0);
}

button.jp-ArrayOperationsButton.jp-mod-styled:disabled {
  cursor: not-allowed;
  opacity: 0.5;
}

/* RJSF form validation error */

.jp-FormGroup-content .validationErrors {
  color: var(--jp-error-color0);
}

/* Hide panel level error as duplicated the field level error */
.jp-FormGroup-content .panel.errors {
  display: none;
}

/* RJSF normal content (settings-editor) */

.jp-FormGroup-contentNormal {
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-FormGroup-contentItem {
  margin-left: 7px;
  color: var(--jp-ui-font-color0);
}

.jp-FormGroup-contentNormal .jp-FormGroup-description {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-default {
  flex-basis: 100%;
  padding: 4px 7px;
}

.jp-FormGroup-contentNormal .jp-FormGroup-fieldLabel {
  font-size: var(--jp-content-font-size1);
  font-weight: normal;
  min-width: 120px;
}

.jp-FormGroup-contentNormal fieldset:not(:first-child) {
  margin-left: 7px;
}

.jp-FormGroup-contentNormal .field-array-of-string .array-item {
  /* Display `jp-ArrayOperations` buttons side-by-side with content except
    for small screens where flex-wrap will place them one below the other.
  */
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}

.jp-FormGroup-contentNormal .jp-objectFieldWrapper .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

/* RJSF compact content (metadata-form) */

.jp-FormGroup-content.jp-FormGroup-contentCompact {
  width: 100%;
}

.jp-FormGroup-contentCompact .form-group {
  display: flex;
  padding: 0.5em 0.2em 0.5em 0;
}

.jp-FormGroup-contentCompact
  .jp-FormGroup-compactTitle
  .jp-FormGroup-description {
  font-size: var(--jp-ui-font-size1);
  color: var(--jp-ui-font-color2);
}

.jp-FormGroup-contentCompact .jp-FormGroup-fieldLabel {
  padding-bottom: 0.3em;
}

.jp-FormGroup-contentCompact .jp-inputFieldWrapper .form-control {
  width: 100%;
  box-sizing: border-box;
}

.jp-FormGroup-contentCompact .jp-arrayFieldWrapper .jp-FormGroup-compactTitle {
  padding-bottom: 7px;
}

.jp-FormGroup-contentCompact
  .jp-objectFieldWrapper
  .jp-objectFieldWrapper
  .form-group {
  padding: 2px 8px 2px var(--jp-private-settingeditor-modifier-indent);
  margin-top: 2px;
}

.jp-FormGroup-contentCompact ul.error-detail {
  margin-block-start: 0.5em;
  margin-block-end: 0.5em;
  padding-inline-start: 1em;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-SidePanel {
  display: flex;
  flex-direction: column;
  min-width: var(--jp-sidebar-min-width);
  overflow-y: auto;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);
  font-size: var(--jp-ui-font-size1);
}

.jp-SidePanel-header {
  flex: 0 0 auto;
  display: flex;
  border-bottom: var(--jp-border-width) solid var(--jp-border-color2);
  font-size: var(--jp-ui-font-size0);
  font-weight: 600;
  letter-spacing: 1px;
  margin: 0;
  padding: 2px;
  text-transform: uppercase;
}

.jp-SidePanel-toolbar {
  flex: 0 0 auto;
}

.jp-SidePanel-content {
  flex: 1 1 auto;
}

.jp-SidePanel-toolbar,
.jp-AccordionPanel-toolbar {
  height: var(--jp-private-toolbar-height);
}

.jp-SidePanel-toolbar.jp-Toolbar-micro {
  display: none;
}

.lm-AccordionPanel .jp-AccordionPanel-title {
  box-sizing: border-box;
  line-height: 25px;
  margin: 0;
  display: flex;
  align-items: center;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  font-size: var(--jp-ui-font-size0);
}

.jp-AccordionPanel-title {
  cursor: pointer;
  user-select: none;
  -moz-user-select: none;
  -webkit-user-select: none;
  text-transform: uppercase;
}

.lm-AccordionPanel[data-orientation='horizontal'] > .jp-AccordionPanel-title {
  /* Title is rotated for horizontal accordion panel using CSS */
  display: block;
  transform-origin: top left;
  transform: rotate(-90deg) translate(-100%);
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleLabel {
  user-select: none;
  text-overflow: ellipsis;
  white-space: nowrap;
  overflow: hidden;
}

.jp-AccordionPanel-title .lm-AccordionPanel-titleCollapser {
  transform: rotate(-90deg);
  margin: auto 0;
  height: 16px;
}

.jp-AccordionPanel-title.lm-mod-expanded .lm-AccordionPanel-titleCollapser {
  transform: rotate(0deg);
}

.lm-AccordionPanel .jp-AccordionPanel-toolbar {
  background: none;
  box-shadow: none;
  border: none;
  margin-left: auto;
}

.lm-AccordionPanel .lm-SplitPanel-handle:hover {
  background: var(--jp-layout-color3);
}

.jp-text-truncated {
  overflow: hidden;
  text-overflow: ellipsis;
  white-space: nowrap;
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

.jp-SpinnerContent::before {
  width: 50%;
  height: 50%;
  background: #f37626;
  border-radius: 100% 0 0;
  position: absolute;
  top: 0;
  left: 0;
  content: '';
}

.jp-SpinnerContent::after {
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
  padding: 0 12px;
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

input[type='checkbox'].jp-mod-styled {
  appearance: checkbox;
  -webkit-appearance: checkbox;
  -moz-appearance: checkbox;
  height: auto;
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
  box-sizing: border-box;
  margin-bottom: 12px;
}

.jp-select-wrapper:not(.multiple) {
  height: 28px;
}

.jp-select-wrapper.jp-mod-focused select.jp-mod-styled {
  border: var(--jp-border-width) solid var(--jp-input-active-border-color);
  box-shadow: var(--jp-input-box-shadow);
  background-color: var(--jp-input-active-background);
}

select.jp-mod-styled:hover {
  cursor: pointer;
  color: var(--jp-ui-font-color0);
  background-color: var(--jp-input-hover-background);
  box-shadow: inset 0 0 1px rgba(0, 0, 0, 0.5);
}

select.jp-mod-styled {
  flex: 1 1 auto;
  width: 100%;
  font-size: var(--jp-ui-font-size2);
  background: var(--jp-input-background);
  color: var(--jp-ui-font-color0);
  padding: 0 25px 0 8px;
  border: var(--jp-border-width) solid var(--jp-input-border-color);
  border-radius: 0;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
}

select.jp-mod-styled:not([multiple]) {
  height: 32px;
}

select.jp-mod-styled[multiple] {
  max-height: 200px;
  overflow-y: auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-switch {
  display: flex;
  align-items: center;
  padding-left: 4px;
  padding-right: 4px;
  font-size: var(--jp-ui-font-size1);
  background-color: transparent;
  color: var(--jp-ui-font-color1);
  border: none;
  height: 20px;
}

.jp-switch:hover {
  background-color: var(--jp-layout-color2);
}

.jp-switch-label {
  margin-right: 5px;
  font-family: var(--jp-ui-font-family);
}

.jp-switch-track {
  cursor: pointer;
  background-color: var(--jp-switch-color, var(--jp-border-color1));
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 34px;
  height: 16px;
  width: 35px;
  position: relative;
}

.jp-switch-track::before {
  content: '';
  position: absolute;
  height: 10px;
  width: 10px;
  margin: 3px;
  left: 0;
  background-color: var(--jp-ui-inverse-font-color1);
  -webkit-transition: 0.4s;
  transition: 0.4s;
  border-radius: 50%;
}

.jp-switch[aria-checked='true'] .jp-switch-track {
  background-color: var(--jp-switch-true-position-color, var(--jp-warn-color0));
}

.jp-switch[aria-checked='true'] .jp-switch-track::before {
  /* track width (35) - margins (3 + 3) - thumb width (10) */
  left: 19px;
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
  z-index: 8;
  overflow-x: hidden;
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
  padding: 0;
  margin: 0;
}

button.jp-ToolbarButtonComponent {
  background: var(--jp-layout-color1);
  border: none;
  box-sizing: border-box;
  outline: none;
  appearance: none;
  -webkit-appearance: none;
  -moz-appearance: none;
  padding: 0 6px;
  margin: 0;
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

button.jp-ToolbarButtonComponent > span {
  padding: 0;
  flex: 0 0 auto;
}

button.jp-ToolbarButtonComponent .jp-ToolbarButtonComponent-label {
  font-size: var(--jp-ui-font-size1);
  line-height: 100%;
  padding-left: 2px;
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar.jp-Toolbar-micro {
  padding: 0;
  min-height: 0;
}

#jp-main-dock-panel[data-mode='single-document']
  .jp-MainAreaWidget
  > .jp-Toolbar {
  border: none;
  box-shadow: none;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-WindowedPanel-outer {
  position: relative;
  overflow-y: auto;
}

.jp-WindowedPanel-inner {
  position: relative;
}

.jp-WindowedPanel-window {
  position: absolute;
  left: 0;
  right: 0;
  overflow: visible;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/* Sibling imports */

body {
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
}

/* Disable native link decoration styles everywhere outside of dialog boxes */
a {
  text-decoration: unset;
  color: unset;
}

a:hover {
  text-decoration: unset;
  color: unset;
}

/* Accessibility for links inside dialog box text */
.jp-Dialog-content a {
  text-decoration: revert;
  color: var(--jp-content-link-color);
}

.jp-Dialog-content a:hover {
  text-decoration: revert;
}

/* Styles for ui-components */
.jp-Button {
  color: var(--jp-ui-font-color2);
  border-radius: var(--jp-border-radius);
  padding: 0 12px;
  font-size: var(--jp-ui-font-size1);

  /* Copy from blueprint 3 */
  display: inline-flex;
  flex-direction: row;
  border: none;
  cursor: pointer;
  align-items: center;
  justify-content: center;
  text-align: left;
  vertical-align: middle;
  min-height: 30px;
  min-width: 30px;
}

.jp-Button:disabled {
  cursor: not-allowed;
}

.jp-Button:empty {
  padding: 0 !important;
}

.jp-Button.jp-mod-small {
  min-height: 24px;
  min-width: 24px;
  font-size: 12px;
  padding: 0 7px;
}

/* Use our own theme for hover styles */
.jp-Button.jp-mod-minimal:hover {
  background-color: var(--jp-layout-color2);
}

.jp-Button.jp-mod-minimal {
  background: none;
}

.jp-InputGroup {
  display: block;
  position: relative;
}

.jp-InputGroup input {
  box-sizing: border-box;
  border: none;
  border-radius: 0;
  background-color: transparent;
  color: var(--jp-ui-font-color0);
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
  padding-bottom: 0;
  padding-top: 0;
  padding-left: 10px;
  padding-right: 28px;
  position: relative;
  width: 100%;
  -webkit-appearance: none;
  -moz-appearance: none;
  appearance: none;
  font-size: 14px;
  font-weight: 400;
  height: 30px;
  line-height: 30px;
  outline: none;
  vertical-align: middle;
}

.jp-InputGroup input:focus {
  box-shadow: inset 0 0 0 var(--jp-border-width)
      var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-InputGroup input:disabled {
  cursor: not-allowed;
  resize: block;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input:disabled ~ span {
  cursor: not-allowed;
  color: var(--jp-ui-font-color2);
}

.jp-InputGroup input::placeholder,
input::placeholder {
  color: var(--jp-ui-font-color2);
}

.jp-InputGroupAction {
  position: absolute;
  bottom: 1px;
  right: 0;
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
  font-family: var(--jp-ui-font-family);
  height: 24px;
  line-height: 14px;
  padding: 0 25px 0 10px;
  text-align: left;
  -moz-appearance: none;
  -webkit-appearance: none;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled {
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color2);
  cursor: not-allowed;
  resize: block;
}

.jp-HTMLSelect.jp-DefaultStyle select:disabled ~ span {
  cursor: not-allowed;
}

/* Use our own theme for hover and option styles */
/* stylelint-disable-next-line selector-max-type */
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

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-StatusBar-Widget {
  display: flex;
  align-items: center;
  background: var(--jp-layout-color2);
  min-height: var(--jp-statusbar-height);
  justify-content: space-between;
  padding: 0 10px;
}

.jp-StatusBar-Left {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-StatusBar-Middle {
  display: flex;
  align-items: center;
}

.jp-StatusBar-Right {
  display: flex;
  align-items: center;
  flex-direction: row-reverse;
}

.jp-StatusBar-Item {
  max-height: var(--jp-statusbar-height);
  margin: 0 2px;
  height: var(--jp-statusbar-height);
  white-space: nowrap;
  text-overflow: ellipsis;
  color: var(--jp-ui-font-color1);
  padding: 0 6px;
}

.jp-mod-highlighted:hover {
  background-color: var(--jp-layout-color3);
}

.jp-mod-clicked {
  background-color: var(--jp-brand-color1);
}

.jp-mod-clicked:hover {
  background-color: var(--jp-brand-color0);
}

.jp-mod-clicked .jp-StatusBar-TextItem {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-StatusBar-HoverItem {
  box-shadow: '0px 4px 4px rgba(0, 0, 0, 0.25)';
}

.jp-StatusBar-TextItem {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  line-height: 24px;
  color: var(--jp-ui-font-color1);
}

.jp-StatusBar-GroupItem {
  display: flex;
  align-items: center;
  flex-direction: row;
}

.jp-Statusbar-ProgressCircle svg {
  display: block;
  margin: 0 auto;
  width: 16px;
  height: 24px;
  align-self: normal;
}

.jp-Statusbar-ProgressCircle path {
  fill: var(--jp-inverse-layout-color3);
}

.jp-Statusbar-ProgressBar-progress-bar {
  height: 10px;
  width: 100px;
  border: solid 0.25px var(--jp-brand-color2);
  border-radius: 3px;
  overflow: hidden;
  align-self: center;
}

.jp-Statusbar-ProgressBar-progress-bar > div {
  background-color: var(--jp-brand-color2);
  background-image: linear-gradient(
    -45deg,
    rgba(255, 255, 255, 0.2) 25%,
    transparent 25%,
    transparent 50%,
    rgba(255, 255, 255, 0.2) 50%,
    rgba(255, 255, 255, 0.2) 75%,
    transparent 75%,
    transparent
  );
  background-size: 40px 40px;
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 14px;
  color: #fff;
  text-align: center;
  animation: jp-Statusbar-ExecutionTime-progress-bar 2s linear infinite;
}

.jp-Statusbar-ProgressBar-progress-bar p {
  color: var(--jp-ui-font-color1);
  font-family: var(--jp-ui-font-family);
  font-size: var(--jp-ui-font-size1);
  line-height: 10px;
  width: 100px;
}

@keyframes jp-Statusbar-ExecutionTime-progress-bar {
  0% {
    background-position: 0 0;
  }

  100% {
    background-position: 40px 40px;
  }
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
  padding-bottom: 0;
  color: var(--jp-ui-font-color1);
  background: var(--jp-layout-color1);

  /* This is needed so that all font sizing of children done in ems is
   * relative to this base size */
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Modal variant
|----------------------------------------------------------------------------*/

.jp-ModalCommandPalette {
  position: absolute;
  z-index: 10000;
  top: 38px;
  left: 30%;
  margin: 0;
  padding: 4px;
  width: 40%;
  box-shadow: var(--jp-elevation-z4);
  border-radius: 4px;
  background: var(--jp-layout-color0);
}

.jp-ModalCommandPalette .lm-CommandPalette {
  max-height: 40vh;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-close-icon::after {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-header {
  display: none;
}

.jp-ModalCommandPalette .lm-CommandPalette .lm-CommandPalette-item {
  margin-left: 4px;
  margin-right: 4px;
}

.jp-ModalCommandPalette
  .lm-CommandPalette
  .lm-CommandPalette-item.lm-mod-disabled {
  display: none;
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
  padding: 0 9px;
  background-color: var(--jp-input-active-background);
  height: 30px;
  box-shadow: inset 0 0 0 var(--jp-border-width) var(--jp-input-border-color);
}

.lm-CommandPalette.lm-mod-focused .lm-CommandPalette-wrapper {
  box-shadow: inset 0 0 0 1px var(--jp-input-active-box-shadow-color),
    inset 0 0 0 3px var(--jp-input-active-box-shadow-color);
}

.jp-SearchIconGroup {
  color: white;
  background-color: var(--jp-brand-color1);
  position: absolute;
  top: 4px;
  right: 4px;
  padding: 5px 5px 1px;
}

.jp-SearchIconGroup svg {
  height: 20px;
  width: 20px;
}

.jp-SearchIconGroup .jp-icon3[fill] {
  fill: var(--jp-layout-color0);
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
  color: var(--jp-ui-font-color2);
  font-size: var(--jp-ui-font-size1);
}

/*-----------------------------------------------------------------------------
| Results
|----------------------------------------------------------------------------*/

.lm-CommandPalette-header:first-child {
  margin-top: 0;
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
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item.lm-mod-active {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
}

.lm-CommandPalette-item.lm-mod-active .lm-CommandPalette-itemLabel > mark {
  color: var(--jp-ui-inverse-font-color0);
}

.lm-CommandPalette-item.lm-mod-active .jp-icon-selectable[fill] {
  fill: var(--jp-layout-color0);
}

.lm-CommandPalette-item.lm-mod-active:hover:not(.lm-mod-disabled) {
  color: var(--jp-ui-inverse-font-color1);
  background: var(--jp-brand-color1);
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
  color: var(--jp-ui-font-color2);
}

.lm-CommandPalette-item .lm-CommandPalette-itemIcon {
  margin: 0 4px 0 0;
  position: relative;
  width: 16px;
  top: 2px;
  flex: 0 0 auto;
}

.lm-CommandPalette-item.lm-mod-disabled .lm-CommandPalette-itemIcon {
  opacity: 0.6;
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

.lm-CommandPalette-content:empty::after {
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
  padding: 0 8px;
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
  top: 0;
  left: 0;
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
  padding: 24px 24px 12px;
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
  resize: both;
}

.jp-Dialog-content.jp-Dialog-content-small {
  max-width: 500px;
}

.jp-Dialog-button {
  overflow: visible;
}

button.jp-Dialog-button:focus {
  outline: 1px solid var(--jp-brand-color1);
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button:focus::-moz-focus-inner {
  border: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus,
button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline-offset: 4px;
  -moz-outline-radius: 0;
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-accept:focus {
  outline: 1px solid var(--jp-accept-color-normal, var(--jp-brand-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-warn:focus {
  outline: 1px solid var(--jp-warn-color-normal, var(--jp-error-color1));
}

button.jp-Dialog-button.jp-mod-styled.jp-mod-reject:focus {
  outline: 1px solid var(--jp-reject-color-normal, var(--md-grey-600));
}

button.jp-Dialog-close-button {
  padding: 0;
  height: 100%;
  min-width: unset;
  min-height: unset;
}

.jp-Dialog-header {
  display: flex;
  justify-content: space-between;
  flex: 0 0 auto;
  padding-bottom: 12px;
  font-size: var(--jp-ui-font-size3);
  font-weight: 400;
  color: var(--jp-ui-font-color1);
}

.jp-Dialog-body {
  display: flex;
  flex-direction: column;
  flex: 1 1 auto;
  font-size: var(--jp-ui-font-size1);
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  overflow: auto;
}

.jp-Dialog-footer {
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  flex: 0 0 auto;
  margin-left: -12px;
  margin-right: -12px;
  padding: 12px;
}

.jp-Dialog-checkbox {
  padding-right: 5px;
}

.jp-Dialog-checkbox > input:focus-visible {
  outline: 1px solid var(--jp-input-active-border-color);
  outline-offset: 1px;
}

.jp-Dialog-spacer {
  flex: 1 1 auto;
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
  padding: 0 16px;
}

.jp-Dialog-body > label {
  line-height: 1.4;
  color: var(--jp-ui-font-color0);
}

.jp-Dialog-button.jp-mod-styled:not(:last-child) {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Input-Boolean-Dialog {
  flex-direction: row-reverse;
  align-items: end;
  width: 100%;
}

.jp-Input-Boolean-Dialog > label {
  flex: 1 1 auto;
}

/*-----------------------------------------------------------------------------
| Copyright (c) 2014-2016, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-MainAreaWidget > :focus {
  outline: none;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error {
  padding: 6px;
}

.jp-MainAreaWidget .jp-MainAreaWidget-error > pre {
  width: auto;
  padding: 10px;
  background: var(--jp-error-color3);
  border: var(--jp-border-width) solid var(--jp-error-color1);
  border-radius: var(--jp-border-radius);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  white-space: pre-wrap;
  word-wrap: break-word;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

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
  --md-purple-A700: #a0f;
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
  --md-yellow-A200: #ff0;
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
  --md-grey-200: #eee;
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
| Copyright (c) 2014-2017, Jupyter Development Team.
|
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| RenderedText
|----------------------------------------------------------------------------*/

:root {
  /* This is the padding value to fill the gaps between lines containing spans with background color. */
  --jp-private-code-span-padding: calc(
    (var(--jp-code-line-height) - 1) * var(--jp-code-font-size) / 2
  );
}

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
  margin: 0;
  padding: 0;
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
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-bg {
  background-color: #e75c58;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-bg {
  background-color: #00a250;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-bg {
  background-color: #ddb62b;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-bg {
  background-color: #208ffb;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-bg {
  background-color: #d160c4;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-bg {
  background-color: #60c6c8;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-bg {
  background-color: #c5c1b4;
  padding: var(--jp-private-code-span-padding) 0;
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
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-red-intense-bg {
  background-color: #b22b31;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-green-intense-bg {
  background-color: #007427;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-yellow-intense-bg {
  background-color: #b27d12;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-blue-intense-bg {
  background-color: #0065ca;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-magenta-intense-bg {
  background-color: #a03196;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-cyan-intense-bg {
  background-color: #258f8f;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-white-intense-bg {
  background-color: #a1a6b2;
  padding: var(--jp-private-code-span-padding) 0;
}

.jp-RenderedText pre .ansi-default-inverse-fg {
  color: var(--jp-ui-inverse-font-color0);
}

.jp-RenderedText pre .ansi-default-inverse-bg {
  background-color: var(--jp-inverse-layout-color0);
  padding: var(--jp-private-code-span-padding) 0;
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

/* stylelint-disable selector-max-type, selector-max-compound-selectors */

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
  margin-bottom: 0;
}

/* stylelint-enable selector-max-type, selector-max-compound-selectors */

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
  font-size: var(--jp-ui-font-size1);
  table-layout: fixed;
  margin-left: auto;
  margin-bottom: 1em;
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
  padding: 0.5em;
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

.jp-RenderedHTMLCommon p {
  text-align: left;
  margin: 0;
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
  font-size: var(--jp-ui-font-size0);
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

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Copyright (c) 2014-2017, PhosphorJS Contributors
|
| Distributed under the terms of the BSD 3-Clause License.
|
| The full license is in the file LICENSE, distributed with this software.
|----------------------------------------------------------------------------*/

.lm-cursor-backdrop {
  position: fixed;
  width: 200px;
  height: 200px;
  margin-top: -100px;
  margin-left: -100px;
  will-change: transform;
  z-index: 100;
}

.lm-mod-drag-image {
  will-change: transform;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-lineFormSearch {
  padding: 4px 12px;
  background-color: var(--jp-layout-color2);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
  font-size: var(--jp-ui-font-size1);
}

.jp-lineFormCaption {
  font-size: var(--jp-ui-font-size0);
  line-height: var(--jp-ui-font-size1);
  margin-top: 4px;
  color: var(--jp-ui-font-color0);
}

.jp-baseLineForm {
  border: none;
  border-radius: 0;
  position: absolute;
  background-size: 16px;
  background-repeat: no-repeat;
  background-position: center;
  outline: none;
}

.jp-lineFormButtonContainer {
  top: 4px;
  right: 8px;
  height: 24px;
  padding: 0 12px;
  width: 12px;
}

.jp-lineFormButtonIcon {
  top: 0;
  right: 0;
  background-color: var(--jp-brand-color1);
  height: 100%;
  width: 100%;
  box-sizing: border-box;
  padding: 4px 6px;
}

.jp-lineFormButton {
  top: 0;
  right: 0;
  background-color: transparent;
  height: 100%;
  width: 100%;
  box-sizing: border-box;
}

.jp-lineFormWrapper {
  overflow: hidden;
  padding: 0 8px;
  border: 1px solid var(--jp-border-color0);
  background-color: var(--jp-input-active-background);
  height: 22px;
}

.jp-lineFormWrapperFocusWithin {
  border: var(--jp-border-width) solid var(--md-blue-500);
  box-shadow: inset 0 0 4px var(--md-blue-300);
}

.jp-lineFormInput {
  background: transparent;
  width: 200px;
  height: 100%;
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  line-height: 28px;
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
  border-radius: 0;
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
.jp-DocumentSearch-input {
  border: none;
  outline: none;
  color: var(--jp-ui-font-color0);
  font-size: var(--jp-ui-font-size1);
  background-color: var(--jp-layout-color0);
  font-family: var(--jp-ui-font-family);
  padding: 2px 1px;
  resize: none;
}

.jp-DocumentSearch-overlay {
  position: absolute;
  background-color: var(--jp-toolbar-background);
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  border-left: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  top: 0;
  right: 0;
  z-index: 7;
  min-width: 405px;
  padding: 2px;
  font-size: var(--jp-ui-font-size1);

  --jp-private-document-search-button-height: 20px;
}

.jp-DocumentSearch-overlay button {
  background-color: var(--jp-toolbar-background);
  outline: 0;
}

.jp-DocumentSearch-overlay button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-overlay button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-overlay-row {
  display: flex;
  align-items: center;
  margin-bottom: 2px;
}

.jp-DocumentSearch-button-content {
  display: inline-block;
  cursor: pointer;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-button-content svg {
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-input-wrapper {
  border: var(--jp-border-width) solid var(--jp-border-color0);
  display: flex;
  background-color: var(--jp-layout-color0);
  margin: 2px;
}

.jp-DocumentSearch-input-wrapper:focus-within {
  border-color: var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper {
  all: initial;
  overflow: hidden;
  display: inline-block;
  border: none;
  box-sizing: border-box;
}

.jp-DocumentSearch-toggle-wrapper {
  width: 14px;
  height: 14px;
}

.jp-DocumentSearch-button-wrapper {
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
}

.jp-DocumentSearch-toggle-wrapper:focus,
.jp-DocumentSearch-button-wrapper:focus {
  outline: var(--jp-border-width) solid
    var(--jp-cell-editor-active-border-color);
  outline-offset: -1px;
}

.jp-DocumentSearch-toggle-wrapper,
.jp-DocumentSearch-button-wrapper,
.jp-DocumentSearch-button-content:focus {
  outline: none;
}

.jp-DocumentSearch-toggle-placeholder {
  width: 5px;
}

.jp-DocumentSearch-input-button::before {
  display: block;
  padding-top: 100%;
}

.jp-DocumentSearch-input-button-off {
  opacity: var(--jp-search-toggle-off-opacity);
}

.jp-DocumentSearch-input-button-off:hover {
  opacity: var(--jp-search-toggle-hover-opacity);
}

.jp-DocumentSearch-input-button-on {
  opacity: var(--jp-search-toggle-on-opacity);
}

.jp-DocumentSearch-index-counter {
  padding-left: 10px;
  padding-right: 10px;
  user-select: none;
  min-width: 35px;
  display: inline-block;
}

.jp-DocumentSearch-up-down-wrapper {
  display: inline-block;
  padding-right: 2px;
  margin-left: auto;
  white-space: nowrap;
}

.jp-DocumentSearch-spacer {
  margin-left: auto;
}

.jp-DocumentSearch-up-down-wrapper button {
  outline: 0;
  border: none;
  width: var(--jp-private-document-search-button-height);
  height: var(--jp-private-document-search-button-height);
  vertical-align: middle;
  margin: 1px 5px 2px;
}

.jp-DocumentSearch-up-down-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-up-down-button:active {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-filter-button {
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-filter-button:hover {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled {
  background-color: var(--jp-layout-color2);
}

.jp-DocumentSearch-filter-button-enabled:hover {
  background-color: var(--jp-layout-color3);
}

.jp-DocumentSearch-search-options {
  padding: 0 8px;
  margin-left: 3px;
  width: 100%;
  display: grid;
  justify-content: start;
  grid-template-columns: 1fr 1fr;
  align-items: center;
  justify-items: stretch;
}

.jp-DocumentSearch-search-filter-disabled {
  color: var(--jp-ui-font-color2);
}

.jp-DocumentSearch-search-filter {
  display: flex;
  align-items: center;
  user-select: none;
}

.jp-DocumentSearch-regex-error {
  color: var(--jp-error-color0);
}

.jp-DocumentSearch-replace-button-wrapper {
  overflow: hidden;
  display: inline-block;
  box-sizing: border-box;
  border: var(--jp-border-width) solid var(--jp-border-color0);
  margin: auto 2px;
  padding: 1px 4px;
  height: calc(var(--jp-private-document-search-button-height) + 2px);
}

.jp-DocumentSearch-replace-button-wrapper:focus {
  border: var(--jp-border-width) solid var(--jp-cell-editor-active-border-color);
}

.jp-DocumentSearch-replace-button {
  display: inline-block;
  text-align: center;
  cursor: pointer;
  box-sizing: border-box;
  color: var(--jp-ui-font-color1);

  /* height - 2 * (padding of wrapper) */
  line-height: calc(var(--jp-private-document-search-button-height) - 2px);
  width: 100%;
  height: 100%;
}

.jp-DocumentSearch-replace-button:focus {
  outline: none;
}

.jp-DocumentSearch-replace-wrapper-class {
  margin-left: 14px;
  display: flex;
}

.jp-DocumentSearch-replace-toggle {
  border: none;
  background-color: var(--jp-toolbar-background);
  border-radius: var(--jp-border-radius);
}

.jp-DocumentSearch-replace-toggle:hover {
  background-color: var(--jp-layout-color2);
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.cm-editor {
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  font-family: var(--jp-code-font-family);
  border: 0;
  border-radius: 0;
  height: auto;

  /* Changed to auto to autogrow */
}

.cm-editor pre {
  padding: 0 var(--jp-code-padding);
}

.jp-CodeMirrorEditor[data-type='inline'] .cm-dialog {
  background-color: var(--jp-layout-color0);
  color: var(--jp-content-font-color1);
}

.jp-CodeMirrorEditor {
  cursor: text;
}

/* When zoomed out 67% and 33% on a screen of 1440 width x 900 height */
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width1) solid
      var(--jp-editor-cursor-color);
  }
}

/* When zoomed out less than 33% */
@media screen and (min-width: 4320px) {
  .jp-CodeMirrorEditor[data-type='inline'] .cm-cursor {
    border-left: var(--jp-code-cursor-width2) solid
      var(--jp-editor-cursor-color);
  }
}

.cm-editor.jp-mod-readOnly .cm-cursor {
  display: none;
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

.cm-searching,
.cm-searching span {
  /* `.cm-searching span`: we need to override syntax highlighting */
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.cm-searching::selection,
.cm-searching span::selection {
  background-color: var(--jp-search-unselected-match-background-color);
  color: var(--jp-search-unselected-match-color);
}

.jp-current-match > .cm-searching,
.jp-current-match > .cm-searching span,
.cm-searching > .jp-current-match,
.cm-searching > .jp-current-match span {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.jp-current-match > .cm-searching::selection,
.cm-searching > .jp-current-match::selection,
.jp-current-match > .cm-searching span::selection {
  background-color: var(--jp-search-selected-match-background-color);
  color: var(--jp-search-selected-match-color);
}

.cm-trailingspace {
  background-image: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAAgAAAAFCAYAAAB4ka1VAAAAsElEQVQIHQGlAFr/AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA7+r3zKmT0/+pk9P/7+r3zAAAAAAAAAAABAAAAAAAAAAA6OPzM+/q9wAAAAAA6OPzMwAAAAAAAAAAAgAAAAAAAAAAGR8NiRQaCgAZIA0AGR8NiQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQyoYJ/SY80UAAAAASUVORK5CYII=);
  background-position: center left;
  background-repeat: repeat-x;
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

/* Styles for shared cursors (remote cursor locations and selected ranges) */
.jp-CodeMirrorEditor .cm-ySelectionCaret {
  position: relative;
  border-left: 1px solid black;
  margin-left: -1px;
  margin-right: -1px;
  box-sizing: border-box;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret > .cm-ySelectionInfo {
  white-space: nowrap;
  position: absolute;
  top: -1.15em;
  padding-bottom: 0.05em;
  left: -1px;
  font-size: 0.95em;
  font-family: var(--jp-ui-font-family);
  font-weight: bold;
  line-height: normal;
  user-select: none;
  color: white;
  padding-left: 2px;
  padding-right: 2px;
  z-index: 101;
  transition: opacity 0.3s ease-in-out;
}

.jp-CodeMirrorEditor .cm-ySelectionInfo {
  transition-delay: 0.7s;
  opacity: 0;
}

.jp-CodeMirrorEditor .cm-ySelectionCaret:hover > .cm-ySelectionInfo {
  opacity: 1;
  transition-delay: 0s;
}

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

.jp-FileBrowser .jp-SidePanel-content {
  display: flex;
  flex-direction: column;
}

.jp-FileBrowser-toolbar.jp-Toolbar {
  flex-wrap: wrap;
  row-gap: 12px;
  border-bottom: none;
  height: auto;
  margin: 8px 12px 0;
  box-shadow: none;
  padding: 0;
  justify-content: flex-start;
}

.jp-FileBrowser-Panel {
  flex: 1 1 auto;
  display: flex;
  flex-direction: column;
}

.jp-BreadCrumbs {
  flex: 0 0 auto;
  margin: 8px 12px;
}

.jp-BreadCrumbs-item {
  margin: 0 2px;
  padding: 0 2px;
  border-radius: var(--jp-border-radius);
  cursor: pointer;
}

.jp-BreadCrumbs-item:hover {
  background-color: var(--jp-layout-color2);
}

.jp-BreadCrumbs-item:first-child {
  margin-left: 0;
}

.jp-BreadCrumbs-item.jp-mod-dropTarget {
  background-color: var(--jp-brand-color2);
  opacity: 0.7;
}

/*-----------------------------------------------------------------------------
| Buttons
|----------------------------------------------------------------------------*/

.jp-FileBrowser-toolbar > .jp-Toolbar-item {
  flex: 0 0 auto;
  padding-left: 0;
  padding-right: 2px;
  align-items: center;
  height: unset;
}

.jp-FileBrowser-toolbar > .jp-Toolbar-item .jp-ToolbarButtonComponent {
  width: 40px;
}

/*-----------------------------------------------------------------------------
| Other styles
|----------------------------------------------------------------------------*/

.jp-FileDialog.jp-mod-conflict input {
  color: var(--jp-error-color1);
}

.jp-FileDialog .jp-new-name-title {
  margin-top: 12px;
}

.jp-LastModified-hidden {
  display: none;
}

.jp-FileSize-hidden {
  display: none;
}

.jp-FileBrowser .lm-AccordionPanel > h3:first-child {
  display: none;
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
  align-items: center;
  overflow: hidden;
  border-top: var(--jp-border-width) solid var(--jp-border-color2);
  border-bottom: var(--jp-border-width) solid var(--jp-border-color1);
  box-shadow: var(--jp-toolbar-box-shadow);
  z-index: 2;
}

.jp-DirListing-headerItem {
  padding: 4px 12px 2px;
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

.jp-DirListing-headerItem.jp-id-filesize {
  flex: 0 0 75px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
}

.jp-id-narrow {
  display: none;
  flex: 0 0 5px;
  padding: 4px;
  border-left: var(--jp-border-width) solid var(--jp-border-color2);
  text-align: right;
  color: var(--jp-border-color2);
}

.jp-DirListing-narrow .jp-id-narrow {
  display: block;
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

.jp-DirListing-content mark {
  color: var(--jp-ui-font-color0);
  background-color: transparent;
  font-weight: bold;
}

.jp-DirListing-content .jp-DirListing-item.jp-mod-selected mark {
  color: var(--jp-ui-inverse-font-color0);
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
  align-items: center;
  padding: 4px 12px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-DirListing-checkboxWrapper {
  /* Increases hit area of checkbox. */
  padding: 4px;
}

.jp-DirListing-header
  .jp-DirListing-checkboxWrapper
  + .jp-DirListing-headerItem {
  padding-left: 4px;
}

.jp-DirListing-content .jp-DirListing-checkboxWrapper {
  position: relative;
  left: -4px;
  margin: -4px 0 -4px -8px;
}

.jp-DirListing-checkboxWrapper.jp-mod-visible {
  visibility: visible;
}

/* For devices that support hovering, hide checkboxes until hovered, selected...
*/
@media (hover: hover) {
  .jp-DirListing-checkboxWrapper {
    visibility: hidden;
  }

  .jp-DirListing-item:hover .jp-DirListing-checkboxWrapper,
  .jp-DirListing-item.jp-mod-selected .jp-DirListing-checkboxWrapper {
    visibility: visible;
  }
}

.jp-DirListing-item[data-is-dot] {
  opacity: 75%;
}

.jp-DirListing-item.jp-mod-selected {
  color: var(--jp-ui-inverse-font-color1);
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

.jp-DirListing-itemText:focus {
  outline-width: 2px;
  outline-color: var(--jp-inverse-layout-color1);
  outline-style: solid;
  outline-offset: 1px;
}

.jp-DirListing-item.jp-mod-selected .jp-DirListing-itemText:focus {
  outline-color: var(--jp-layout-color1);
}

.jp-DirListing-itemModified {
  flex: 0 0 125px;
  text-align: right;
}

.jp-DirListing-itemFileSize {
  flex: 0 0 90px;
  text-align: right;
}

.jp-DirListing-editor {
  flex: 1 0 64px;
  outline: none;
  border: none;
  color: var(--jp-ui-font-color1);
  background-color: var(--jp-layout-color1);
}

.jp-DirListing-item.jp-mod-running .jp-DirListing-itemIcon::before {
  color: var(--jp-success-color1);
  content: '\25CF';
  font-size: 8px;
  position: absolute;
  left: -8px;
}

.jp-DirListing-item.jp-mod-running.jp-mod-selected
  .jp-DirListing-itemIcon::before {
  color: var(--jp-ui-inverse-font-color1);
}

.jp-DirListing-item.lm-mod-drag-image,
.jp-DirListing-item.jp-mod-selected.lm-mod-drag-image {
  font-size: var(--jp-ui-font-size1);
  padding-left: 4px;
  margin-left: 4px;
  width: 160px;
  background-color: var(--jp-ui-inverse-font-color2);
  box-shadow: var(--jp-elevation-z2);
  border-radius: 0;
  color: var(--jp-ui-font-color1);
  transform: translateX(-40%) translateY(-58%);
}

.jp-Document {
  min-width: 120px;
  min-height: 120px;
  outline: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Main OutputArea
| OutputArea has a list of Outputs
|----------------------------------------------------------------------------*/

.jp-OutputArea {
  overflow-y: auto;
}

.jp-OutputArea-child {
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-OutputPrompt {
  width: var(--jp-cell-prompt-width);
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

.jp-OutputArea-prompt {
  display: table-cell;
  vertical-align: top;
}

.jp-OutputArea-output {
  display: table-cell;
  width: 100%;
  height: auto;
  overflow: auto;
  user-select: text;
  -moz-user-select: text;
  -webkit-user-select: text;
  -ms-user-select: text;
}

.jp-OutputArea .jp-RenderedText {
  padding-left: 1ch;
}

/**
 * Prompt overlay.
 */

.jp-OutputArea-promptOverlay {
  position: absolute;
  top: 0;
  width: var(--jp-cell-prompt-width);
  height: 100%;
  opacity: 0.5;
}

.jp-OutputArea-promptOverlay:hover {
  background: var(--jp-layout-color2);
  box-shadow: inset 0 0 1px var(--jp-inverse-layout-color0);
  cursor: zoom-out;
}

.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay:hover {
  cursor: zoom-in;
}

/**
 * Isolated output.
 */
.jp-OutputArea-output.jp-mod-isolated {
  width: 100%;
  display: block;
}

/*
When drag events occur, `lm-mod-override-cursor` is added to the body.
Because iframes steal all cursor events, the following two rules are necessary
to suppress pointer events while resize drags are occurring. There may be a
better solution to this problem.
*/
body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated {
  position: relative;
}

body.lm-mod-override-cursor .jp-OutputArea-output.jp-mod-isolated::before {
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
  margin: 0;
  padding: 0;
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

.jp-TrimmedOutputs pre {
  background: var(--jp-layout-color3);
  font-size: calc(var(--jp-code-font-size) * 1.4);
  text-align: center;
  text-transform: uppercase;
}

/* Hide the gutter in case of
 *  - nested output areas (e.g. in the case of output widgets)
 *  - mirrored output areas
 */
.jp-OutputArea .jp-OutputArea .jp-OutputArea-prompt {
  display: none;
}

/* Hide empty lines in the output area, for instance due to cleared widgets */
.jp-OutputArea-prompt:empty {
  padding: 0;
  border: 0;
}

/*-----------------------------------------------------------------------------
| executeResult is added to any Output-result for the display of the object
| returned by a cell
|----------------------------------------------------------------------------*/

.jp-OutputArea-output.jp-OutputArea-executeResult {
  margin-left: 0;
  width: 100%;
}

/* Text output with the Out[] prompt needs a top padding to match the
 * alignment of the Out[] prompt itself.
 */
.jp-OutputArea-executeResult .jp-RenderedText.jp-OutputArea-output {
  padding-top: var(--jp-code-padding);
  border-top: var(--jp-border-width) solid transparent;
}

/*-----------------------------------------------------------------------------
| The Stdin output
|----------------------------------------------------------------------------*/

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
  padding: 0 0.25em;
  margin: 0 0.25em;
  flex: 0 0 70%;
}

.jp-Stdin-input::placeholder {
  opacity: 0;
}

.jp-Stdin-input:focus {
  box-shadow: none;
}

.jp-Stdin-input:focus::placeholder {
  opacity: 1;
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
| Printing
|----------------------------------------------------------------------------*/

@media print {
  .jp-OutputArea-child {
    break-inside: avoid-page;
  }
}

/*-----------------------------------------------------------------------------
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-OutputPrompt {
    display: table-row;
    text-align: left;
  }

  .jp-OutputArea-child .jp-OutputArea-output {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }
}

/* Trimmed outputs warning */
.jp-TrimmedOutputs > a {
  margin: 10px;
  text-decoration: none;
  cursor: pointer;
}

.jp-TrimmedOutputs > a:hover {
  text-decoration: none;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Table of Contents
|----------------------------------------------------------------------------*/

:root {
  --jp-private-toc-active-width: 4px;
}

.jp-TableOfContents {
  display: flex;
  flex-direction: column;
  background: var(--jp-layout-color1);
  color: var(--jp-ui-font-color1);
  font-size: var(--jp-ui-font-size1);
  height: 100%;
}

.jp-TableOfContents-placeholder {
  text-align: center;
}

.jp-TableOfContents-placeholderContent {
  color: var(--jp-content-font-color2);
  padding: 8px;
}

.jp-TableOfContents-placeholderContent > h3 {
  margin-bottom: var(--jp-content-heading-margin-bottom);
}

.jp-TableOfContents .jp-SidePanel-content {
  overflow-y: auto;
}

.jp-TableOfContents-tree {
  margin: 4px;
}

.jp-TableOfContents ol {
  list-style-type: none;
}

/* stylelint-disable-next-line selector-max-type */
.jp-TableOfContents li > ol {
  /* Align left border with triangle icon center */
  padding-left: 11px;
}

.jp-TableOfContents-content {
  /* left margin for the active heading indicator */
  margin: 0 0 0 var(--jp-private-toc-active-width);
  padding: 0;
  background-color: var(--jp-layout-color1);
}

.jp-tocItem {
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}

.jp-tocItem-heading {
  display: flex;
  cursor: pointer;
}

.jp-tocItem-heading:hover {
  background-color: var(--jp-layout-color2);
}

.jp-tocItem-content {
  display: block;
  padding: 4px 0;
  white-space: nowrap;
  text-overflow: ellipsis;
  overflow-x: hidden;
}

.jp-tocItem-collapser {
  height: 20px;
  margin: 2px 2px 0;
  padding: 0;
  background: none;
  border: none;
  cursor: pointer;
}

.jp-tocItem-collapser:hover {
  background-color: var(--jp-layout-color3);
}

/* Active heading indicator */

.jp-tocItem-heading::before {
  content: ' ';
  background: transparent;
  width: var(--jp-private-toc-active-width);
  height: 24px;
  position: absolute;
  left: 0;
  border-radius: var(--jp-border-radius);
}

.jp-tocItem-heading.jp-tocItem-active::before {
  background-color: var(--jp-brand-color1);
}

.jp-tocItem-heading:hover.jp-tocItem-active::before {
  background: var(--jp-brand-color0);
  opacity: 1;
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

.jp-Collapser {
  flex: 0 0 var(--jp-cell-collapser-width);
  padding: 0;
  margin: 0;
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
  top: 0;
  bottom: 0;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Hiding collapsers in print mode.

Note: input and output wrappers have "display: block" propery in print mode.
*/

@media print {
  .jp-Collapser {
    display: none;
  }
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
  height: 0;
  width: 100%;
  padding: 0;
  margin: 0;
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
  display: table;
  table-layout: fixed;
  width: 100%;
  overflow: hidden;
}

.jp-InputArea-editor {
  display: table-cell;
  overflow: hidden;
  vertical-align: top;

  /* This is the non-active, default styling */
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  background: var(--jp-cell-editor-background);
}

.jp-InputPrompt {
  display: table-cell;
  vertical-align: top;
  width: var(--jp-cell-prompt-width);
  color: var(--jp-cell-inprompt-font-color);
  font-family: var(--jp-cell-prompt-font-family);
  padding: var(--jp-code-padding);
  letter-spacing: var(--jp-cell-prompt-letter-spacing);
  opacity: var(--jp-cell-prompt-opacity);
  line-height: var(--jp-code-line-height);
  font-size: var(--jp-code-font-size);
  border: var(--jp-border-width) solid transparent;

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
| Mobile
|----------------------------------------------------------------------------*/
@media only screen and (max-width: 760px) {
  .jp-InputArea-editor {
    display: table-row;
    margin-left: var(--jp-notebook-padding);
  }

  .jp-InputPrompt {
    display: table-row;
    text-align: left;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Placeholder {
  display: table;
  table-layout: fixed;
  width: 100%;
}

.jp-Placeholder-prompt {
  display: table-cell;
  box-sizing: border-box;
}

.jp-Placeholder-content {
  display: table-cell;
  padding: 4px 6px;
  border: 1px solid transparent;
  border-radius: 0;
  background: none;
  box-sizing: border-box;
  cursor: pointer;
}

.jp-Placeholder-contentContainer {
  display: flex;
}

.jp-Placeholder-content:hover,
.jp-InputPlaceholder > .jp-Placeholder-content:hover {
  border-color: var(--jp-layout-color3);
}

.jp-Placeholder-content .jp-MoreHorizIcon {
  width: 32px;
  height: 16px;
  border: 1px solid transparent;
  border-radius: var(--jp-border-radius);
}

.jp-Placeholder-content .jp-MoreHorizIcon:hover {
  border: 1px solid var(--jp-border-color1);
  box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.25);
  background-color: var(--jp-layout-color0);
}

.jp-PlaceholderText {
  white-space: nowrap;
  overflow-x: hidden;
  color: var(--jp-inverse-layout-color3);
  font-family: var(--jp-code-font-family);
}

.jp-InputPlaceholder > .jp-Placeholder-content {
  border-color: var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
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
  margin: 0;
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
  padding: 0;
  margin: 0;

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

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea {
  overflow-y: auto;
  max-height: 24em;
  margin-left: var(--jp-private-cell-scrolling-output-offset);
  resize: vertical;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea[style*='height'] {
  max-height: unset;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-Cell-outputArea::after {
  content: ' ';
  box-shadow: inset 0 0 6px 2px rgb(0 0 0 / 30%);
  width: 100%;
  height: 100%;
  position: sticky;
  bottom: 0;
  top: 0;
  margin-top: -50%;
  float: left;
  display: block;
  pointer-events: none;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-child {
  padding-top: 6px;
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-prompt {
  width: calc(
    var(--jp-cell-prompt-width) - var(--jp-private-cell-scrolling-output-offset)
  );
}

.jp-CodeCell.jp-mod-outputsScrolled .jp-OutputArea-promptOverlay {
  left: calc(-1 * var(--jp-private-cell-scrolling-output-offset));
}

/*-----------------------------------------------------------------------------
| CodeCell
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| MarkdownCell
|----------------------------------------------------------------------------*/

.jp-MarkdownOutput {
  display: table-cell;
  width: 100%;
  margin-top: 0;
  margin-bottom: 0;
  padding-left: var(--jp-code-padding);
}

.jp-MarkdownOutput.jp-RenderedHTMLCommon {
  overflow: auto;
}

/* collapseHeadingButton (show always if hiddenCellsButton is _not_ shown) */
.jp-collapseHeadingButton {
  display: flex;
  min-height: var(--jp-cell-collapser-min-height);
  font-size: var(--jp-code-font-size);
  position: absolute;
  background-color: transparent;
  background-size: 25px;
  background-repeat: no-repeat;
  background-position-x: center;
  background-position-y: top;
  background-image: var(--jp-icon-caret-down);
  right: 0;
  top: 0;
  bottom: 0;
}

.jp-collapseHeadingButton.jp-mod-collapsed {
  background-image: var(--jp-icon-caret-right);
}

/*
 set the container font size to match that of content
 so that the nested collapse buttons have the right size
*/
.jp-MarkdownCell .jp-InputPrompt {
  font-size: var(--jp-content-font-size1);
}

/*
  Align collapseHeadingButton with cell top header
  The font sizes are identical to the ones in packages/rendermime/style/base.css
*/
.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='1'] {
  font-size: var(--jp-content-font-size5);
  background-position-y: calc(0.3 * var(--jp-content-font-size5));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='2'] {
  font-size: var(--jp-content-font-size4);
  background-position-y: calc(0.3 * var(--jp-content-font-size4));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='3'] {
  font-size: var(--jp-content-font-size3);
  background-position-y: calc(0.3 * var(--jp-content-font-size3));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='4'] {
  font-size: var(--jp-content-font-size2);
  background-position-y: calc(0.3 * var(--jp-content-font-size2));
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='5'] {
  font-size: var(--jp-content-font-size1);
  background-position-y: top;
}

.jp-mod-rendered .jp-collapseHeadingButton[data-heading-level='6'] {
  font-size: var(--jp-content-font-size0);
  background-position-y: top;
}

/* collapseHeadingButton (show only on (hover,active) if hiddenCellsButton is shown) */
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-collapseHeadingButton {
  display: none;
}

.jp-Notebook.jp-mod-showHiddenCellsButton
  :is(.jp-MarkdownCell:hover, .jp-mod-active)
  .jp-collapseHeadingButton {
  display: flex;
}

/* showHiddenCellsButton (only show if jp-mod-showHiddenCellsButton is set, which
is a consequence of the showHiddenCellsButton option in Notebook Settings)*/
.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton {
  margin-left: calc(var(--jp-cell-prompt-width) + 2 * var(--jp-code-padding));
  margin-top: var(--jp-code-padding);
  border: 1px solid var(--jp-border-color2);
  background-color: var(--jp-border-color3) !important;
  color: var(--jp-content-font-color0) !important;
  display: flex;
}

.jp-Notebook.jp-mod-showHiddenCellsButton .jp-showHiddenCellsButton:hover {
  background-color: var(--jp-border-color2) !important;
}

.jp-showHiddenCellsButton {
  display: none;
}

/*-----------------------------------------------------------------------------
| Printing
|----------------------------------------------------------------------------*/

/*
Using block instead of flex to allow the use of the break-inside CSS property for
cell outputs.
*/

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}

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
  --jp-notebook-toolbar-padding: 2px 5px 2px 2px;
}

/*-----------------------------------------------------------------------------

/*-----------------------------------------------------------------------------
| Styles
|----------------------------------------------------------------------------*/

.jp-NotebookPanel-toolbar {
  padding: var(--jp-notebook-toolbar-padding);

  /* disable paint containment from lumino 2.0 default strict CSS containment */
  contain: style size !important;
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

.jp-Toolbar-responsive-popup {
  position: absolute;
  height: fit-content;
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  justify-content: flex-end;
  border-bottom: var(--jp-border-width) solid var(--jp-toolbar-border-color);
  box-shadow: var(--jp-toolbar-box-shadow);
  background: var(--jp-toolbar-background);
  min-height: var(--jp-toolbar-micro-height);
  padding: var(--jp-notebook-toolbar-padding);
  z-index: 1;
  right: 0;
  top: 0;
}

.jp-Toolbar > .jp-Toolbar-responsive-opener {
  margin-left: auto;
}

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

.jp-Notebook-ExecutionIndicator {
  position: relative;
  display: inline-block;
  height: 100%;
  z-index: 9997;
}

.jp-Notebook-ExecutionIndicator-tooltip {
  visibility: hidden;
  height: auto;
  width: max-content;
  width: -moz-max-content;
  background-color: var(--jp-layout-color2);
  color: var(--jp-ui-font-color1);
  text-align: justify;
  border-radius: 6px;
  padding: 0 5px;
  position: fixed;
  display: table;
}

.jp-Notebook-ExecutionIndicator-tooltip.up {
  transform: translateX(-50%) translateY(-100%) translateY(-32px);
}

.jp-Notebook-ExecutionIndicator-tooltip.down {
  transform: translateX(calc(-100% + 16px)) translateY(5px);
}

.jp-Notebook-ExecutionIndicator-tooltip.hidden {
  display: none;
}

.jp-Notebook-ExecutionIndicator:hover .jp-Notebook-ExecutionIndicator-tooltip {
  visibility: visible;
}

.jp-Notebook-ExecutionIndicator span {
  font-size: var(--jp-ui-font-size1);
  font-family: var(--jp-ui-font-family);
  color: var(--jp-ui-font-color1);
  line-height: 24px;
  display: block;
}

.jp-Notebook-ExecutionIndicator-progress-bar {
  display: flex;
  justify-content: center;
  height: 100%;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

/*
 * Execution indicator
 */
.jp-tocItem-content::after {
  content: '';

  /* Must be identical to form a circle */
  width: 12px;
  height: 12px;
  background: none;
  border: none;
  position: absolute;
  right: 0;
}

.jp-tocItem-content[data-running='0']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background: none;
}

.jp-tocItem-content[data-running='1']::after {
  border-radius: 50%;
  border: var(--jp-border-width) solid var(--jp-inverse-layout-color3);
  background-color: var(--jp-inverse-layout-color3);
}

.jp-tocItem-content[data-running='0'],
.jp-tocItem-content[data-running='1'] {
  margin-right: 12px;
}

/*
 * Copyright (c) Jupyter Development Team.
 * Distributed under the terms of the Modified BSD License.
 */

.jp-Notebook-footer {
  height: 27px;
  margin-left: calc(
    var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
      var(--jp-cell-padding)
  );
  width: calc(
    100% -
      (
        var(--jp-cell-prompt-width) + var(--jp-cell-collapser-width) +
          var(--jp-cell-padding) + var(--jp-cell-padding)
      )
  );
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  color: var(--jp-ui-font-color3);
  margin-top: 6px;
  background: none;
  cursor: pointer;
}

.jp-Notebook-footer:focus {
  border-color: var(--jp-cell-editor-active-border-color);
}

/* For devices that support hovering, hide footer until hover */
@media (hover: hover) {
  .jp-Notebook-footer {
    opacity: 0;
  }

  .jp-Notebook-footer:focus,
  .jp-Notebook-footer:hover {
    opacity: 1;
  }
}

/*-----------------------------------------------------------------------------
| Copyright (c) Jupyter Development Team.
| Distributed under the terms of the Modified BSD License.
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| Imports
|----------------------------------------------------------------------------*/

/*-----------------------------------------------------------------------------
| CSS variables
|----------------------------------------------------------------------------*/

:root {
  --jp-side-by-side-output-size: 1fr;
  --jp-side-by-side-resized-cell: var(--jp-side-by-side-output-size);
  --jp-private-notebook-dragImage-width: 304px;
  --jp-private-notebook-dragImage-height: 36px;
  --jp-private-notebook-selected-color: var(--md-blue-400);
  --jp-private-notebook-active-color: var(--md-green-400);
}

/*-----------------------------------------------------------------------------
| Notebook
|----------------------------------------------------------------------------*/

/* stylelint-disable selector-max-class */

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

.jp-MainAreaWidget-ContainStrict .jp-Notebook * {
  contain: strict;
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

/* cell is dirty */
.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt {
  color: var(--jp-warn-color1);
}

.jp-Notebook .jp-Cell.jp-mod-dirty .jp-InputPrompt::before {
  color: var(--jp-warn-color1);
  content: '•';
}

.jp-Notebook .jp-Cell.jp-mod-active.jp-mod-dirty .jp-Collapser {
  background: var(--jp-warn-color1);
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
  display: block;
  flex-direction: row;
  width: var(--jp-private-notebook-dragImage-width);
  height: var(--jp-private-notebook-dragImage-height);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  background: var(--jp-cell-editor-background);
  overflow: visible;
}

.jp-dragImage-singlePrompt {
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
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
  margin: 4px 4px 4px 0;
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
  box-shadow: 2px 2px 4px 0 rgba(0, 0, 0, 0.12);
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

.jp-ActiveCellTool {
  padding: 12px 0;
  display: flex;
}

.jp-ActiveCellTool-Content {
  flex: 1 1 auto;
}

.jp-ActiveCellTool .jp-ActiveCellTool-CellContent {
  background: var(--jp-cell-editor-background);
  border: var(--jp-border-width) solid var(--jp-cell-editor-border-color);
  border-radius: 0;
  min-height: 29px;
}

.jp-ActiveCellTool .jp-InputPrompt {
  min-width: calc(var(--jp-cell-prompt-width) * 0.75);
}

.jp-ActiveCellTool-CellContent > pre {
  padding: 5px 4px;
  margin: 0;
  white-space: normal;
}

.jp-MetadataEditorTool {
  flex-direction: column;
  padding: 12px 0;
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
.jp-MetadataEditorTool label,
.jp-NumberSetter label {
  line-height: 1.4;
}

.jp-NotebookTools .jp-select-wrapper {
  margin-top: 4px;
  margin-bottom: 0;
}

.jp-NumberSetter input {
  width: 100%;
  margin-top: 4px;
}

.jp-NotebookTools .jp-Collapse {
  margin-top: 16px;
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
| Side-by-side Mode (.jp-mod-sideBySide)
|----------------------------------------------------------------------------*/
.jp-mod-sideBySide.jp-Notebook .jp-Notebook-cell {
  margin-top: 3em;
  margin-bottom: 3em;
  margin-left: 5%;
  margin-right: 5%;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell {
  display: grid;
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-output-size)
    );
  grid-template-rows: auto minmax(0, 1fr) auto;
  grid-template-areas:
    'header header header'
    'input handle output'
    'footer footer footer';
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell.jp-mod-resizedCell {
  grid-template-columns: minmax(0, 1fr) min-content minmax(
      0,
      var(--jp-side-by-side-resized-cell)
    );
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellHeader {
  grid-area: header;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-inputWrapper {
  grid-area: input;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-Cell-outputWrapper {
  /* overwrite the default margin (no vertical separation needed in side by side move */
  margin-top: 0;
  grid-area: output;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellFooter {
  grid-area: footer;
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle {
  grid-area: handle;
  user-select: none;
  display: block;
  height: 100%;
  cursor: ew-resize;
  padding: 0 var(--jp-cell-padding);
}

.jp-mod-sideBySide.jp-Notebook .jp-CodeCell .jp-CellResizeHandle::after {
  content: '';
  display: block;
  background: var(--jp-border-color2);
  height: 100%;
  width: 5px;
}

.jp-mod-sideBySide.jp-Notebook
  .jp-CodeCell.jp-mod-resizedCell
  .jp-CellResizeHandle::after {
  background: var(--jp-border-color0);
}

.jp-CellResizeHandle {
  display: none;
}

/*-----------------------------------------------------------------------------
| Placeholder
|----------------------------------------------------------------------------*/

.jp-Cell-Placeholder {
  padding-left: 55px;
}

.jp-Cell-Placeholder-wrapper {
  background: #fff;
  border: 1px solid;
  border-color: #e5e6e9 #dfe0e4 #d0d1d5;
  border-radius: 4px;
  -webkit-border-radius: 4px;
  margin: 10px 15px;
}

.jp-Cell-Placeholder-wrapper-inner {
  padding: 15px;
  position: relative;
}

.jp-Cell-Placeholder-wrapper-body {
  background-repeat: repeat;
  background-size: 50% auto;
}

.jp-Cell-Placeholder-wrapper-body div {
  background: #f6f7f8;
  background-image: -webkit-linear-gradient(
    left,
    #f6f7f8 0%,
    #edeef1 20%,
    #f6f7f8 40%,
    #f6f7f8 100%
  );
  background-repeat: no-repeat;
  background-size: 800px 104px;
  height: 104px;
  position: absolute;
  right: 15px;
  left: 15px;
  top: 15px;
}

div.jp-Cell-Placeholder-h1 {
  top: 20px;
  height: 20px;
  left: 15px;
  width: 150px;
}

div.jp-Cell-Placeholder-h2 {
  left: 15px;
  top: 50px;
  height: 10px;
  width: 100px;
}

div.jp-Cell-Placeholder-content-1,
div.jp-Cell-Placeholder-content-2,
div.jp-Cell-Placeholder-content-3 {
  left: 15px;
  right: 15px;
  height: 10px;
}

div.jp-Cell-Placeholder-content-1 {
  top: 100px;
}

div.jp-Cell-Placeholder-content-2 {
  top: 120px;
}

div.jp-Cell-Placeholder-content-3 {
  top: 140px;
}

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
  --jp-elevation-z1: 0 2px 1px -1px var(--jp-shadow-umbra-color),
    0 1px 1px 0 var(--jp-shadow-penumbra-color),
    0 1px 3px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z2: 0 3px 1px -2px var(--jp-shadow-umbra-color),
    0 2px 2px 0 var(--jp-shadow-penumbra-color),
    0 1px 5px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z4: 0 2px 4px -1px var(--jp-shadow-umbra-color),
    0 4px 5px 0 var(--jp-shadow-penumbra-color),
    0 1px 10px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z6: 0 3px 5px -1px var(--jp-shadow-umbra-color),
    0 6px 10px 0 var(--jp-shadow-penumbra-color),
    0 1px 18px 0 var(--jp-shadow-ambient-color);
  --jp-elevation-z8: 0 5px 5px -3px var(--jp-shadow-umbra-color),
    0 8px 10px 1px var(--jp-shadow-penumbra-color),
    0 3px 14px 2px var(--jp-shadow-ambient-color);
  --jp-elevation-z12: 0 7px 8px -4px var(--jp-shadow-umbra-color),
    0 12px 17px 2px var(--jp-shadow-penumbra-color),
    0 5px 22px 4px var(--jp-shadow-ambient-color);
  --jp-elevation-z16: 0 8px 10px -5px var(--jp-shadow-umbra-color),
    0 16px 24px 2px var(--jp-shadow-penumbra-color),
    0 6px 30px 5px var(--jp-shadow-ambient-color);
  --jp-elevation-z20: 0 10px 13px -6px var(--jp-shadow-umbra-color),
    0 20px 31px 3px var(--jp-shadow-penumbra-color),
    0 8px 38px 7px var(--jp-shadow-ambient-color);
  --jp-elevation-z24: 0 11px 15px -7px var(--jp-shadow-umbra-color),
    0 24px 38px 3px var(--jp-shadow-penumbra-color),
    0 9px 46px 8px var(--jp-shadow-ambient-color);

  /* Borders
   *
   * The following variables, specify the visual styling of borders in JupyterLab.
   */

  --jp-border-width: 1px;
  --jp-border-color0: var(--md-grey-400);
  --jp-border-color1: var(--md-grey-400);
  --jp-border-color2: var(--md-grey-300);
  --jp-border-color3: var(--md-grey-200);
  --jp-inverse-border-color: var(--md-grey-600);
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
  --jp-ui-font-family: system-ui, -apple-system, blinkmacsystemfont, 'Segoe UI',
    helvetica, arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji',
    'Segoe UI Symbol';

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
  --jp-content-link-color: var(--md-blue-900);
  --jp-content-font-family: system-ui, -apple-system, blinkmacsystemfont,
    'Segoe UI', helvetica, arial, sans-serif, 'Apple Color Emoji',
    'Segoe UI Emoji', 'Segoe UI Symbol';

  /*
   * Code Fonts
   *
   * Code font variables are used for typography of code and other monospaces content.
   */

  --jp-code-font-size: 13px;
  --jp-code-line-height: 1.3077; /* 17px for 13px base */
  --jp-code-padding: 5px; /* 5px for 13px base, codemirror highlighting needs integer px value */
  --jp-code-font-family-default: menlo, consolas, 'DejaVu Sans Mono', monospace;
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

  --jp-inverse-layout-color0: #111;
  --jp-inverse-layout-color1: var(--md-grey-900);
  --jp-inverse-layout-color2: var(--md-grey-800);
  --jp-inverse-layout-color3: var(--md-grey-700);
  --jp-inverse-layout-color4: var(--md-grey-600);

  /* Brand/accent */

  --jp-brand-color0: var(--md-blue-900);
  --jp-brand-color1: var(--md-blue-700);
  --jp-brand-color2: var(--md-blue-300);
  --jp-brand-color3: var(--md-blue-100);
  --jp-brand-color4: var(--md-blue-50);
  --jp-accent-color0: var(--md-green-900);
  --jp-accent-color1: var(--md-green-700);
  --jp-accent-color2: var(--md-green-300);
  --jp-accent-color3: var(--md-green-100);

  /* State colors (warn, error, success, info) */

  --jp-warn-color0: var(--md-orange-900);
  --jp-warn-color1: var(--md-orange-700);
  --jp-warn-color2: var(--md-orange-300);
  --jp-warn-color3: var(--md-orange-100);
  --jp-error-color0: var(--md-red-900);
  --jp-error-color1: var(--md-red-700);
  --jp-error-color2: var(--md-red-300);
  --jp-error-color3: var(--md-red-100);
  --jp-success-color0: var(--md-green-900);
  --jp-success-color1: var(--md-green-700);
  --jp-success-color2: var(--md-green-300);
  --jp-success-color3: var(--md-green-100);
  --jp-info-color0: var(--md-cyan-900);
  --jp-info-color1: var(--md-cyan-700);
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
  --jp-cell-prompt-font-family: var(--jp-code-font-family-default);
  --jp-cell-prompt-letter-spacing: 0;
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
  --jp-toolbar-box-shadow: 0 0 2px 0 rgba(0, 0, 0, 0.24);
  --jp-toolbar-header-margin: 4px 4px 0 4px;
  --jp-toolbar-active-background: var(--md-grey-300);

  /* Statusbar specific styles */

  --jp-statusbar-height: 24px;

  /* Input field styles */

  --jp-input-box-shadow: inset 0 0 2px var(--md-blue-300);
  --jp-input-active-background: var(--jp-layout-color1);
  --jp-input-hover-background: var(--jp-layout-color1);
  --jp-input-background: var(--md-grey-100);
  --jp-input-border-color: var(--jp-inverse-border-color);
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
  --jp-mirror-editor-variable-2-color: rgb(0, 54, 109);
  --jp-mirror-editor-variable-3-color: #085;
  --jp-mirror-editor-punctuation-color: #05a;
  --jp-mirror-editor-property-color: #05a;
  --jp-mirror-editor-operator-color: #a2f;
  --jp-mirror-editor-comment-color: #408080;
  --jp-mirror-editor-string-color: #ba2121;
  --jp-mirror-editor-string-2-color: #708;
  --jp-mirror-editor-meta-color: #a2f;
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

  /*
    RTC user specific colors.
    These colors are used for the cursor, username in the editor,
    and the icon of the user.
  */

  --jp-collaborator-color1: #ffad8e;
  --jp-collaborator-color2: #dac83d;
  --jp-collaborator-color3: #72dd76;
  --jp-collaborator-color4: #00e4d0;
  --jp-collaborator-color5: #45d4ff;
  --jp-collaborator-color6: #e2b1ff;
  --jp-collaborator-color7: #ff9de6;

  /* Vega extension styles */

  --jp-vega-background: white;

  /* Sidebar-related styles */

  --jp-sidebar-min-width: 250px;

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

  /* Button colors */
  --jp-accept-color-normal: var(--md-blue-700);
  --jp-accept-color-hover: var(--md-blue-800);
  --jp-accept-color-active: var(--md-blue-900);
  --jp-warn-color-normal: var(--md-red-700);
  --jp-warn-color-hover: var(--md-red-800);
  --jp-warn-color-active: var(--md-red-900);
  --jp-reject-color-normal: var(--md-grey-600);
  --jp-reject-color-hover: var(--md-grey-700);
  --jp-reject-color-active: var(--md-grey-800);

  /* File or activity icons and switch semantic variables */
  --jp-jupyter-icon-color: #f37626;
  --jp-notebook-icon-color: #f37626;
  --jp-json-icon-color: var(--md-orange-700);
  --jp-console-icon-background-color: var(--md-blue-700);
  --jp-console-icon-color: white;
  --jp-terminal-icon-background-color: var(--md-grey-800);
  --jp-terminal-icon-color: var(--md-grey-200);
  --jp-text-editor-icon-color: var(--md-grey-700);
  --jp-inspector-icon-color: var(--md-grey-700);
  --jp-switch-color: var(--md-grey-400);
  --jp-switch-true-position-color: var(--md-orange-900);
}
</style>
<style type="text/css">
/* Force rendering true colors when outputing to pdf */
* {
  -webkit-print-color-adjust: exact;
}

/* Misc */
a.anchor-link {
  display: none;
}

/* Input area styling */
.jp-InputArea {
  overflow: hidden;
}

.jp-InputArea-editor {
  overflow: hidden;
}

.cm-editor.cm-s-jupyter .highlight pre {
/* weird, but --jp-code-padding defined to be 5px but 4px horizontal padding is hardcoded for pre.cm-line */
  padding: var(--jp-code-padding) 4px;
  margin: 0;

  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  color: inherit;

}

.jp-OutputArea-output pre {
  line-height: inherit;
  font-family: inherit;
}

.jp-RenderedText pre {
  color: var(--jp-content-font-color1);
  font-size: var(--jp-code-font-size);
}

/* Hiding the collapser by default */
.jp-Collapser {
  display: none;
}

@page {
    margin: 0.5in; /* Margin for each printed piece of paper */
}

@media print {
  .jp-Cell-inputWrapper,
  .jp-Cell-outputWrapper {
    display: block;
  }
}
</style>
<!-- Load mathjax -->
<script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/latest.js?config=TeX-AMS_CHTML-full,Safe"> </script>
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
                }
            });

            MathJax.Hub.Queue(["Typeset", MathJax.Hub]);
        }
    }
    init_mathjax();
    </script>
<!-- End of mathjax configuration --><script type="module">
  document.addEventListener("DOMContentLoaded", async () => {
    const diagrams = document.querySelectorAll(".jp-Mermaid > pre.mermaid");
    // do not load mermaidjs if not needed
    if (!diagrams.length) {
      return;
    }
    const mermaid = (await import("https://cdnjs.cloudflare.com/ajax/libs/mermaid/10.6.0/mermaid.esm.min.mjs")).default;
    const parser = new DOMParser();

    mermaid.initialize({
      maxTextSize: 100000,
      startOnLoad: false,
      fontFamily: window
        .getComputedStyle(document.body)
        .getPropertyValue("--jp-ui-font-family"),
      theme: document.querySelector("body[data-jp-theme-light='true']")
        ? "default"
        : "dark",
    });

    let _nextMermaidId = 0;

    function makeMermaidImage(svg) {
      const img = document.createElement("img");
      const doc = parser.parseFromString(svg, "image/svg+xml");
      const svgEl = doc.querySelector("svg");
      const { maxWidth } = svgEl?.style || {};
      const firstTitle = doc.querySelector("title");
      const firstDesc = doc.querySelector("desc");

      img.setAttribute("src", `data:image/svg+xml,${encodeURIComponent(svg)}`);
      if (maxWidth) {
        img.width = parseInt(maxWidth);
      }
      if (firstTitle) {
        img.setAttribute("alt", firstTitle.textContent);
      }
      if (firstDesc) {
        const caption = document.createElement("figcaption");
        caption.className = "sr-only";
        caption.textContent = firstDesc.textContent;
        return [img, caption];
      }
      return [img];
    }

    async function makeMermaidError(text) {
      let errorMessage = "";
      try {
        await mermaid.parse(text);
      } catch (err) {
        errorMessage = `${err}`;
      }

      const result = document.createElement("details");
      result.className = 'jp-RenderedMermaid-Details';
      const summary = document.createElement("summary");
      summary.className = 'jp-RenderedMermaid-Summary';
      const pre = document.createElement("pre");
      const code = document.createElement("code");
      code.innerText = text;
      pre.appendChild(code);
      summary.appendChild(pre);
      result.appendChild(summary);

      const warning = document.createElement("pre");
      warning.innerText = errorMessage;
      result.appendChild(warning);
      return [result];
    }

    async function renderOneMarmaid(src) {
      const id = `jp-mermaid-${_nextMermaidId++}`;
      const parent = src.parentNode;
      let raw = src.textContent.trim();
      const el = document.createElement("div");
      el.style.visibility = "hidden";
      document.body.appendChild(el);
      let results = null;
      let output = null;
      try {
        const { svg } = await mermaid.render(id, raw, el);
        results = makeMermaidImage(svg);
        output = document.createElement("figure");
        results.map(output.appendChild, output);
      } catch (err) {
        parent.classList.add("jp-mod-warning");
        results = await makeMermaidError(raw);
        output = results[0];
      } finally {
        el.remove();
      }
      parent.classList.add("jp-RenderedMermaid");
      parent.appendChild(output);
    }

    void Promise.all([...diagrams].map(renderOneMarmaid));
  });
</script>
<style>
  .jp-Mermaid:not(.jp-RenderedMermaid) {
    display: none;
  }

  .jp-RenderedMermaid {
    overflow: auto;
    display: flex;
  }

  .jp-RenderedMermaid.jp-mod-warning {
    width: auto;
    padding: 0.5em;
    margin-top: 0.5em;
    border: var(--jp-border-width) solid var(--jp-warn-color2);
    border-radius: var(--jp-border-radius);
    color: var(--jp-ui-font-color1);
    font-size: var(--jp-ui-font-size1);
    white-space: pre-wrap;
    word-wrap: break-word;
  }

  .jp-RenderedMermaid figure {
    margin: 0;
    overflow: auto;
    max-width: 100%;
  }

  .jp-RenderedMermaid img {
    max-width: 100%;
  }

  .jp-RenderedMermaid-Details > pre {
    margin-top: 1em;
  }

  .jp-RenderedMermaid-Summary {
    color: var(--jp-warn-color2);
  }

  .jp-RenderedMermaid:not(.jp-mod-warning) pre {
    display: none;
  }

  .jp-RenderedMermaid-Summary > pre {
    display: inline-block;
    white-space: normal;
  }
</style>
<!-- End of mermaid configuration --></head>
<body class="jp-Notebook" data-jp-theme-light="true" data-jp-theme-name="JupyterLab Light">
<main>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h1 id="-%D0%9F%D1%80%D0%B5%D0%B4%D1%81%D0%BA%D0%B0%D0%B7%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D0%BE%D0%BB%D0%B0-%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%D0%B0-"><center> Предсказание пола клиента </center><a class="anchor-link" href="#-%D0%9F%D1%80%D0%B5%D0%B4%D1%81%D0%BA%D0%B0%D0%B7%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D0%BE%D0%BB%D0%B0-%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%D0%B0-">¶</a></h1><h3 id="%D0%9D%D0%B5%D0%BE%D0%B1%D1%85%D0%BE%D0%B4%D0%B8%D0%BC%D0%BE-%D0%B2%D1%8B%D1%8F%D0%B2%D0%B8%D1%82%D1%8C-%D0%BF%D0%BE%D0%BB-%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%D0%B0,-%D0%BE%D1%81%D0%BD%D0%BE%D0%B2%D1%8B%D0%B2%D0%B0%D1%8F%D1%81%D1%8C-%D0%BD%D0%B0-%D0%B5%D0%B3%D0%BE-%D1%82%D1%80%D0%B0%D0%BD%D0%B7%D0%B0%D0%BA%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D1%8B%D1%85-%D0%B8%D1%81%D1%82%D0%BE%D1%80%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D1%85-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85.-%D0%92-%D1%80%D0%BE%D0%BB%D0%B8-%D0%BC%D0%B5%D1%82%D1%80%D0%B8%D0%BA%D0%B8-%D0%BA%D0%B0%D1%87%D0%B5%D1%81%D1%82%D0%B2%D0%B0-%D0%B2%D1%8B%D1%81%D1%82%D1%83%D0%BF%D0%B0%D0%B5%D1%82-ROC-AUC,-%D0%BA%D0%BE%D1%82%D0%BE%D1%80%D1%8B%D0%B9-%D0%B8-%D0%BD%D1%83%D0%B6%D0%BD%D0%BE-%D0%B1%D1%83%D0%B4%D0%B5%D1%82-%D0%BC%D0%B0%D0%BA%D1%81%D0%B8%D0%BC%D0%B8%D0%B7%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D1%82%D1%8C.">Необходимо выявить пол клиента, основываясь на его транзакционных исторических данных. В роли метрики качества выступает <a href="https://dyakonov.org/2017/07/28/auc-roc-%D0%BF%D0%BB%D0%BE%D1%89%D0%B0%D0%B4%D1%8C-%D0%BF%D0%BE%D0%B4-%D0%BA%D1%80%D0%B8%D0%B2%D0%BE%D0%B9-%D0%BE%D1%88%D0%B8%D0%B1%D0%BE%D0%BA/">ROC AUC</a>, который и нужно будет максимизировать.<a class="anchor-link" href="#%D0%9D%D0%B5%D0%BE%D0%B1%D1%85%D0%BE%D0%B4%D0%B8%D0%BC%D0%BE-%D0%B2%D1%8B%D1%8F%D0%B2%D0%B8%D1%82%D1%8C-%D0%BF%D0%BE%D0%BB-%D0%BA%D0%BB%D0%B8%D0%B5%D0%BD%D1%82%D0%B0,-%D0%BE%D1%81%D0%BD%D0%BE%D0%B2%D1%8B%D0%B2%D0%B0%D1%8F%D1%81%D1%8C-%D0%BD%D0%B0-%D0%B5%D0%B3%D0%BE-%D1%82%D1%80%D0%B0%D0%BD%D0%B7%D0%B0%D0%BA%D1%86%D0%B8%D0%BE%D0%BD%D0%BD%D1%8B%D1%85-%D0%B8%D1%81%D1%82%D0%BE%D1%80%D0%B8%D1%87%D0%B5%D1%81%D0%BA%D0%B8%D1%85-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85.-%D0%92-%D1%80%D0%BE%D0%BB%D0%B8-%D0%BC%D0%B5%D1%82%D1%80%D0%B8%D0%BA%D0%B8-%D0%BA%D0%B0%D1%87%D0%B5%D1%81%D1%82%D0%B2%D0%B0-%D0%B2%D1%8B%D1%81%D1%82%D1%83%D0%BF%D0%B0%D0%B5%D1%82-ROC-AUC,-%D0%BA%D0%BE%D1%82%D0%BE%D1%80%D1%8B%D0%B9-%D0%B8-%D0%BD%D1%83%D0%B6%D0%BD%D0%BE-%D0%B1%D1%83%D0%B4%D0%B5%D1%82-%D0%BC%D0%B0%D0%BA%D1%81%D0%B8%D0%BC%D0%B8%D0%B7%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D1%82%D1%8C.">¶</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="%D0%9E%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2">Описание файлов<a class="anchor-link" href="#%D0%9E%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D1%84%D0%B0%D0%B9%D0%BB%D0%BE%D0%B2">¶</a></h2><ul>
<li>transactions.csv - исторические транзакции банковских клиентов</li>
<li>gender.csv - информация по полу для части клиентов (null - для тестовых)</li>
<li>tr_mcc_codes.csv - mcc-коды транзакций</li>
<li>tr_types.csv - типы транзакций</li>
</ul>
<h2 id="%D0%9E%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D0%BE%D0%BB%D0%B5%D0%B9">Описание полей<a class="anchor-link" href="#%D0%9E%D0%BF%D0%B8%D1%81%D0%B0%D0%BD%D0%B8%D0%B5-%D0%BF%D0%BE%D0%BB%D0%B5%D0%B9">¶</a></h2><h3 id="transactions.csv">transactions.csv<a class="anchor-link" href="#transactions.csv">¶</a></h3><ul>
<li>customer_id - идентификатор клиента</li>
<li>tr_datetime - день и время совершения транзакции (дни нумеруются с начала данных)</li>
<li>mcc_code - mcc-код транзакции</li>
<li>tr_type - тип транзакции</li>
<li>amount - сумма транзакции в условных единицах; со знаком "+" — начисление средств клиенту, "-" — списание средств</li>
<li>term_id - идентификатор терминала</li>
</ul>
<h3 id="gender.csv">gender.csv<a class="anchor-link" href="#gender.csv">¶</a></h3><ul>
<li>customer_id - идентификатор клиента</li>
<li>gender - пол клиента (пустые значения - тестовые клиенты)</li>
</ul>
<h3 id="tr_mcc_codes.csv">tr_mcc_codes.csv<a class="anchor-link" href="#tr_mcc_codes.csv">¶</a></h3><ul>
<li>mcc_code - mcc-код транзакции</li>
<li>mcc_description - описание mcc-кода транзакции</li>
</ul>
<h3 id="tr_types.csv">tr_types.csv<a class="anchor-link" href="#tr_types.csv">¶</a></h3><ul>
<li>tr_type - тип транзакции</li>
<li>tr_description - описание типа транзакции</li>
</ul>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h2 id="%D0%97%D0%B0%D0%B4%D0%B0%D1%87%D0%B8:">Задачи:<a class="anchor-link" href="#%D0%97%D0%B0%D0%B4%D0%B0%D1%87%D0%B8:">¶</a></h2><ul>
<li>Разработать модель бинарной классификации для определения пола клиента. Никаких ограничений к модели - может быть что угодно от KNN до трансформеров. Главное, чтобы ROC AUC на отложенном тесте получился выше 77.5%.</li>
<li>Интерпретировать результаты модели: важность входящих в нее переменных, демонстрация на нескольких примерах, почему получился соответствующий прогноз. Последнее позволит понять, какой пол к какому из таргетов (0/1) принадлежит. Опять же, полная свобода выбора подходов! Полезные ключевые слова: gain, permutation importance, SHAP.</li>
<li>Конвертировать результаты в отчет без кода (идеально - напрямую в <a href="https://stackoverflow.com/questions/49907455/hide-code-when-exporting-jupyter-notebook-to-html">html</a>)</li>
</ul>
<h4 id="P.S.-%D0%9D%D0%B5-%D0%B7%D0%B0%D0%B1%D1%8B%D0%B2%D0%B0%D0%B5%D0%BC-%D0%BF%D1%80%D0%BE-PEP8!">P.S. Не забываем про <a href="https://www.python.org/dev/peps/pep-0008/">PEP8</a>!<a class="anchor-link" href="#P.S.-%D0%9D%D0%B5-%D0%B7%D0%B0%D0%B1%D1%8B%D0%B2%D0%B0%D0%B5%D0%BC-%D0%BF%D1%80%D0%BE-PEP8!">¶</a></h4>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="1.-%D0%97%D0%BD%D0%B0%D0%BA%D0%BE%D0%BC%D1%81%D1%82%D0%B2%D0%BE-%D1%81-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D0%BC%D0%B8">1. Знакомство с данными<a class="anchor-link" href="#1.-%D0%97%D0%BD%D0%B0%D0%BA%D0%BE%D0%BC%D1%81%D1%82%D0%B2%D0%BE-%D1%81-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D0%BC%D0%B8">¶</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Подгружаем данные</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Исторические транзакции банковских клиентов</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
RangeIndex: 6849346 entries, 0 to 6849345
Data columns (total 6 columns):
 #   Column       Dtype  
---  ------       -----  
 0   customer_id  int64  
 1   tr_datetime  object 
 2   mcc_code     int64  
 3   tr_type      int64  
 4   amount       float64
 5   term_id      object 
dtypes: float64(1), int64(3), object(2)
memory usage: 313.5+ MB
None
   customer_id tr_datetime  mcc_code  tr_type    amount term_id
0     39026145  0 10:23:26      4814     1030  -2245.92     NaN
1     39026145  1 10:19:29      6011     7010  56147.89     NaN
2     39026145  1 10:20:56      4829     2330 -56147.89     NaN
3     39026145  1 10:39:54      5499     1010  -1392.47     NaN
4     39026145  2 15:33:42      5499     1010   -920.83     NaN
customer_id          0
tr_datetime          0
mcc_code             0
tr_type              0
amount               0
term_id        2765195
dtype: int64
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Типы транзакций</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
RangeIndex: 155 entries, 0 to 154
Data columns (total 2 columns):
 #   Column          Non-Null Count  Dtype 
---  ------          --------------  ----- 
 0   tr_type         155 non-null    int64 
 1   tr_description  155 non-null    object
dtypes: int64(1), object(1)
memory usage: 2.5+ KB
None
   tr_type                                     tr_description
0     3200  Плата за предоставление услуг посредством моби...
1     3210  Плата за предоставление отчета по счету карты ...
2     3800  Плата за обслуживание банковской карты (за пер...
3     4000            Плата за получение наличных в Сбербанке
4     4001  Плата за получение наличных в Сбербанке (в дру...
tr_type           0
tr_description    0
dtype: int64
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Mcc-коды транзакций</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
RangeIndex: 184 entries, 0 to 183
Data columns (total 2 columns):
 #   Column           Non-Null Count  Dtype 
---  ------           --------------  ----- 
 0   mcc_code         184 non-null    int64 
 1   mcc_description  184 non-null    object
dtypes: int64(1), object(1)
memory usage: 3.0+ KB
None
   mcc_code                                    mcc_description
0       742                                Ветеринарные услуги
1      1711  Генеральные подрядчики по вентиляции, теплосна...
2      1731                        Подрядчики по электричеству
3      1799  Подрядчики, специализированная торговля — нигд...
4      2741           Разнообразные издательства/печатное дело
mcc_code           0
mcc_description    0
dtype: int64
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Информация по полу для части клиентов (null - для тестовых)</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>&lt;class 'pandas.core.frame.DataFrame'&gt;
RangeIndex: 12000 entries, 0 to 11999
Data columns (total 2 columns):
 #   Column       Non-Null Count  Dtype  
---  ------       --------------  -----  
 0   customer_id  12000 non-null  int64  
 1   gender       8400 non-null   float64
dtypes: float64(1), int64(1)
memory usage: 187.6 KB
None
   customer_id  gender
0      6740969     1.0
1     36599781     0.0
2     91453656     1.0
3     17431962     1.0
4     72568668     1.0
customer_id       0
gender         3600
dtype: int64
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Посмотрим распределение таргета</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAkQAAAHHCAYAAABeLEexAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjguMiwgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy8g+/7EAAAACXBIWXMAAA9hAAAPYQGoP6dpAAAzOElEQVR4nO3deVyU9f7//+ewoziYGqCGiZoLpplYSpZmomRYmZrZ8YTHtLLQk3rSDp9ybbHy5FJStpyk9ZiWLS65YWonSYskl9TM8Gga4BKMkoDC9f2jH9fPEdwIGOz9uN9uc7s57+t1va/XNTLy9FpmHJZlWQIAADCYl6cbAAAA8DQCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIqALJyclyOBz2IyAgQM2bN9eIESOUlZXl6fYAwHg+nm4AMMmUKVMUERGh/Px8/fe//9XLL7+spUuXauvWrapRo4an2wMAYxGIgCrUq1cvdejQQZI0bNgw1a1bV9OnT9cnn3yiu+++28PdAYC5OGUGeNBNN90kScrIyJAkHTlyRI888ojatGmjoKAgOZ1O9erVS999912pdfPz8zVp0iQ1b95cAQEBql+/vvr27avdu3dLkvbs2eN2mu70x4033mjPtWbNGjkcDr3//vv6v//7P4WFhalmzZq67bbbtG/fvlLb3rBhg26++WYFBwerRo0a6tq1q7788ssy9/HGG28sc/uTJk0qVfvOO+8oKipKgYGBqlOnjgYOHFjm9s+2b6cqLi7WzJkz1bp1awUEBCg0NFQPPPCAfv31V7e6xo0bq3fv3qW2M2LEiFJzltX7tGnTSr2mklRQUKCJEyeqWbNm8vf3V3h4uMaNG6eCgoIyX6sSZ3rNytrPuXPn6qabblJISIj8/f0VGRmpl19+udScJfu4YsUKtWvXTgEBAYqMjNTChQvd6k4/vXvq4+eff7brduzYof79+6tOnToKCAhQhw4d9Omnn57XPCWP5ORkSdLmzZv1t7/9TU2aNFFAQIDCwsJ077336vDhw2d9nYCKxBEiwINKwkvdunUlST/99JM+/vhj3XnnnYqIiFBWVpZeeeUVde3aVd9//70aNGggSSoqKlLv3r2VkpKigQMH6uGHH9bRo0e1cuVKbd26VU2bNrW3cffdd+uWW25x225iYmKZ/Tz11FNyOBx69NFHlZ2drZkzZyomJkbp6ekKDAyUJK1evVq9evVSVFSUJk6cKC8vL/uX8hdffKFrr7221LyXXXaZpk6dKkk6duyYHnzwwTK3PX78eA0YMEDDhg3TwYMH9eKLL6pLly7atGmTateuXWqd+++/XzfccIMkaeHChfroo4/clj/wwANKTk7WkCFD9Pe//10ZGRmaPXu2Nm3apC+//FK+vr5lvg4XIicnx963UxUXF+u2227Tf//7X91///1q1aqVtmzZohkzZuiHH37Qxx9/fMY5H3vsMQ0bNkySdOjQIY0ePdptX0/18ssvq3Xr1rrtttvk4+OjRYsW6aGHHlJxcbESEhLcanft2qW77rpLw4cP1+DBgzV37lzdeeedWrZsmXr06OFWW3J691R16tSRJG3btk2dO3dWw4YN9c9//lM1a9bU/Pnz1adPH3344Ye644471KVLF7399tv2uk899ZS9byWuu+46SdLKlSv1008/aciQIQoLC9O2bdv06quvatu2bfrqq69KhVKgUlgAKt3cuXMtSdaqVausgwcPWvv27bPmzZtn1a1b1woMDLR+/vlny7IsKz8/3yoqKnJbNyMjw/L397emTJlij73xxhuWJGv69OmltlVcXGyvJ8maNm1aqZrWrVtbXbt2tZ9//vnnliSrYcOGlsvlssfnz59vSbJmzZplz33FFVdYsbGx9nYsy7J+++03KyIiwurRo0epbV133XXWlVdeaT8/ePCgJcmaOHGiPbZnzx7L29vbeuqpp9zW3bJli+Xj41NqfNeuXZYk680337THJk6caJ36T9oXX3xhSbLeffddt3WXLVtWavzyyy+34uLiSvWekJBgnf7P5Om9jxs3zgoJCbGioqLcXtO3337b8vLysr744gu39efMmWNJsr788stS2ytLyd/j3Llzy1z+22+/lRqLjY21mjRp4jZ2+eWXW5KsDz/80B7Lzc216tevb1199dX2WMnP6tdff33Gnrp37261adPGys/Pt8eKi4ut6667zrriiivKXKdr165ur8+59uE///mPJclat27dGfsAKhKnzIAqFBMTo0svvVTh4eEaOHCggoKC9NFHH6lhw4aSJH9/f3l5/f62LCoq0uHDhxUUFKQWLVro22+/tef58MMPVa9ePY0cObLUNv7I/6bj4+NVq1Yt+3n//v1Vv359LV26VJKUnp6uXbt26S9/+YsOHz6sQ4cO6dChQ8rLy1P37t21bt06FRcXu82Zn5+vgICAs2534cKFKi4u1oABA+w5Dx06pLCwMF1xxRX6/PPP3eoLCwsl/f56ncmCBQsUHBysHj16uM0ZFRWloKCgUnOeOHHCre7QoUPKz88/a9/79+/Xiy++qPHjxysoKKjU9lu1aqWWLVu6zVlymvT07ZdXyZE7ScrNzdWhQ4fUtWtX/fTTT8rNzXWrbdCgge644w77udPpVHx8vDZt2qTMzMzz2t6RI0e0evVqDRgwQEePHrX36/Dhw4qNjdWuXbu0f//+cu9Dfn6+Dh06pE6dOkmS2889UJk4ZQZUoaSkJDVv3lw+Pj4KDQ1VixYt7AAk/X6aZdasWXrppZeUkZGhoqIie1nJaTXp91NtLVq0kI9Pxb6Fr7jiCrfnDodDzZo10549eyT9fspFkgYPHnzGOXJzc3XJJZfYzw8dOlRq3tPt2rVLlmWdse70U1s5OTmSVCqEnD5nbm6uQkJCylyenZ3t9nzFihW69NJLz9rn6SZOnKgGDRrogQce0AcffFBq+9u3bz/jnKdvv7y+/PJLTZw4Uampqfrtt9/cluXm5io4ONh+3qxZs1KBuXnz5pJ+vy4rLCzsnNv78ccfZVmWxo8fr/Hjx5dZk52dbYf883HkyBFNnjxZ8+bNK/W6nB7qgMpCIAKq0LXXXmvfZVaWp59+WuPHj9e9996rJ554QnXq1JGXl5dGjRpV6siLJ5T0MG3aNLVr167MmlNDSmFhoX755ZdS16eUNa/D4dBnn30mb2/vs84pyT6acbZf4MXFxQoJCdG7775b5vLTg0rHjh315JNPuo3Nnj1bn3zySZnrb9++XcnJyXrnnXfKvBapuLhYbdq00fTp08tcPzw8/Iy9n6/du3ere/fuatmypaZPn67w8HD5+flp6dKlmjFjRqX8zJTM+cgjjyg2NrbMmmbNml3QnAMGDND69es1duxYtWvXTkFBQSouLtbNN99cLX7uYQYCEVCNfPDBB+rWrZv+/e9/u43n5OSoXr169vOmTZtqw4YNOnHiRIVcGFyi5AhQCcuy9OOPP6pt27b2dqXfT7XExMScc77vvvtOJ06cOGsILJnXsixFRETYRyzO5vvvv5fD4VCLFi3OOueqVavUuXNnt1MyZ1KvXr1S+3S2C58TExPVrl073XXXXWfc/nfffafu3btX2kXBixYtUkFBgT799FM1atTIHj/T6biSozun9vPDDz9I+v0utPPRpEkTSb8ftTufn4Fz+fXXX5WSkqLJkydrwoQJ9vjpP4tAZeMaIqAa8fb2lmVZbmMLFiwodU1Gv379dOjQIc2ePbvUHKevfyHeeustHT161H7+wQcf6JdfflGvXr0kSVFRUWratKn+9a9/6dixY6XWP3jwYKnevb29y7yl/VR9+/aVt7e3Jk+eXKp/y7Lcbr8+efKkPvzwQ1177bVnPWU2YMAAFRUV6Yknnii17OTJk/Zpt/JITU3VJ598omeeeeaMYWfAgAHav3+/XnvttVLLjh8/rry8vHJvv0TJ0bRTX7Pc3FzNnTu3zPoDBw643Ynncrn01ltvqV27dud1ukySQkJCdOONN+qVV17RL7/8Umr56T8D51LWPkjSzJkzL2ge4I/iCBFQjfTu3VtTpkzRkCFDdN1112nLli1699137f+Vl4iPj9dbb72lMWPGaOPGjbrhhhuUl5enVatW6aGHHtLtt99eru3XqVNH119/vYYMGaKsrCzNnDlTzZo103333SdJ8vLy0uuvv65evXqpdevWGjJkiBo2bKj9+/fr888/l9Pp1KJFi5SXl6ekpCS98MILat68udasWWNvoyRIbd68WampqYqOjlbTpk315JNPKjExUXv27FGfPn1Uq1YtZWRk6KOPPtL999+vRx55RKtWrdL48eO1efNmLVq06Kz70rVrVz3wwAOaOnWq0tPT1bNnT/n6+mrXrl1asGCBZs2apf79+5frdVqxYoV69Ohx1iMk99xzj+bPn6/hw4fr888/V+fOnVVUVKQdO3Zo/vz5Wr58+TmPnJ1Lz5495efnp1tvvVUPPPCAjh07ptdee00hISFlhpXmzZtr6NCh+vrrrxUaGqo33nhDWVlZZwxQZ5KUlKTrr79ebdq00X333acmTZooKytLqamp+vnnn8v83KwzcTqd6tKli5577jmdOHFCDRs21IoVK+zP5gKqjIfubgOMcj63MlvW77fd/+Mf/7Dq169vBQYGWp07d7ZSU1PLvGX5t99+sx577DErIiLC8vX1tcLCwqz+/ftbu3fvtiyrfLfd/+c//7ESExOtkJAQKzAw0IqLi7P+97//lVp/06ZNVt++fa26deta/v7+1uWXX24NGDDASklJcdv2uR6DBw92m/fDDz+0rr/+eqtmzZpWzZo1rZYtW1oJCQnWzp07LcuyrJEjR1pdunSxli1bVqqn02+7L/Hqq69aUVFRVmBgoFWrVi2rTZs21rhx46wDBw7YNRd6273D4bDS0tLcxsv6OyosLLSeffZZq3Xr1pa/v791ySWXWFFRUdbkyZOt3NzcUtsry7luu//000+ttm3bWgEBAVbjxo2tZ5991v5YhoyMjFL7uHz5cqtt27aWv7+/1bJlS2vBggVu853vz+ru3but+Ph4KywszPL19bUaNmxo9e7d2/rggw/KrD/bbfc///yzdccdd1i1a9e2goODrTvvvNM6cOBAqY84ACqTw7L+wPF1AH8Ka9asUbdu3bRgwYJyHzU51Z49exQREaGMjIwzXpsyadIk7dmzx/60YlSuxo0b68orr9TixYs93QpQLXENEQAAMB7XEAGocEFBQRo0aNBZL3pu27at/VUkAOBpBCIAFa5evXp65513zlrTt2/fKuoGAM6Na4gAAIDxuIYIAAAYj0AEAACMxzVE56G4uFgHDhxQrVq1Ku0j+AEAQMWyLEtHjx5VgwYN3L5IuywEovNw4MCBCvkiRgAAUPX27dunyy677Kw1BKLzUKtWLUm/v6BOp9PD3QAAgPPhcrkUHh5u/x4/GwLReSg5TeZ0OglEAABcZM7nchcuqgYAAMYjEAEAAOMRiAAAgPEIRAAAwHgEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIAAAYz8fTDeD/FzX2LU+3AFRLadPiPd0CgD85jhABAADjEYgAAIDxCEQAAMB4BCIAAGA8AhEAADAegQgAABiPQAQAAIxHIAIAAMYjEAEAAOMRiAAAgPEIRAAAwHgEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIAAAYj0AEAACMRyACAADGIxABAADjEYgAAIDxCEQAAMB4BCIAAGA8AhEAADAegQgAABiPQAQAAIxHIAIAAMYjEAEAAOMRiAAAgPEIRAAAwHgEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgvGoTiJ555hk5HA6NGjXKHsvPz1dCQoLq1q2roKAg9evXT1lZWW7r7d27V3FxcapRo4ZCQkI0duxYnTx50q1mzZo1at++vfz9/dWsWTMlJydXwR4BAICLRbUIRF9//bVeeeUVtW3b1m189OjRWrRokRYsWKC1a9fqwIED6tu3r728qKhIcXFxKiws1Pr16/Xmm28qOTlZEyZMsGsyMjIUFxenbt26KT09XaNGjdKwYcO0fPnyKts/AABQvXk8EB07dkyDBg3Sa6+9pksuucQez83N1b///W9Nnz5dN910k6KiojR37lytX79eX331lSRpxYoV+v777/XOO++oXbt26tWrl5544gklJSWpsLBQkjRnzhxFRETo+eefV6tWrTRixAj1799fM2bM8Mj+AgCA6sfjgSghIUFxcXGKiYlxG09LS9OJEyfcxlu2bKlGjRopNTVVkpSamqo2bdooNDTUromNjZXL5dK2bdvsmtPnjo2NtecoS0FBgVwul9sDAAD8efl4cuPz5s3Tt99+q6+//rrUsszMTPn5+al27dpu46GhocrMzLRrTg1DJctLlp2txuVy6fjx4woMDCy17alTp2ry5Mnl3i8AAHBx8dgRon379unhhx/Wu+++q4CAAE+1UabExETl5ubaj3379nm6JQAAUIk8FojS0tKUnZ2t9u3by8fHRz4+Plq7dq1eeOEF+fj4KDQ0VIWFhcrJyXFbLysrS2FhYZKksLCwUnedlTw/V43T6Szz6JAk+fv7y+l0uj0AAMCfl8cCUffu3bVlyxalp6fbjw4dOmjQoEH2n319fZWSkmKvs3PnTu3du1fR0dGSpOjoaG3ZskXZ2dl2zcqVK+V0OhUZGWnXnDpHSU3JHAAAAB67hqhWrVq68sor3cZq1qypunXr2uNDhw7VmDFjVKdOHTmdTo0cOVLR0dHq1KmTJKlnz56KjIzUPffco+eee06ZmZl6/PHHlZCQIH9/f0nS8OHDNXv2bI0bN0733nuvVq9erfnz52vJkiVVu8MAAKDa8uhF1ecyY8YMeXl5qV+/fiooKFBsbKxeeukle7m3t7cWL16sBx98UNHR0apZs6YGDx6sKVOm2DURERFasmSJRo8erVmzZumyyy7T66+/rtjYWE/sEgAAqIYclmVZnm6iunO5XAoODlZubm6lXk8UNfatSpsbuJilTYv3dAsA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AABVoVyBaPPmzWrXrp0kaevWrW7LuMAaAABcbMoViD7//POK7gMAAMBjynUNEQAAwJ9JuY4QdevW7aynxlavXl3uhgAAAKpauQJRyfVDJU6cOKH09HRt3bq11Je+AgAAVHflCkQzZswoc3zSpEk6duzYH2oIAACgqlXoNUR//etf+R4zAABw0anQQJSamqqAgICKnBIAAKDSleuUWd++fd2eW5alX375Rd98843Gjx9fIY0BAABUlXIFouDgYLfnXl5eatGihaZMmaKePXtWSGMAAABVpVyBaO7cuRXdBwAAgMeUKxCVSEtL0/bt2yVJrVu31tVXX10hTQEAAFSlcgWi7OxsDRw4UGvWrFHt2rUlSTk5OerWrZvmzZunSy+9tCJ7BAAAqFTlusts5MiROnr0qLZt26YjR47oyJEj2rp1q1wul/7+979XdI8AAACVqlxHiJYtW6ZVq1apVatW9lhkZKSSkpK4qBoAAFx0ynWEqLi4WL6+vqXGfX19VVxc/IebAgAAqErlCkQ33XSTHn74YR04cMAe279/v0aPHq3u3btXWHMAAABVoVyBaPbs2XK5XGrcuLGaNm2qpk2bKiIiQi6XSy+++GJF9wgAAFCpynUNUXh4uL799lutWrVKO3bskCS1atVKMTExFdocAABAVbigI0SrV69WZGSkXC6XHA6HevTooZEjR2rkyJG65ppr1Lp1a33xxReV1SsAAECluKBANHPmTN13331yOp2llgUHB+uBBx7Q9OnTK6w5AACAqnBBgei7777TzTfffMblPXv2VFpa2h9uCgAAoCpdUCDKysoq83b7Ej4+Pjp48OAfbgoAAKAqXVAgatiwobZu3XrG5Zs3b1b9+vX/cFMAAABV6YIC0S233KLx48crPz+/1LLjx49r4sSJ6t27d4U1BwAAUBUu6Lb7xx9/XAsXLlTz5s01YsQItWjRQpK0Y8cOJSUlqaioSI899lilNAoAAFBZLigQhYaGav369XrwwQeVmJgoy7IkSQ6HQ7GxsUpKSlJoaGilNAoAAFBZLviDGS+//HItXbpUv/76q3788UdZlqUrrrhCl1xySWX0BwAAUOnK9UnVknTJJZfommuuqcheAAAAPKJc32UGAADwZ0IgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPI8GoqlTp+qaa65RrVq1FBISoj59+mjnzp1uNfn5+UpISFDdunUVFBSkfv36KSsry61m7969iouLU40aNRQSEqKxY8fq5MmTbjVr1qxR+/bt5e/vr2bNmik5Obmydw8AAFwkPBqI1q5dq4SEBH311VdauXKlTpw4oZ49eyovL8+uGT16tBYtWqQFCxZo7dq1OnDggPr27WsvLyoqUlxcnAoLC7V+/Xq9+eabSk5O1oQJE+yajIwMxcXFqVu3bkpPT9eoUaM0bNgwLV++vEr3FwAAVE8Oq+T7N6qBgwcPKiQkRGvXrlWXLl2Um5urSy+9VO+995769+8v6ffvTWvVqpVSU1PVqVMnffbZZ+rdu7cOHDhgf23InDlz9Oijj+rgwYPy8/PTo48+qiVLlmjr1q32tgYOHKicnBwtW7bsnH25XC4FBwcrNzdXTqezcnZeUtTYtyptbuBiljYt3tMt/GG8v4GyVeb7+0J+f1era4hyc3MlSXXq1JEkpaWl6cSJE4qJibFrWrZsqUaNGik1NVWSlJqaqjZt2rh9h1psbKxcLpe2bdtm15w6R0lNyRynKygokMvlcnsAAIA/r2oTiIqLizVq1Ch17txZV155pSQpMzNTfn5+ql27tlttaGioMjMz7ZrTv1C25Pm5alwul44fP16ql6lTpyo4ONh+hIeHV8g+AgCA6qnaBKKEhARt3bpV8+bN83QrSkxMVG5urv3Yt2+fp1sCAACVqNxf7lqRRowYocWLF2vdunW67LLL7PGwsDAVFhYqJyfH7ShRVlaWwsLC7JqNGze6zVdyF9qpNaffmZaVlSWn06nAwMBS/fj7+8vf379C9g0AAFR/Hj1CZFmWRowYoY8++kirV69WRESE2/KoqCj5+voqJSXFHtu5c6f27t2r6OhoSVJ0dLS2bNmi7Oxsu2blypVyOp2KjIy0a06do6SmZA4AAGA2jx4hSkhI0HvvvadPPvlEtWrVsq/5CQ4OVmBgoIKDgzV06FCNGTNGderUkdPp1MiRIxUdHa1OnTpJknr27KnIyEjdc889eu6555SZmanHH39cCQkJ9lGe4cOHa/bs2Ro3bpzuvfderV69WvPnz9eSJUs8tu8AAKD68OgRopdfflm5ubm68cYbVb9+ffvx/vvv2zUzZsxQ79691a9fP3Xp0kVhYWFauHChvdzb21uLFy+Wt7e3oqOj9de//lXx8fGaMmWKXRMREaElS5Zo5cqVuuqqq/T888/r9ddfV2xsbJXuLwAAqJ48eoTofD4CKSAgQElJSUpKSjpjzeWXX66lS5eedZ4bb7xRmzZtuuAeAQDAn1+1ucsMAADAUwhEAADAeAQiAABgPAIRAAAwHoEIAAAYj0AEAACMRyACAADGIxABAADjEYgAAIDxCEQAAMB4BCIAAGA8AhEAADAegQgAABiPQAQAAIxHIAIAAMYjEAEAAOMRiAAAgPEIRAAAwHgEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIAAAYj0AEAACMRyACAADGIxABAADjEYgAAIDxCEQAAMB4BCIAAGA8AhEAADAegQgAABiPQAQAAIxHIAIAAMYjEAEAAOMRiAAAgPEIRAAAwHgEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIAAAYj0AEAACMRyACAADGIxABAADjEYgAAIDxCEQAAMB4BCIAAGA8AhEAADAegQgAABiPQAQAAIxHIAIAAMYjEAEAAOMRiAAAgPE8GojWrVunW2+9VQ0aNJDD4dDHH3/sttyyLE2YMEH169dXYGCgYmJitGvXLreaI0eOaNCgQXI6napdu7aGDh2qY8eOudVs3rxZN9xwgwICAhQeHq7nnnuusncNAABcRDwaiPLy8nTVVVcpKSmpzOXPPfecXnjhBc2ZM0cbNmxQzZo1FRsbq/z8fLtm0KBB2rZtm1auXKnFixdr3bp1uv/+++3lLpdLPXv21OWXX660tDRNmzZNkyZN0quvvlrp+wcAAC4OPp7ceK9evdSrV68yl1mWpZkzZ+rxxx/X7bffLkl66623FBoaqo8//lgDBw7U9u3btWzZMn399dfq0KGDJOnFF1/ULbfcon/9619q0KCB3n33XRUWFuqNN96Qn5+fWrdurfT0dE2fPt0tOAEAAHNV22uIMjIylJmZqZiYGHssODhYHTt2VGpqqiQpNTVVtWvXtsOQJMXExMjLy0sbNmywa7p06SI/Pz+7JjY2Vjt37tSvv/5a5rYLCgrkcrncHgAA4M+r2gaizMxMSVJoaKjbeGhoqL0sMzNTISEhbst9fHxUp04dt5qy5jh1G6ebOnWqgoOD7Ud4ePgf3yEAAFBtVdtA5EmJiYnKzc21H/v27fN0SwAAoBJV20AUFhYmScrKynIbz8rKspeFhYUpOzvbbfnJkyd15MgRt5qy5jh1G6fz9/eX0+l0ewAAgD+vahuIIiIiFBYWppSUFHvM5XJpw4YNio6OliRFR0crJydHaWlpds3q1atVXFysjh072jXr1q3TiRMn7JqVK1eqRYsWuuSSS6pobwAAQHXm0UB07NgxpaenKz09XdLvF1Knp6dr7969cjgcGjVqlJ588kl9+umn2rJli+Lj49WgQQP16dNHktSqVSvdfPPNuu+++7Rx40Z9+eWXGjFihAYOHKgGDRpIkv7yl7/Iz89PQ4cO1bZt2/T+++9r1qxZGjNmjIf2GgAAVDceve3+m2++Ubdu3eznJSFl8ODBSk5O1rhx45SXl6f7779fOTk5uv7667Vs2TIFBATY67z77rsaMWKEunfvLi8vL/Xr108vvPCCvTw4OFgrVqxQQkKCoqKiVK9ePU2YMIFb7gEAgM1hWZbl6SaqO5fLpeDgYOXm5lbq9URRY9+qtLmBi1natHhPt/CH8f4GylaZ7+8L+f1dba8hAgAAqCoEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIAAAYj0AEAACMRyACAADGIxABAADjEYgAAIDxCEQAAMB4BCIAAGA8AhEAADAegQgAABiPQAQAAIxHIAIAAMYjEAEAAOMRiAAAgPEIRAAAwHgEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIAAAYj0AEAACMRyACAADGIxABAADjEYgAAIDxCEQAAMB4BCIAAGA8AhEAADAegQgAABiPQAQAAIxHIAIAAMYjEAEAAOMRiAAAgPEIRAAAwHgEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIAAAYj0AEAACMRyACAADGIxABAADjEYgAAIDxjApESUlJaty4sQICAtSxY0dt3LjR0y0BAIBqwJhA9P7772vMmDGaOHGivv32W1111VWKjY1Vdna2p1sDAAAeZkwgmj59uu677z4NGTJEkZGRmjNnjmrUqKE33njD060BAAAPMyIQFRYWKi0tTTExMfaYl5eXYmJilJqa6sHOAABAdeDj6QaqwqFDh1RUVKTQ0FC38dDQUO3YsaNUfUFBgQoKCuznubm5kiSXy1WpfRYVHK/U+YGLVWW/96oC72+gbJX5/i6Z27Ksc9YaEYgu1NSpUzV58uRS4+Hh4R7oBkDwi8M93QKASlIV7++jR48qODj4rDVGBKJ69erJ29tbWVlZbuNZWVkKCwsrVZ+YmKgxY8bYz4uLi3XkyBHVrVtXDoej0vuFZ7lcLoWHh2vfvn1yOp2ebgdABeL9bRbLsnT06FE1aNDgnLVGBCI/Pz9FRUUpJSVFffr0kfR7yElJSdGIESNK1fv7+8vf399trHbt2lXQKaoTp9PJP5jAnxTvb3Oc68hQCSMCkSSNGTNGgwcPVocOHXTttddq5syZysvL05AhQzzdGgAA8DBjAtFdd92lgwcPasKECcrMzFS7du20bNmyUhdaAwAA8xgTiCRpxIgRZZ4iA07l7++viRMnljptCuDix/sbZ+KwzudeNAAAgD8xIz6YEQAA4GwIRAAAwHgEIgAAYDwCEQAAMB6BCEZKSkpS48aNFRAQoI4dO2rjxo1nrV+wYIFatmypgIAAtWnTRkuXLq2iTgFciHXr1unWW29VgwYN5HA49PHHH59znTVr1qh9+/by9/dXs2bNlJycXOl9ovohEME477//vsaMGaOJEyfq22+/1VVXXaXY2FhlZ2eXWb9+/XrdfffdGjp0qDZt2qQ+ffqoT58+2rp1axV3DuBc8vLydNVVVykpKem86jMyMhQXF6du3bopPT1do0aN0rBhw7R8+fJK7hTVDbfdwzgdO3bUNddco9mzZ0v6/WtcwsPDNXLkSP3zn/8sVX/XXXcpLy9Pixcvtsc6deqkdu3aac6cOVXWN4AL43A49NFHH9lf2VSWRx99VEuWLHH7D87AgQOVk5OjZcuWVUGXqC44QgSjFBYWKi0tTTExMfaYl5eXYmJilJqaWuY6qampbvWSFBsbe8Z6ABcP3t8oQSCCUQ4dOqSioqJSX9kSGhqqzMzMMtfJzMy8oHoAF48zvb9dLpeOHz/uoa7gCQQiAABgPAIRjFKvXj15e3srKyvLbTwrK0thYWFlrhMWFnZB9QAuHmd6fzudTgUGBnqoK3gCgQhG8fPzU1RUlFJSUuyx4uJipaSkKDo6usx1oqOj3eolaeXKlWesB3Dx4P2NEgQiGGfMmDF67bXX9Oabb2r79u168MEHlZeXpyFDhkiS4uPjlZiYaNc//PDDWrZsmZ5//nnt2LFDkyZN0jfffKMRI0Z4ahcAnMGxY8eUnp6u9PR0Sb/fVp+enq69e/dKkhITExUfH2/XDx8+XD/99JPGjRunHTt26KWXXtL8+fM1evRoT7QPT7IAA7344otWo0aNLD8/P+vaa6+1vvrqK3tZ165drcGDB7vVz58/32revLnl5+dntW7d2lqyZEkVdwzgfHz++eeWpFKPkvf04MGDra5du5Zap127dpafn5/VpEkTa+7cuVXeNzyPzyECAADG45QZAAAwHoEIAAAYj0AEAACMRyACAADGIxABAADjEYgAAIDxCEQAAMB4BCIAOA833nijRo0a5ek2AFQSAhGAi0ZmZqYefvhhNWvWTAEBAQoNDVXnzp318ssv67fffvN0ewAuYj6ebgAAzsdPP/2kzp07q3bt2nr66afVpk0b+fv7a8uWLXr11VfVsGFD3XbbbZ5u84yKiorkcDjk5cX/Q4HqiHcmgIvCQw89JB8fH33zzTcaMGCAWrVqpSZNmuj222/XkiVLdOutt0qScnJyNGzYMF166aVyOp266aab9N1339nzTJo0Se3atdPbb7+txo0bKzg4WAMHDtTRo0ftmry8PMXHxysoKEj169fX888/X6qfgoICPfLII2rYsKFq1qypjh07as2aNfby5ORk1a5dW59++qkiIyPl7+9vf8EogOqHQASg2jt8+LBWrFihhIQE1axZs8wah8MhSbrzzjuVnZ2tzz77TGlpaWrfvr26d++uI0eO2LW7d+/Wxx9/rMWLF2vx4sVau3atnnnmGXv52LFjtXbtWn3yySdasWKF1qxZo2+//dZteyNGjFBqaqrmzZunzZs3684779TNN9+sXbt22TW//fabnn32Wb3++uvatm2bQkJCKvJlAVCRPP3tsgBwLl999ZUlyVq4cKHbeN26da2aNWtaNWvWtMaNG2d98cUXltPptPLz893qmjZtar3yyiuWZVnWxIkTrRo1algul8tePnbsWKtjx46WZVnW0aNHLT8/P2v+/Pn28sOHD1uBgYHWww8/bFmWZf3vf/+zvL29rf3797ttp3v37lZiYqJlWZY1d+5cS5KVnp5eMS8CgErFNUQALlobN25UcXGxBg0apIKCAn333Xc6duyY6tat61Z3/Phx7d69237euHFj1apVy35ev359ZWdnS/r96FFhYaE6duxoL69Tp45atGhhP9+yZYuKiorUvHlzt+0UFBS4bdvPz09t27atmJ0FUKkIRACqvWbNmsnhcGjnzp1u402aNJEkBQYGSpKOHTum+vXru13LU6J27dr2n319fd2WORwOFRcXn3c/x44dk7e3t9LS0uTt7e22LCgoyP5zYGCgfSoPQPVGIAJQ7dWtW1c9evTQ7NmzNXLkyDNeR9S+fXtlZmbKx8dHjRs3Lte2mjZtKl9fX23YsEGNGjWSJP3666/64Ycf1LVrV0nS1VdfraKiImVnZ+uGG24o13YAVC9cVA3govDSSy/p5MmT6tChg95//31t375dO3fu1DvvvKMdO3bI29tbMTExio6OVp8+fbRixQrt2bNH69ev12OPPaZvvvnmvLYTFBSkoUOHauzYsVq9erW2bt2qv/3tb263yzdv3lyDBg1SfHy8Fi5cqIyMDG3cuFFTp07VkiVLKuslAFCJOEIE4KLQtGlTbdq0SU8//bQSExP1888/y9/fX5GRkXrkkUf00EMPyeFwaOnSpXrsscc0ZMgQHTx4UGFhYerSpYtCQ0PPe1vTpk3TsWPHdOutt6pWrVr6xz/+odzcXLeauXPn6sknn9Q//vEP7d+/X/Xq1VOnTp3Uu3fvit51AFXAYVmW5ekmAAAAPIlTZgAAwHgEIgAAYDwCEQAAMB6BCAAAGI9ABAAAjEcgAgAAxiMQAQAA4xGIAACA8QhEAADAeAQiAABgPAIRAAAwHoEIAAAY7/8BeyHvyHrCaTUAAAAASUVORK5CYII="/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Выводы:<br/>
Таргет не имеет классового дизбаланса.<br/>
Во всех данных, исключая исторические транзакции банковских клиентов отсутствуют пропуски. В данных по транзакциям пропущено 2 765 195 значений в колонке term_id, а это 40% от общего объема данных. Принято решение удалить фичу term_id.</p>
<p>В исторической транзакции банковских клиентов 6 849 346 строк.<br/>
Как вариант можно снизить размерность таблицы, сгруппировав данные по customer_id. В таком случае обучение пройдет быстрее, но потеряются часть данных, в частности характеристика времени.<br/>
Также можно привязать таргет (gender) по customer_id и провести анализ по корреляции данных. Для проверки корреляции между временем в формате timestamp и таргетом можно использовать коэффициент корреляции Пирсона или Спирмена.</p>
<p>Принято решение выбрать вариант снижения размерности таблицы, просуммировав количество кажого типа и mcc кода транзакции для каждого customer_id. Если точность такого варианта не удовлетворит ТЗ, вернуться к варианту с созранением временного ряда.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="2.-%D0%9F%D1%80%D0%B5%D0%B4%D0%BE%D0%B1%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B0">2. Предобработка<a class="anchor-link" href="#2.-%D0%9F%D1%80%D0%B5%D0%B4%D0%BE%D0%B1%D1%80%D0%B0%D0%B1%D0%BE%D1%82%D0%BA%D0%B0">¶</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Группируем данные по customer_id, просуммировав количество кажого типа и mcc кода транзакции</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Переименование колонок в mcc_features в mcc_description</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Объединим все полученые переменные</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Добавим таргет к данным</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Посмотрим на результат</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>customer_id</th>
<th>Ветеринарные услуги</th>
<th>Генеральные подрядчики по вентиляции, теплоснабжению, и водопроводу</th>
<th>Подрядчики по электричеству</th>
<th>Подрядчики, специализированная торговля — нигде более не классифицированные</th>
<th>Разнообразные издательства/печатное дело</th>
<th>Авиалинии, авиакомпании</th>
<th>Агентства по аренде автомобилей</th>
<th>Жилье — отели, мотели, курорты</th>
<th>Транспортировка — пригородные и локальные сезонные транспортные средства, включая электрички</th>
<th>...</th>
<th>tr_type_7070</th>
<th>tr_type_7071</th>
<th>tr_type_7074</th>
<th>tr_type_7075</th>
<th>tr_type_8100</th>
<th>tr_type_8145</th>
<th>tr_type_8146</th>
<th>add_cash</th>
<th>withdraw_cash</th>
<th>gender</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>6815</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>2706553.10</td>
<td>-3956007.97</td>
<td>NaN</td>
</tr>
<tr>
<th>1</th>
<td>22899</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>9</td>
<td>3</td>
<td>0</td>
<td>1</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>5818923.05</td>
<td>-6448719.64</td>
<td>1.0</td>
</tr>
<tr>
<th>2</th>
<td>27914</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>409879.70</td>
<td>-3386906.52</td>
<td>1.0</td>
</tr>
<tr>
<th>3</th>
<td>28753</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>14</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>45707408.97</td>
<td>-72253691.83</td>
<td>0.0</td>
</tr>
<tr>
<th>4</th>
<td>31385</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>1</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>1251334.45</td>
<td>-3431338.03</td>
<td>0.0</td>
</tr>
</tbody>
</table>
<p>5 rows × 265 columns</p>
</div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Количество фичей</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>265</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="3.-%D0%A1%D1%82%D0%B0%D1%82%D0%B8%D1%81%D1%82%D0%B8%D0%BA%D0%B0">3. Статистика<a class="anchor-link" href="#3.-%D0%A1%D1%82%D0%B0%D1%82%D0%B8%D1%81%D1%82%D0%B8%D0%BA%D0%B0">¶</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Исходя из того, что все данные числовые, можно провести t-test и отбросить фичи, которые не являются статистически значимыми.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Список фичей, которые не являются статистически значимыи</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>['Подрядчики, специализированная торговля — нигде более не классифицированные', 'Разнообразные издательства/печатное дело', 'Транспортировка — пригородные и локальные сезонные транспортные средства, включая электрички', 'Пассажирские железные перевозки', 'Автобусные линии', 'Агентства по автотранспортным перевозкам, местные/дальные автогрузоперевозки, компании попереезду и хранению, местная доставка', 'Услуги курьера — по воздуху и на земле, агентство по отправке грузов', 'Круизные линии', 'Авиалинии, авиакомпании, нигде более не классифицированные', 'Туристические агентства и организаторы экскурсий', 'Услуги по транспортировке — нигде более не классифицированные', 'Денежные переводы', 'Коммунальные услуги — электричество, газ, санитария, вода', 'Стоматологическое/лабороторное/медицинское/офтальмологическое стационарное оборудование и устройства', 'Промышленное оборудование — нигде более не классифицированное', 'Драгоценные камни и металлы, часы и ювелирные изделия', 'Товары длительного пользования — нигде более не классифицированные', 'Канцелярия, офисные сопутствующие товары, бумага для печатания и письма', 'Лекарства, их распространители, аптеки', 'Мужская, женская и детская спец-одежда', 'Химикалии и смежные вещества, не классифицированные ранее', 'Нефть и нефтепродукты', 'Книги, периодические издания и газеты', 'Товары недлительного пользования, не классифицированные ранее', 'Товары для дома', 'Оптовики', 'Универмаги', 'Универсальные магазины', 'Различные товары общего назначения', 'Продажа свежего и мороженого мяса', 'Кондитерские', 'Продажа молочных продуктов в розницу', 'Булочные', 'Продажа мотоциклов', 'Услуги по переделке, починке и пошиву одежды', 'Оборудование, мебель и бытовые принадлежности (кроме электрооборудования)', 'Покрытия для пола', 'Различные специализированные магазины бытовых принадлежностей', 'Магазины звукозаписи', 'Поставщики провизии', 'Магазины second hand, магазины б/у товаров, комиссионки', 'Магазины по продаже часов, ювелирных изделий и изделий из серебра', 'Магазины фотооборудования и фотоприборов', 'Магазины хрусталя и изделий из стекла', 'Прямой маркетинг — комбинированный каталог и торговцы в розницу', 'Прямой маркетинг — другие торговые точки прямого маркетинга (нигде более не классифицированные)', 'Магазины художественных и ремесленных изделий', 'Галереи и художественные посредники', 'Ортопедические товары', 'Табачные магазины', 'Дилеры по продаже печатной продукции', 'Зоомагазины', 'Плавательные бассейны — распродажа', 'Агенты и менеджеры по аренде недвижимости', 'Денежные переводы MasterCard MoneySend', 'Химчистки', 'Фотостудии', 'Службы знакомств', 'Сервисы по покупке/продаже', 'Иной сервис', 'Услуги копировальных центров', 'Информационные провайдеры', 'Фотостудии, фотолаборатории', 'Паркинги и гаражи', 'Ремонт бытовой техники, ремонт электроприборы', 'Производство и дистрибуция видеофильмов', 'Видеопрокат', 'Театральные продюсерские агентства', 'Туристические аттракционы и шоу', 'Луна-парки, карнавалы, цирки, предсказатели будущего', 'Клубы — сельские клубы, членство(спортивный, отдых, спорт), частные поля для гольфа', 'Услуги отдыха, нигде ранее не классифицируемые', 'Доктора, нигде ранее не классифицируемые', 'Дантисты, ортодонтисты', 'Оптика, оптические товары и очки', 'Больницы', 'Зубные и медицинские лаборатории', 'Колледжи, университеты, профессиональные школы и младшие колледжи', 'Школы — бизнес и секретарей', 'Образовательные услуги', 'Организации благотворительные и общественные службы', 'Ассоциации — гражданские, социальные и братские', 'Организации, членства, нигде ранее не классифицируемые', 'Профессиональные услуги, нигде ранее не классифицируемые', 'Судовые выплаты, включая алименты и детскую поддержку', 'Налоговые платежи', 'Почтовые услуги — только правительство', 'tr_type_1210', 'tr_type_1410', 'tr_type_1510', 'tr_type_2021', 'tr_type_2100', 'tr_type_2200', 'tr_type_2210', 'tr_type_2320', 'tr_type_2330', 'tr_type_2331', 'tr_type_2340', 'tr_type_2341', 'tr_type_2370', 'tr_type_2371', 'tr_type_2440', 'tr_type_2446', 'tr_type_2456', 'tr_type_4020', 'tr_type_4021', 'tr_type_4031', 'tr_type_4035', 'tr_type_4041', 'tr_type_4045', 'tr_type_4051', 'tr_type_4061', 'tr_type_4071', 'tr_type_4090', 'tr_type_4096', 'tr_type_4097', 'tr_type_4100', 'tr_type_4200', 'tr_type_6000', 'tr_type_6100', 'tr_type_7014', 'tr_type_7015', 'tr_type_7024', 'tr_type_7025', 'tr_type_7031', 'tr_type_7034', 'tr_type_7035', 'tr_type_7040', 'tr_type_7041', 'tr_type_7044', 'tr_type_7071', 'tr_type_7074', 'tr_type_8100', 'tr_type_8145', 'tr_type_8146']
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Сохраним датасет с фичами из списка</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Количество фичей после фильтрования</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-RenderedText jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/plain" tabindex="0">
<pre>130</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="4.-%D0%9F%D0%BE%D0%B4%D0%B3%D0%BE%D1%82%D0%BE%D0%B2%D0%BA%D0%B0-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85-%D0%B4%D0%BB%D1%8F-%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D1%8F-%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8.-%D0%9A%D0%B0%D0%BA%D0%BE%D0%B9-%D0%BF%D0%BE%D0%BB-%D0%BA-%D0%BA%D0%B0%D0%BA%D0%BE%D0%BC%D1%83-%D0%B8%D0%B7-%D1%82%D0%B0%D1%80%D0%B3%D0%B5%D1%82%D0%BE%D0%B2-(0/1)-%D0%BF%D1%80%D0%B8%D0%BD%D0%B0%D0%B4%D0%BB%D0%B5%D0%B6%D0%B8%D1%82.">4. Подготовка данных для обучения модели. Какой пол к какому из таргетов (0/1) принадлежит.<a class="anchor-link" href="#4.-%D0%9F%D0%BE%D0%B4%D0%B3%D0%BE%D1%82%D0%BE%D0%B2%D0%BA%D0%B0-%D0%B4%D0%B0%D0%BD%D0%BD%D1%8B%D1%85-%D0%B4%D0%BB%D1%8F-%D0%BE%D0%B1%D1%83%D1%87%D0%B5%D0%BD%D0%B8%D1%8F-%D0%BC%D0%BE%D0%B4%D0%B5%D0%BB%D0%B8.-%D0%9A%D0%B0%D0%BA%D0%BE%D0%B9-%D0%BF%D0%BE%D0%BB-%D0%BA-%D0%BA%D0%B0%D0%BA%D0%BE%D0%BC%D1%83-%D0%B8%D0%B7-%D1%82%D0%B0%D1%80%D0%B3%D0%B5%D1%82%D0%BE%D0%B2-(0/1)-%D0%BF%D1%80%D0%B8%D0%BD%D0%B0%D0%B4%D0%BB%D0%B5%D0%B6%D0%B8%D1%82.">¶</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Разделим данные на тренировочные и тестовые</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Сохраним customer_id для тестовой выборки, для проверки результата, если это потребуется</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Удалим customer_id из данных, т.к. эта фича не поможет в формировании предсказания</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Для того, чтобы определиться какой пол к какому из таргетов (0/1) принадлежит возникла идея сгруппировать таблицу train по таргету и просуммировать все фичи. После найти коды операций, количество которых резко отличается для категории таргета 1 и 0.</p>
<p>Для этого оставим только фичи с типом транзакции mcc</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Ветеринарные услуги</th>
<th>Генеральные подрядчики по вентиляции, теплоснабжению, и водопроводу</th>
<th>Подрядчики по электричеству</th>
<th>Подрядчики, специализированная торговля — нигде более не классифицированные</th>
<th>Разнообразные издательства/печатное дело</th>
<th>Авиалинии, авиакомпании</th>
<th>Агентства по аренде автомобилей</th>
<th>Жилье — отели, мотели, курорты</th>
<th>Транспортировка — пригородные и локальные сезонные транспортные средства, включая электрички</th>
<th>Пассажирские железные перевозки</th>
<th>...</th>
<th>Организации благотворительные и общественные службы</th>
<th>Ассоциации — гражданские, социальные и братские</th>
<th>Организации, членства, нигде ранее не классифицируемые</th>
<th>Профессиональные услуги, нигде ранее не классифицируемые</th>
<th>Судовые выплаты, включая алименты и детскую поддержку</th>
<th>Штрафы</th>
<th>Налоговые платежи</th>
<th>Правительственные услуги, нигде ранее не классифицируемые</th>
<th>Почтовые услуги — только правительство</th>
<th>gender</th>
</tr>
</thead>
<tbody>
<tr>
<th>1</th>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>1.0</td>
</tr>
<tr>
<th>2</th>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>1.0</td>
</tr>
<tr>
<th>3</th>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>2</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0.0</td>
</tr>
<tr>
<th>4</th>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>...</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0.0</td>
</tr>
<tr>
<th>5</th>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>3</td>
<td>...</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0</td>
<td>0.0</td>
</tr>
</tbody>
</table>
<p>5 rows × 185 columns</p>
</div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Сгруппируем данные по фиче gender, просуммировав остаток фичей и посчитаем дельту для каждой фичи по gender.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>Ветеринарные услуги</th>
<th>Генеральные подрядчики по вентиляции, теплоснабжению, и водопроводу</th>
<th>Подрядчики по электричеству</th>
<th>Подрядчики, специализированная торговля — нигде более не классифицированные</th>
<th>Разнообразные издательства/печатное дело</th>
<th>Авиалинии, авиакомпании</th>
<th>Агентства по аренде автомобилей</th>
<th>Жилье — отели, мотели, курорты</th>
<th>Транспортировка — пригородные и локальные сезонные транспортные средства, включая электрички</th>
<th>Пассажирские железные перевозки</th>
<th>...</th>
<th>Образовательные услуги</th>
<th>Организации благотворительные и общественные службы</th>
<th>Ассоциации — гражданские, социальные и братские</th>
<th>Организации, членства, нигде ранее не классифицируемые</th>
<th>Профессиональные услуги, нигде ранее не классифицируемые</th>
<th>Судовые выплаты, включая алименты и детскую поддержку</th>
<th>Штрафы</th>
<th>Налоговые платежи</th>
<th>Правительственные услуги, нигде ранее не классифицируемые</th>
<th>Почтовые услуги — только правительство</th>
</tr>
<tr>
<th>gender</th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
<tr>
<th>0.0</th>
<td>115</td>
<td>14</td>
<td>5</td>
<td>25</td>
<td>7</td>
<td>779</td>
<td>7</td>
<td>50</td>
<td>863</td>
<td>4106</td>
<td>...</td>
<td>100</td>
<td>215</td>
<td>481</td>
<td>16</td>
<td>7339</td>
<td>24</td>
<td>84</td>
<td>42</td>
<td>337</td>
<td>23</td>
</tr>
<tr>
<th>1.0</th>
<td>39</td>
<td>53</td>
<td>51</td>
<td>59</td>
<td>13</td>
<td>1096</td>
<td>32</td>
<td>216</td>
<td>955</td>
<td>3607</td>
<td>...</td>
<td>64</td>
<td>124</td>
<td>325</td>
<td>33</td>
<td>5569</td>
<td>7</td>
<td>182</td>
<td>62</td>
<td>607</td>
<td>20</td>
</tr>
</tbody>
</table>
<p>2 rows × 184 columns</p>
</div>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Полученный список отсортируем и посмотрим 10 самых небольших и самых маленьких значений</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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OVPffvttgrGGDRumjh076syZM5owYYLeffddbd++Xba2ttq1a5eaNm2qatWqafbs2cqWLZvSpk2roKAgLV26NEFfyb2mryIgIED16tVTrVq1FBwcnGS7GzduaOLEiRo8eLDVTBOpRVxcnDJnzqwlS5YkWp/cRJR4yf01e7xbt24pOjr6uUlZd+7cUfXq1eXm5qbRo0crX758cnBw0IEDBxQQEJDgfkvud++bb76Rv7+/mjdvrgEDBihz5sxKkyaNxo0bpzNnziRo3759e3Xo0EEffvjhSx3j6zB06FD5+PjIz89Pu3btSrLd999/L0m6fPmybt68mexktyxZsuibb76R9CShYOHChapfv752796tokWLJrqPt7e3bG1tdeTIkQR11atXlyTZ2lq/Zo2/VhMnTlSJEiUS7ffZJIrX9fyPH/v9999PMqGiWLFiVp9f5n6+fv16smZMcnFxeWECD/CySGgAAAAAAAAAALxWuXPn1vbt23Xv3j2rWRrip07PnTu3Vfv4X7U+7eTJk3JycnrpF45JKVGihHbt2qW4uDirKeX37t0rJycn85fdqVW+fPkSfbGWXHXr1tWcOXMUFRWl9evX64MPPlBISIj5Mj937tyKi4vTqVOnrKZhv3btmu7cuZPgmu3fv1+2trZJvrSLlzt3bp04cSJBeVL3QunSpVWjRg1JUoMGDfTnn3/q888/1/Dhw62u299x6tQpq18mnz59WnFxceYL4u+++06PHj3Shg0brH49Hb88wbMyZsyoOnXqWJWtX78+0bZFihQxZ6QoWrSoqlWrpm3btqlBgwZas2aNHBwctHXrVqslCoKCghLt60XX9FWtX79ev/zyS5LLXDxt7NixcnV1VZ8+ff7WmK8iLi5OZ8+etfrunjx5UtL/vezPly+ftm/frsqVKz/35W38fXjixAmrWR+io6N17tw58/rG3zdJ3dPOzs7KmDGjWRa/pMrzljYICQnRzZs3tXbtWlWrVs0sP3fuXKLt42fleNFyC6tXr1bevHm1du1aq3siqeSgvHnzqk6dOsqfP79CQ0MVExNjNUtD/Hf2dScxHTx4UMuXL9f69euTfLkvSXPnztW2bdv06aefaty4cerWrVuiSUOJcXBwsPqONm3aVOnTp9fMmTM1b968RPdxdnZWjRo1tHPnTv3555/KkSPHC8eJn0XBzc0twTPhVcU/m8+cOWOVsPTsPZgpUya5uroqNjb2tY39tLJlyyaYqScxI0eO1KhRo177+Pjf9nr+9AcAAAAAAAAA4P9r2LChYmNjNXPmTKvyL774QhaLRQ0aNLAqf/bl6cWLF/Xtt9/qrbfeeu4LrpfRqlUrXbt2TWvXrjXLbty4oVWrVqlJkyYvXOM+pbVs2VKHDh3SunXrEtQl55e8lSpVUpo0aeTs7Ky5c+fqp59+0pdffmnWN2zYUJI0depUq/2mTJkiSWrUqJFZFh0drQ0bNqhWrVov/CVuw4YNtW/fPv3yyy9m2f379zV//nx5eXmpUKFCz93/4cOHevz4sR4/fvzCY0yuWbNmWX2eMWOGJJn3Zfw99/R5jYiISDKx4FXFLx0Qv7REmjRpZLFYrH4Fff78+SSTI150TV9FbGyshgwZovfee++FySrnz5/XnDlzNGrUqJeeueB1efoZYxiGZs6cqbRp06p27dqSpDZt2ig2NlZjxoxJsO/jx491584dSVKdOnVkZ2en6dOnW133BQsWKCIiwrz/M2XKpDJlymjRokUJloTZsGGDGjRoYPXMWr58uezs7FSlSpUkjyGx+y06OlqzZ89OtP3q1avl6+ub6LIXL+p37969Vt/FxNSvX18RERFWM3PExcVp2rRpsre3f+0vywcNGqTKlSuradOmSbY5d+6cBgwYoJYtW2rIkCGaNGmSNmzYoMWLF7/SmNHR0Xr8+HGiyxA9bcSIEYqNjdX777+f6NITzz57S5curXz58mnSpEmJtr9+/fpLxxr/XJo+fbpV+bPP6jRp0qhly5Zas2ZNoslvrzL205YsWaJt27a9cOvQocPfGgdIDDM0AAAAAAAAAABeqyZNmqhmzZoaOnSozp8/r+LFi+v777/Xt99+q759+yZYC7xIkSKqV6+eevfuLXt7e/NFXmBg4AvH+u6773To0CFJUkxMjH777Tdz+v+mTZuaU2y3atVKFSpUUMeOHXXs2DFlzJhRs2fPVmxsbLLGSWkDBgzQ6tWr1bp1a3Xq1EmlS5fWrVu3tGHDBs2dO1fFixdPdl/16tXT+++/r4EDB6pJkybKli2bihcvLj8/P82fP9+cAn/fvn1atGiRmjdvrpo1a0qSfvvtNwUGBurSpUtq1KiROY27JDMpZf369Wrbtq2yZMmiQYMGadmyZWrQoIF69+6t9OnTa9GiRTp37pzWrFmTYNaFbdu26dKlS+aSE0uWLFHTpk1lZ2f3Gs7iE+fOnVPTpk1Vv359/fLLL/rmm2/03nvvmefwrbfekp2dnZo0aaJu3bopMjJSX375pTJnzpzosiXJ8eWXX+qnn35SqVKl5ObmpmPHjunLL79UtmzZzJfvjRo10pQpU1S/fn299957+uuvvzRr1ix5e3vrt99+e27/iV3TeBcuXNCWLVus2l+/fl0PHz7Uli1bVL16dTMh4dKlS+byGi+yc+dOFSxYUB07dnxuO39/f/Oav85f9zs4OGjLli3y8/NT+fLl9Z///EebNm3SkCFDzJldqlevrm7dumncuHEKDw/XW2+9pbRp0+rUqVNatWqVpk2bplatWilTpkwaPHiwAgMDVb9+fTVt2lQnTpzQ7NmzVbZsWb3//vvmuBMmTNBbb72lihUrqkuXLoqKitKsWbPk4OCgTz/9VNKTWUBGjhypZcuWadCgQXJzc0vyOCpVqqR06dLJz89PvXv3lsVi0ddff53gZfnZs2c1YcIE7du3Ty1atLD67oWFhUl68v3JlSuX8ubNq8aNG2vt2rV6++231ahRI507d05z585VoUKFEn3ZHq9Lly6aO3euevToocOHD8vX11fffvuttm3bpnHjxilDhgxW7U+cOGF1f0VGRsrGxsaqLH42gZ07d8rNzc1qeZLvv/9eoaGhScZjGIY6deokR0dHzZkzR5LUrVs3rVmzRn369FGdOnVeuGTQ/fv3rZac+PrrrxUVFaW33377uftVrVpVM2fO1EcffSQfHx+1a9dOBQoUUHR0tE6ePKklS5bIzs7OXPrCxsZGX331lRo0aKDChQurY8eOypEjh/7880/t2LFDbm5u+u6775475rNKlCihtm3bavbs2YqIiFClSpX0ww8/6PTp0wnajh8/Xjt27FD58uXVtWtXFSpUSLdu3dKBAwe0fft23bp166XGflrlypVfed9n/fbbb9qwYYOkJzPkREREmH9uFy9eXE2aNHltY+G/hAEAAAAAAAAAwN/Qs2dP49l/br53757x8ccfG9mzZzfSpk1r+Pj4GBMnTjTi4uKs2kkyevbsaXzzzTeGj4+PYW9vb5QsWdLYsWNHssb28/MzJCW6BQUFWbW9deuW0blzZyNDhgyGk5OTUb16dSMsLCxZ4+TOndto1KhRgvL4+J927tw5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pEkTc3mNpUuX6tGjR2b9N998oxw5cqhWrVrJPlc//PCDjh8/rpCQEC1btkxr165VYGBgss9B5cqVFRQUpNatWyd4US9Jffr00ZkzZ7R27VqlTZs2Qf327dt15coVrVmzJkFd69at9ddff+k///mPfv31V5UqVUq1a9fWrVu3kn18z1q7dq0OHjxoVXbnzh298847qlGjho4dO6YrV66oTZs2L+yrcOHCunLlis6fP68+ffqof//+On78eLLHfVrXrl3N+zBnzpxWdUuWLNGIESP06aef6vjx4/rss880fPhwLVq0SJJ0//591atXT+nSpVNYWJhWrVql7du3J3mPSVJgYKAeP36c5DHFb8eOHbOqHzBggPr166eDBw+qYsWKatKkiW7evJnkOI8ePdLdu3etNgAAAAB4VSQ0AAAAAACAf70cOXKof//+KlGihPLmzauPPvpI9evX18qVK63axcTEyM7Ozpzh4ekkgkePHumzzz7TwoULVa9ePeXNm1f+/v56//33NW/ePKt+Ro4cqbp166po0aJatGiRrl27pnXr1kl6khDQrl079e3bVz4+PqpUqZKmT5+uxYsXKyoqKkHsixYt0qNHj9SsWbMEdd9++62aNm0qSWrRooVZFi84OFj+/v6yWCxydHSUJD18+PC558rOzk4LFy5U4cKF1ahRI40ePVrTp09XXFxcss9By5YtFRgYqIYNG+rChQtm+YQJE/Ttt99q8+bN5uwZT59fSea5T58+vVX97t27tW/fPq1atUplypSRj4+PJk2aJA8PD6sZIl5GTEyMAgICFBAQYFV+8uRJPXjwQAEBAcqTJ4+yZs1qnr/nsbW1VdasWZUzZ07lypVLadKkkbOzc7LHjffo0SO5u7ub5yJNmjRW9SNHjtTkyZPVokUL5cmTRy1atNDHH39sXoOlS5cqKipKixcvVpEiRVSrVi3NnDlTX3/9ta5du5ZgvJMnT2rhwoX6+OOPkzym+C1z5sxW9b169VLLli1VsGBBzZkzR+7u7lqwYEGS52jcuHFyd3c3N09PzyTbAgAAAMCLkNAAAAAAAAD+9WJjYzVmzBgVLVpU6dOnl4uLi7Zu3Wr1sl2S7t69m+gLaEk6ffq0Hjx4oLp168rFxcXcFi9erDNnzli1rVixovn/6dOnl6+vr/lL/UOHDik4ONiqj3r16ikuLk7nzp2z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y9/fP8bjSNGvWS8vL6vYnle/fn3zRfLJkyfl6OioRYsWmeVLly6Vg4ODTpw4EeP+z/fx816Mq0+fPsqZM6ccHR2VPXt2DRw4UE+ePDHLhwwZEuu5RrX94j0lSe+//74sFosCAwPjHBuLxaLg4OBo8d65c0cFCxZU8+bNZRiGJOnx48fq0qWL0qVLpxQpUqhcuXLav39/tHO2WCyysbFRunTp1Lp1a4WFhcXYR1L0MYk65+efCfv371e1atWUJk0aubm5qUKFCjp48GCsbUr/P+ONxWKRnZ2dcufOrQULFsR6jOe9+NyJqW5M47t8+XLly5dP9vb28vLy0rhx46z2efz4sfr06SNPT0/Z29vL29tbs2fPjvUcli5dqkKFCilTpkzmNn9//1jHMTAwMNbYXry/X7wmUqVKpY8++ki3bt0y97l48aLq1asnZ2dnubq6qnHjxrpx40as8cakYsWK5jEcHBxUuHBhrV+/3ix/8e+IW7duKWXKlC/9OyIh/f+iF9sNDw+Xt7d3jPfti56/vqKW56/j+D7nnn/+DBgwQJkzZ1ZwcLC5befOnSpfvrwcHBzk6empLl266MGDB1ZtxPWslKSUKVOqbNmyWrx4cZznBAAAAABvCgkNAAAAwL9cq1atNHfuXHN9zpw5atmyZbR6Dx48UPfu3fXHH39o8+bNsrGx0YcffqjIyEireps2bdK1a9fMpVq1avHa383NTaNGjVJgYKAOHDigHDly6JNPPok17l69eilFihRvogviLTQ0VBUqVNCVK1e0Zs0aHT58WL17947WBy96sU8yZ84crc7AgQPVoEEDHT58WE2bNtUnn3yioKAgSc/6ztfXVylTptT+/fu1bNkybdq0SZ07d47zeMuXL49WZmNjo8mTJ+v48eOaN2+etmzZot69e5vljRo10qBBg1SzZk1dunTJat/IyEg1adJELi4umjVrlrl95MiRmj9/vr7//nsdP35cX375pT777DNt3749xvgOHDigNWvWxNln0rPp70eNGqWBAwfqxIkTWrRokdKnTx/jucbVt1EePHiggQMHytnZOVrZmDFjVKhQIR06dEh9+/ZV165dtXHjRknPXnA/3/7EiRPN9Y8//vil5/GqcufOrbFjx6pjx466ePGiLl++rA4dOujbb79V3rx5X6ttFxcX+fv768SJE5o0aZJmzpypCRMmWNXJly+fVZ/GdB09b8WKFTp06JC57unpae4blZS0b98+c5unp6fV/qGhoapZs6ayZ8+uOXPmmC/3e/fureXLl2vevHk6ePCgvL295evrq9u3b1vtf+rUKV25ckU//vijlixZYvU8S4j79++rRYsW2rlzp/bs2SMfHx/VrFlT9+/fj3O/6tWr69q1azpz5ozq1Kmjli1bRks6elMOHDigxo0b65NPPtHRo0c1ZMgQDRw40EywkaTmzZvrp59+0uTJkxUUFKQffvghxms/yo4dO1S8ePFo211dXa2uh+cTzWKLLbb7O+p+Xbt2rfbt26fRo0dLevZsqVevnm7fvq3t27dr48aNOn/+fILur7Zt2+ratWs6duyY8ufPb5V89aKhQ4cqIiLilY8Rn/5/me+++y7eCRuGYZjX17Vr11S6dOlY68b1nIsybtw4/fDDD9q4caO8vLwkSefOnVP16tXVoEEDHTlyREuWLNHOnTuj/T0T17MySsmSJbVjx45Yj//48WOFhIRYLQAAAACQUMkSOwAAAAAAb9dnn32mfv366c8//5QkBQQEaPHixdq2bZtVvQYNGlitz5kzR2nTptWJEyeUP39+c3vq1Knl4eER7Tgv2z99+vSqUaOGJCkiIkJZs2aNFkOUrVu3ateuXWrTpo22bt36qqecYIsWLdLff/+t/fv3K1WqVJIkb2/vl+73Yp/Y2tpGq9OoUSO1adNGkjR8+HBt3LhRU6ZM0bRp07Ro0SKFhYVp/vz5cnJykvTsZVidOnX07bffmi/5Hz9+LEny8PCQh4eHGePzXvzF7tdff60OHTpo2rRp5vYvv/xSFy9eVI0aNbRz505z+xdffKHg4GDt2LFDyZMnN485YsQIbdq0yXzJlj17du3cuVM//PCDKlSoEC2G7t27q1evXho4cGCsfXb//n1NmjRJ3333nflCMkeOHCpXrpxVvfj0bZTRo0crb968Mb7ALFu2rPr27StJypkzpwICAjRhwgRVq1ZNadOmtWrfzc0txmv8TerYsaPWrVunzz77THZ2dipRooS++OKL1253wIAB5p+9vLzUs2dPLV682CqpJVmyZFbnF9N1FOXJkyfq06eP+vTpY46nra2tuX/UbAlp06aNsc8eP36shg0bytHRUUuWLFGyZM/+M8SDBw80ffp0+fv7m8+FmTNnauPGjZo9e7Z69epl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r18/eXt76/PPP9fq1aslPfvmeo0aNTR06FB16NDBnHY+b968sre318WLF6363dvb2+rX1pI0ffp0OTs7q1mzZi/tDx8fHzk4OGjz5s0vrfsygYGB+vnnn/X111/HWieu/o8vDw8Pq/OP6aVumjRp5O3trUKFCqlfv366c+dOjL/8v337tvz8/NS/f3/5+fmpadOmevTo0UtjyJYtm1UMz9u1a5eyZs2q/v37q3jx4vLx8YlzWviXGT58uMqXL6/3338/wW2sWbNGH330kdq2bauWLVua0+TnyJFDdnZ2VjNYPHnyRPv371fevHmt2og652rVqqlBgwZauXJlnMd0c3Oz6qMXZ1wJCAhQly5dVLNmTeXLl0/29vZWz6HYRD178uTJo+7du8vOzk6bNm0yy1/luRNVN2rJlCmTVXmePHmize4REBCgnDlzytbWVgUKFFBkZKS2b9/+0rijFClSRCdOnIh3/RfF5/729PSUt7e3ypUrp5YtW5pjlSdPHl26dMnql/onTpzQ3bt3o433y0SNb/78+TV48GBduXJF+/btM8ujZvkZOHCgUqZMGWMbr9v/cenTp4/atGkTr88VSc8+vxIUFKQiRYrEWS8+z7m+ffuqYcOG8vf314QJE7R//36zrGjRojpx4kS057i3t7fVJy7i86w8duzYS+MFAAAAgDeFhAYAAADgP8DW1lZBQUE6ceJEjC9jUqZMqdSpU2vGjBk6e/astmzZou7du8e7/fjsv23bNm3evFnBwcE6ePCgBg0aJE9PT6vPXyxatEg5cuQwP4OQUIZhKCwsTA8ePNCWLVt04sSJaNNvx6RJkyby8PBQ/fr1FRAQoPPnz2v58uXavXv3a8UjScuWLdOcOXN0+vRpDR48WPv27VPnzp0lPfvFcYoUKdSiRQsdO3ZMW7du1RdffKFmzZopffr0evr0qf73v/9p0aJF+uijj3T9+nVdv37dTLz466+/JD1LFnny5ImmTJmi8+fPa8GCBfr++++t4tizZ4/mzJmjGTNmyGKxmC/8ov63a9eucnV11fDhwyVJLi4u6tmzp7788kvNmzdP586d08GDBzVlypRoU72PHj1a48aNi9ev+VOkSKE+ffqod+/e5ucr9uzZo9mzZ79y344dO1bdu3eP8xfOAQEBGj16tE6fPq2pU6dq2bJl6tq16ysf62UiIiIUFhamW7duac6cOXJzc4uW+CFJHTp0kKenpwYMGKDx48fr6dOnr/1rdh8fH128eFGLFy/WuXPnNHny5Je+/I/Nw4cPNWPGDI0ePfq1YopKJhg1apTu3LljfobByclJn3/+uXr16qX169frxIkTatu2rR4+fKjWrVtbtfHXX3/p+vXr2rt3r3755Rflzp37tWLy8fHRggULFBQUpL1796pp06bxmvHg8ePHun79ui5fvqxZs2bp9u3bVrEk9LkTkx49emjz5s0aPny4Tp8+rXnz5um7774zrxEvLy+1aNFCrVq10qpVq3ThwgVt27ZNS5cujbVNX19f7d69O16fTIhJfO7vW7du6fr16zpy5Ih++ukns3+qVq2qAgUKqGnTpjp48KD27dun5s2bq0KFCjHOdBKXhw8f6vr16/rzzz81fvx4JUuWzCp5YPPmzbp37546deqUoPOUXt7/sTl79qy2bdumQYMGxes4J0+eVJMmTeTu7h7tsxcvis9zLup+K1mypLp166aWLVuaM4/06dNHu3btUufOnRUYGKgzZ85o9erV5t9DUeLzrNyxY4c++OCDeJ0jAAAAALwuEhoAAACA/4i4pn22sbHR4sWLdeDAAeXPn19ffvmlxowZE++247P/nTt39MUXXyhPnjyqVq2anjx5orVr11rVefjwYazfBn8VR44ckYODg1xdXeXn56cePXrok08+eel+dnZ2+v3335UuXTrVrFlTBQoU0KhRo176i9z4GDp0qBYvXqyCBQtq/vz5+umnn8xfJjs6OmrDhg26ffu2SpQooYYNG6pKlSr67rvvJEmXLl1ShQoV9PDhQ3Xp0kUZMmRQhgwZ1KBBA0kyZ3EoVKiQxo8fr2+//Vb58+fXwoULNXLkSDOGiIgItWvXTv369VPOnDljjNPW1lYzZ87UhAkTdOzYMUnPfqk/cOBAjRw5Unny5FH16tW1du1aZcuWzWrfSpUqqVKlSvHuk4EDB6pHjx4aNGiQ8uTJo48//thMzngVLi4u6t27d5x1evTooT/++ENFihTR119/rfHjx8c4W8nr6tWrlxwcHOTp6akdO3Zo5cqVsre3t6ozf/58rVu3TgsWLFCyZMnk5OSkH3/8UTNnztRvv/2W4GPXrVtXX375pTp37qzChQtr165dGjhwYILaevLkiVq2bBnrdfKqnJycNGfOHH3zzTfmdTVq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4cOHVnUfP36sL7/8UmnTppWLi4vq1q2ry5cvxxjzlStX1KpVK6VPn1729vbKly+f5syZY1Un6rm5ePFiDRgwQJkyZZKjo6NCQkJe2ievKyQkxEyAjEpmkKTmzZvL2dlZS5cufesx4J+HGRoAAAAAAAAAAG+UYRiqW7eutm7dqtatW6tw4cLasGGDevXqpStXrmjChAlW9bdv364lS5aoS5cusre317Rp01S9enXt27dP+fPnfyMxHTp0SEWLFo3269OSJUtqxowZOn36tAoUKBBnG2fPntWnn36q9u3b67PPPtPYsWNVp04dff/99/rqq6/UsWNHSdLIkSPVuHFjnTp1yup4T58+VY0aNfT+++9r9OjRWrhwoTp37iwnJyf1799fTZs21UcffaTvv/9ezZs3V+nSpZUtWzZJz170lS9fXkFBQWrVqpWKFi2qmzdvas2aNbp8+bLSpEkT775o06aNtm3bpo0bNypv3rxW2+fNm6eGDRuqR48e2rt3r0aOHKmgoCCtXLkyxraaNGmimjVrSpLWrVunn376yar8xo0bKlOmjB4+fKguXbooderUmjdvnurWrauff/5ZH374oVX9r776Snny5NGjR4+0ZMkSffXVV0qXLp1at24d4/Hz5Mlj9amTGTNmKCgoyOoai/okQpTGjRvLy8tLI0eO1J49ezR58mTduXNH8+fPN+tMnz5d+fLlU926dZUsWTL98ssv6tixoyIjI9WpU6e4ujdG4eHhcnFxUdeuXZU6dWqdO3dOU6ZM0ZEjR3T06FGz3qRJk1S3bl01bdpU4eHhWrx4sRo1aqRff/1VtWrVirX92Mb0dQ0aNChaskdMIiIi1L9//zdyzOnTp1vNtnLhwgUNGjQoWr2nT5+qevXqeu+99zR69GitX79egwcPVkREhIYNG2bWa9++vfz9/dWyZUt16dJFFy5c0HfffadDhw4pICBAyZMnl/TsBfPQoUNVtWpVff755zp16pSmT5+u/fv3m/Vu3bolSerXr598fHw0dOhQhYWFaerUqSpbtqz279+vnDlzRou1fPnyateunaRnL+hHjBhhVe7v7y9nZ2d1795dzs7O2rJliwYNGqSQkBCNGTMmxn6qVq2a+ZJ///79mjx5slV5SEiIZs2apSZNmqht27a6f/++Zs+eLV9fX+3bt0+FCxeOsd3w8HBVrVpVJ0+e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pk8//VTjxo1Tz549bSYN2eLi4mJxj77zzjvKkSOHZsyYoTlz5tjcJ2vWrPL399fu3bt1/fp1FShQINV+EmdR8PDwsHomPK/EZ/OFCxcsEpaevQZz584td3d3xcfHv7C+k6pcubLVTD22jBw5UqNGjUq2vEyZMnJwcNChQ4csllp6/PixIiIiLLYBiV7MX38AAAAAAAAAAP6/Jk2aKD4+XjNmzLDY/sUXX8hkMqlx48YW2599eXr16lWtW7dODRo0SPEFV3q8++67unXrltasWWNs++233/Ttt9+qadOmqa5xn9Fatmypo0ePau3atVZlafklb/Xq1WVvb6+sWbPqq6++0g8//KB58+YZ5U2aNJEkTZ061WK/KVOmSJLeeustY9vjx4+1fv161a1bN9Wp9Js0aaIDBw5o//79xraHDx9q7ty58vHx0SuvvJLi/n/++aeePHmiJ0+epHqMaTVz5kyL719++aUkGddl4jWXdFyjoqKSTSx4XolLByROvW5vby+TyWTxK+jIyMhkkyNSO6fPIz4+XkOHDtW//vWvVJNVIiMjNXv2bI0aNSrDpolP+owxm82aMWOGHB0d9eabb0qSWrdurfj4eI0ZM8Zq3ydPnuj+/fuSpHr16snJyUnTp0+3OO8LFixQVFSUcf3nzp1br732mhYtWmS1JMz69evVuHFji2fW119/LScnJ73xxhvJHoOt6+3x48eaNWuWzfqrVq1SiRIlbC57kVq7P/30k8W9aEujRo0UFRVlMTNHQkKCpk2bJmdn5xf+svyjjz5SjRo19M477yRb59KlSxo0aJBatmypoUOHatKkSVq/fr0WL178XH0+fvxYT548sbnsQVIff/yx4uPj1b59e5tLTzz77K1UqZKKFSumSZMm2ax/586ddMea+FyaPn26xfZnn9X29vZq2bKlVq9ebTP57Xn6TmrZsmXatm1bqp+OHTum2I6np6fq1aunpUuX6o8//jC2L1myRNHR0WrVqtVfihMvJ2ZoAAAAAAAAAAC8UE2bNlWdOnU0bNgwRUZGqly5cvruu++0bt069e/f32ot8DJlyqhhw4bq27evnJ2djRd5o0ePTrWvDRs26OjRo5KkuLg4HTt2zJj+/5133jGm2H733XdVtWpVde7cWadOnVKudjcP6gAA8FNJREFUXLk0a9YsxcfHp6mfjDZo0CCtWrVK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TZpIkvz8/HTlyhVjqvzp06dr7dq1Vu24u7vLwcFBDg4OCg0N1Zw5c7Rnzx5Jkq+vr+Li4vTll1/q4sWLWrJkib766itj34SEBK1fv15Dhw5Vx44drV4EJwoODta+ffvUp08f45fy69atU58+fSzqzZw5U82bN1eFChX+0tgkJCQoJiZGf/zxh1auXKm7d+9aTd8vSaNHj9a4ceM0ffp0nT17VsePH1dISIimTJmSpn4+//xzjRo1yiKBIJGfn58OHTqkrVu36uzZsxoxYoTVLBEpScv+s2bN0smTJxUZGamlS5dq27ZtVmM3YcIETZ482WKpg+cRFxenmJgY3bx5U0uXLlXx4sWTTUhISZ8+ffTgwQO99957OnTokM6dO6clS5bozJkzRp2GDRvKw8NDY8eOVefOndPdR+/evXXv3j21bdtWBw8e1IULF7R161Z17tzZYnmHK1euaMCAATpz5oxWrFihL7/8Uv369bNqz2Qy6auvvtKkSZNsJu34+flp27Zt2rdvn06fPq2ePXvq1q1bVvXS0l9igs7rr7+u/v37W8zKkdb7KDVPnjxRTEyM7t69q4ULF8rT01Pe3t7pagMAAAAA/ioSGgAAAAAAeIlt2bJF+fLlU758+VSlShX9+OOPWr58ufz9/SVJ77zzjj788EP16dNH5cuX1759+zRixIgU23z11Vc1bNgwY+mJcuXKacqUKfr8889VpkwZLVu2TOPGjTPq//7773r//ffVqVMnTZ48OcV2d+/erbNnz6pmzZqqUKGCPv74Y6ulDRISEvTpp58+/6D8fxs2bJCrq6ty5Mih4cOH68svv1TVqlWt6nXr1k3z589XSEiIypYtq9q1ays0NFRFihRJUz+vv/66BgwYYDNZoGfPnmrRooXatGmjKlWq6O7duxazLaQmLftv2rRJ/v7+KlmypEaPHq2hQ4daLc9Qp04dmwkX6dW6dWu5urqqePHiunHjhlauXGmzXmBgoHEN2pIzZ059//33io6OVu3atVWpUiXNmzfPIjnCzs5OgYGBio+PV8eOHdMda/78+RUeHq74+Hg1aNBAZcuWVf/+/ZUtWzZjphFJ6tixo/7880+9/vrr6t27t/r166cePXrYbLN+/frq3r27zbLhw4erYsWKatiwofz9/eXl5aWAgACreunpT3qacJOQkGAsPZHW+yg1gwYNkqur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6tUxZ84clChR4rPXCQCzZ8+GlZUVatasiebNm8PX1xcVK1aUwufNm4e7d+/iwIEDuW5fRkYGpkyZ8pfyk5uKFSti48aNWL9+PcqVK4fx48dj0qRJCAgIkOIsWbIE7dq1w4ABA1C6dGkEBgYiKSkpT+upX7++xp5gNNHR0cH69etx6dIllCtXDsOGDcOMGTM0xm3YsCHs7Ozg4+MDa2trrFixQqt1aHt+U7G1tcXo0aM1no+8vLwwe/Zs/PTTTyhXrhzWrl37WcddWloaevTogVKlSuV5WeDTNu3Zswd169aV0unUqRMePnyIokWLAvjUo8OmTZuwY8cOeHt745tvvsH58+ezTXPixInIyMjAhAkTvlg+iYiIiIiI/iqFEELkdyaIiIiIiIiI/osmT56MTZs24erVq/mdFSKir+Lt27ewsLDAn6MHwtxQma950Q+bla/rJyIiIiL6L1M9GyQkJMDc3Fzr5dhDAxEREREREdHfLDExEdevX8fChQsxePDg/M4OEREREREREVGBxAYNRERERERERH+zQYMGoVKlSqhXr95nDzdBRERERERERPRvp5ffGSAiIiIiIiL6r4mIiEBERER+Z4OIiIiIiIiIqEBjDw1ERERERERERERERERERERU4LBBAxERERERERERERERERERERU4HHKCiIiIiIiIiIiIvir9MVOhb26e39kgIiIiIqJ/GPbQQERERERERERERERERERERAUOGzQQERERERERERERERERERFRgcMGDURERERERERERERERERERFTgsEEDERERERERERERERERERERFThs0EBEREREREREREREREREREQFDhs0EBERERERERERERERERERUYGjl98ZICIiIiIiIiIion+3tB+/R5qhMl/WrR82K1/WS0REREREfx17aCAiIiIiIiIiIiIiIiIiIqIChw0aiIiIiIiIiIiIiIiIiIiIqMBhgwYiIiIiIiIiIiIiIiIiIiIqcNiggYiIiIiIiIiIiIiIiIiIiAocNmggIiIiIiIiIiIiIiIiIiKiAocNGoiIiIiIiIiIiIiIiIiIiKjAYYMGIiIiIiLKMyEEPn78mN/ZINIoIyMDGRkZ+Z0NIiIiIiIiIiL6i9iggYiIiIiIcpWUlIQJEyagcuXKsLW1hVKpxIoVK/I7W0QAgJcvX2LEiBEoX748bGxs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Bj73GqFtGQB/z3OXtvtydn9H0WTMmDFISEiQpsxDkhAREREREeVVnhs01K9fH1FRUbhz5w4+fPiA1atXSw9hM2bMwLx58xASEoKjR48iKioKvr6+al3iT5o0CZcuXcLcuXMxe/Zs2UPS06dPAXz6Q21O3rx5g8mTJ2P27Nlq41g2adIEnTp1QrVq1XJ8MTBnzhxERUVJU+XKldXijBw5ElFRUTh48CAcHBzQvHlzte1JTEyErq4uLl26JEsvJiZG6tY2v/3xxx8AgJIlS/6ldMzMzBAVFYWrV69i69at+N///octW7bkKY2nT5/mWr9dunRBVFQUTpw4gTp16qBdu3Z48uTJF+suXlX358+fh62trdR9pLZ1qSoH1bRnzx6N6zl58qQsniYbNmzAlStXsG7dOty5c0fjS/rExERUqlRJllZUVBRu376d6x94CxUqBF9fX6xZswarVq3S+AeQ5s2b4/Xr11i+fDnOnTuHc+fOAUCuw1nkdfmoqCicOXMGVapU0dg95Zo1a5CUlKSxDID/O/+opsxdg6u4u7tLdTt69GiMHz8emzdvznUbVqxYoVa+OU0rVqzQpmhypE3dZ46bef2ajqHz589jz549uH79OpYuXaoxnTt37mDFihX46aef/lLeu3btij179mD9+vWwtbWFp6enLPzMmTPo0qULmjRpgl27duHKlSsYO3as1vuUtsu3aNECV65cwW+//YZz585h27ZtamkFBwdjxIgRsLOz07iuL3Ut0ORLD3HxJdJLTEyUuozPPN25cwd169bVOh1Nx+KIESOwbds2TJ06VTr/eXp6SmWVW/7/7iFBcpKWloZRo0ZhypQp2eZLT08PAQEBWLFiBZYuXSq9JFdRdYu8fPlyWXldv35dNhQQoN0x/iX4+fnh4cOH2Lp1K+7fv48mTZp8lfV8SX/88QdKlCihdr+nou35IjY2FuPHj8fGjRulbvwfPHiA7du3Y8aMGfj999+luKquoM3NzbF27VpcuHBBOr9oex77K96+fYukpKQc94PevXtj/fr1+PDhA8LDw9GxY8ccG31oIv7/UG/alGF2QxgByLZucjJ27Fi0b98eXl5eGsMjIyOxYcMG2bjuKto+c3wJJ0+eRHR0NA4cOIDIyEi1scy/BFU9qHypa3Vux3tiYiLs7OzUrge3bt3CyJEjpXiqe6uc7oHycm98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XL9+HQAQGhqK4OBgjB8/Hh4eHujYsSPi4uKyXXd4eDh+/fVXHDhwAAAwZMgQDB8+HMHBwfD09MS+ffuwY8cOuLm5yZZ1dXWFv79/nsoiKSkJ06ZNy7bnjKxGjx6NMmXK5LieH374AbGxsVi2bBmATw1Edu3ahQMHDqBKlSqoXr065syZI/VooK0lS5agXbt2GDBgAEqXLo3AwEAkJSVpjGtiYoJVq1ZhypQpUj1MmzYNbdu2Rbdu3VCxYkXcvXsX+/fvV+uZon79+qhfv77W+cot3U6dOuHo0aOIjIyEnZ2dND1+/Bjjx4/Hhg0bAHzqGWTFihUIDw+Hp6cnfHx8EBERIQ0V8TllX6FCBTx79gwzZsyQ1qvq2aNhw4Z49OiRtOzIkSNhZGQER0dHnDx5Etu2bYNSqdS6HIiIiIiIiL4EhRBC5HcmiIiIiIiIiIgKsl69euHly5fYsWNHfmeF/uHq1auHCRMmoF69emphQUFB8Pb2RkBAwFdZt0KhQHZ/CvT29sb27dvh5OT0Rdf59u1bWFhY4M/RA2Fu+PUaROiH/fVGUkRERERE9PWong0SEhKy/RBDEw45QURERERERESUjYSEBFy7dg2//vorGzPQF2FtbQ0DAwONYebm5jAyMvpq6y5atGi2YYULF9Y4VA0REREREVF+Yg8NRERERERERETZqFevHs6fP4++fftizpw5+Z0don8c9tBAREREREQAe2ggIiIiIiIiIvrijh07lt9ZICIiIiIiIvrP0snvDBARERERERERERERERERERFlxQYNREREREREREREREREREREVOBwyAkiIiIiIiIiIiL6qvTHTIV+HsbJJSIiIiIiAthDAxERERERERERERERERERERVAbNBAREREREREREREREREREREBQ4bNBAREREREREREREREREREVGBwwYNREREREREREREREREREREVOCwQQMREREREREREREREREREREVOGzQQERERERERERERERERERERAWOXn5ngIiIiIiIiIiIiP7d0n78HmmGyq+Wvn7YrK+WNhERERER5R/20EBEREREREREREREREREREQFDhs0EBERERERERERERERERERUYHDBg1ERERERERERERERERERERU4LBBAxERERERERERERERERERERU4bNBAREREREREREREREREREREBQ4bNBAREREREREREREREREREVGBwwYNREREREREREREREREREREVOCwQQMRERERERHRP1jNmjVx9+5dJCcno06dOrh+/Xp+Z4mIiIiIiIiI6ItggwYiIiIiIiL6TwsICIBCoch2io+Pz+8s5mjQoEEoV64cTE1NUbhwYZQtWza/s0RERERERERE9EWwQQMRERERERH95zVu3BjPnj2TTVu2bMnvbGnlu+++w+vXr/H06VNs27YNCoUiv7NERERERERERPRFsEEDERERERER/ecplUrY2trKJmtra1mciIgIWFpaYvv27XBzc4OhoSF8fX3x6NEjWbxp06bByckJenp6Ui8Pc+fOBQA8ePAACoUCRYoUQWpqqrRMdHQ0FAoFnJycpHkZGRmYNGkSHBwcoFQq4e3tjX379knhqrSioqJgbGwMGxsbhIaGytaniapHitmzZ8vmt27dGgqFAhEREdK8kJAQlCpVCsbGxnB2dkZoaCjS0tKk8AkTJsDb2xtLly6Fo6MjjI2N0aFDByQkJMjW16pVK+n33r17YWpqir1790rzHj16hA4dOsDS0hLW1tZo2bIlHjx4IK0ju94z6tWrp3Edr169gpWVFSwtLdXymtmxY8dkvXBERERoXE9iYmK25flXZbfOrPvDkiVL4OLiAgMDA7i7u+Pnn3+WpaNQKLBkyRL4+fnByMgIzs7O2Lx5sxSu2l+yTrt27QIApKSkYMiQIbCxsYGhoSFq166NCxcuqJWVQqGAjo4ObGxs0KtXLyQnJ8vyUa9ePbV1ZN4fz5w5gxo1asDU1FQKz1ovmWWtW9W2bt++Xfqd0/6TOY2JEyeiSJEiMDc3R79+/WTHYEZGBn788UeULFkSRkZG8PLykpXfiRMn4OHhAWNjY1hYWMDX1xd37tzJNt9Z97fLly/D0tISK1askObNnj0bnp6eMDExgaOjIwYMGCDta5nLW9MEfNrPO3fuDHt7exgbG8PT0xPr1q1Ty4umfSxz3vJS95knDm9DRERERER/BzZoICIiIiIiItLS+/fvMWXKFKxZswaRkZGIj49Hp06dpPADBw5g7NixmDhxIh4+fIhnz57BwcFBLR2lUomtW7dKv5cuXQp7e3tZnHnz5mHWrFmYOXMmrl69Cl9fX7Ro0SLbl6iPHz/G3LlzYWRklOt22NvbY/ny5dLvp0+fIjIyEsbGxrJ4ZmZmiIiIwM2bNzFv3jwsX74cc+bMkcW5e/cuNm7ciJ07d2Lfvn24cuUKBgwYoHG9J0+eRIcOHbBy5Ur4+fkBANLS0uDr6wszMzOcPHkSkZGRMDU1RePGjZGamooRI0ZIvWYEBwejRo0a0u/MZZjZxIkT8fHjx1zLQRNzc3O13jpMTEw+Ky1tdOzYUVrP3Llz4eDgIP1WvVTetm0bhg4diuDgYFy/fh19+/ZFjx49cPToUVlaoaGhaNu2LaKjo9GlSxd06tQJMTExsjiHDh2SbVujRo0AAKNGjcKWLVuwevVqXL58Ga6urvD19cXr169ly9+6dQtPnjzBL7/8gg0bNiA8PFwWLoRAYGCglH7W/b9du3ZwdHTElStXpDr9K3Lbf1QOHz6MmJgYHDt2DOvWrcPWrVsxceJEKfzHH3/EmjVr8L///Q83btzAsGHD0LVrVxw/fhzAp2Nm4cKFuHHjBk6dOgUdHR307dtXqzz+/vvv8PX1xbhx49C7d29pvo6ODubPn48bN25g9erVOHLkCEaNGgUAqFmzplpvMZnrDQCSk5NRqVIl7N69G9evX0efPn3QrVs3nD9/XrZ+IYRsv85a5nmp+8x5KF26tMbtTUlJwdu3b2UTERERERHR52KDBiIiIiIiIiItpaWlYeHChahRowYqVaqE1atX4/Tp09ILxKioKLi4uMDf3x/29vawtbWFrq6uWjo9e/aUGhS8f/8eGzduRLdu3WRxZs6ciZCQEHTq1Anu7u746aef4O3tnW3vC2PHjkXHjh1hY2OT63ZUrlwZBgYGOHnyJABg1apV6NSpE/T19WXxxo0bh5o1a8LJyQnNmzfHiBEjsHHjRlmc5ORkrFmzBt7e3qhbty4WLFiA9evX4/nz57J4ly9fRvPmzTFr1ix07NhRmr9hwwZkZGRgxYoV8PT0hIeHB8LDwxEbG4tjx47B1NRU6jXD1NQUBgYG2faiAQC3b9/GqlWrMGzYsFzLQROFQqHWW8fXHMbDyMhIWo+FhQV0dXWl30WKFAHwaV8ICAjAgAEDUKpUKQwfPhxt2rTBzJkzZWm1b98evXv3RqlSpTB58mRUrlwZCxYskMUpVKiQbNuUSiWSkpKwZMkSzJgxA35+fihTpgyWL18OIyMjrFy5Ura8jY0N7Ozs4OzsDAMDA1hYWMjC09LSYGFhIaWfef+Pi4vD06dPERQUBDc3N6lOcyufDx8+ZBue2/6jYmBggFWrVqFs2bJo2rQpJk2ahPnz5yMjIwMpKSmYOnUqVq1aBV9fXzg7OyMgIABdu3bF0qVLAQAuLi5o0KABSpYsCTc3N9jZ2SE9PT3HvAPAw4cP0ahRI/Tp0wcjRoyQhQUFBaF+/fpwcnLCN998gx9++EE6vjTt55nrDfjUyGLEiBHw9vaGs7MzBg8ejMaNG6sdo2lpabL0Mpd5Xus+cx709PQ0bvOPP/4ICwsLaXJ0dMy1nIiIiIiIiLLDBg1EREREREREWtLT00OVKlWk36VLl4alpaX0FXzJkiXx4MEDREZG5phOixYtEBMTg7t372L9+vXw8fFB0aJFpfC3b9/i6dOnqFWrlmy5WrVqqX1xD3xqLLBt2zZMnjxZ620JDAzEsmXLkJGRgZUrVyIwMFAtzoYNG1CrVi3pJei4ceMQGxsri1O8eHFZ7xI1atRARkYGbt26Jc27f/8+fH19kZycLA0ToRIdHY27d+/CzMwMpqamMDU1hbW1NZKTk3Hv3j2tt0dl1KhR6Nu3L5ydndXCrl27Jq3D1NRU6iXic5w8eVKWljaTqgFJXsXExGi1L9SoUUPtt6b9Jat79+4hLS1Ntg59fX1UrVpVbXkHBweYmJjAzc0NTZo0QefOnWXhb9++zbZHC2tra1hYWGDjxo2yoUtyUq5cOZw9exb379/XGK7t/uPl5SXrgaRGjRpITEzEo0ePcPfuXbx//x6NGjWS1deaNWtkacTGxsLU1BQmJiY4f/68bHgWTeLj49GwYUM8fvwYvr6+auGHDh1CgwYNYG9vDzMzM3Tr1g2vXr3C+/fvtSqb9PR0TJ48GZ6enrC2toapqSn279+vdozmVCd5qXttjRkzBgkJCdKUdVgeIiIiIiKivNDclJqIiIiIiIiI8qxt27Y4duwYvvnmG+jo6EBXV1fjy0k9PT0EBARgxYoVOHr0KCZNmvTZLw8BIDg4GCNGjICdnZ3Wy3Tt2hVhYWFYv349bG1t4enpKQs/c+YMunTpgokTJ8LX1xcWFhZYv349Zs2alef8Xb16FaNHj0ZcXBx69uyJEydOQEfn0zcWiYmJqFSpEtauXau2nKqHAm0dP34cJ0+eRHh4OH777Te1cHd3d+zYsUP6fe7cOXTt2jWPW/NJ5cqVERUVladlsg4r8k908uRJmJmZ4f79++jTpw9mz54tG8Lg6dOnKFasmMZl9fT08PPPP6N///5YuHAhDA0NkZqaijJlymS7vp49e2Lbtm1wdnbW+FL+S+w/iYmJAIDdu3er1ZFSqZT+X6xYMURFReH58+cYM2YMpk2bJvXgoMnDhw/RpUsXdO3aFT179sTVq1elRhUPHjxAs2bN0L9/f0yZMgXW1tY4deoUevXqhdTUVLXhXzSZMWMG5s2bh7lz58LT0xMmJiYICgqSDbUB5FwnX4NSqZSVGxERERER0V/BBg1EREREREREWvr48SMuXryIqlWrAvg0pnx8fDw8PDwAADo6OggJCcHGjRsxa9Ys1KxZU61HApXAwEB4e3vD2toajRo1kjVoMDc3R7FixRAZGQkfHx9pfmRkpLRulR07duD27dvYvXt3nrbF0tISLVq0QL9+/TQOY3H69GmUKFECY8eOleY9fPhQLV5sbKzshenZs2eho6MDd3d3KU7dunXx448/IiEhAeXKlcO8efOkISEqVqyIDRs2wMbGBubm5nnahsyEEAgODkZoaCisrKw0xjEwMICrq6v0+/Hjx5+9PiMjI1laX5OHhwciIyPh7+8vzYuMjFRrCHD27Fl0795d9rtChQq5pu/i4gIDAwNERkaiRIkSAD4NU3DhwgUEBQXJ4pYsWRKWlpZwdXVF27ZtsW3bNqlBw7179/DmzZsc19m8eXP8/PPPSEtLw4wZMzB//nycOHEi2/hGRkY4dOgQXrx4gXfv3gEA3NzcpHBt95/o6Gh8+PABRkZGAD6VjampKRwdHWFtbQ2lUonY2FjZ8ZaVnp4eXF1d4erqihEjRqBLly45NmhwdnaWenH47bffMGbMGMybNw8AcOnSJWRkZGDWrFlS456sQ0XkJjIyEi1btpQa5WRkZOD27dtq+8WFCxeyrZO81D0REREREVF+YIMGIiIiIiIiIi3p6+tj8ODBmD9/PvT09DBo0CBUr15damSQkpKCtm3bomfPntKL5ezGmS9ZsiRmz54NBwcH6YVmZiNHjkRYWBhcXFzg7e2N8PBwREVFqX2JPn36dCxYsECrL7qzGj16NNzd3dGxY0e1MDc3N8TGxmL9+vWoUqUKdu/ejW3btqnFMzQ0hL+/P2bOnIm3b99iyJAh6NChA2xtbaU4qgYGFhYWWLZsGdq1a4dmzZrBzc0NXbp0wYwZM9CyZUtMmjQJDg4OePjwIbZu3YpRo0bBwcFBq205fPgw7OzsMHDgwDyXQ0E3cuRIdOjQARUqVEDDhg2xc+dObN26FYcOHZLF27RpEypXrozatWtj7dq1OH/+PFauXJlr+iYmJujfvz9GjhwJa2trFC9eHNOnT8f79+/Rq1cvWdy4uDgkJyfj4cOH2LlzJ+rUqQMAuHjxIoYMGQJPT09Urlw523XNnj0bUVFRuHDhAiwsLGBtba1VGRQtWlQ2LIuKtvtPamoqevXqhXHjxuHBgwcICwvDoEGDoKOjAzMzM4wYMQLDhg1DRkYGateujYSEBERGRsLc3Bz+/v7YtWsXrKys4OjoiMePH2P69Om5NhYxMzOTjv+IiAhUrVoV7dq1Q506deDq6oq0tDQsWLAAzZs3R2RkJP73v/9pVRYqbm5u2Lx5M06fPg0rKyvMnj0bL168kBo0/Pnnn5gzZw4iIyOz7VklL3VPRERERESUH9iggYiIiIiIiEhLxsbGCAkJwXfffYcnT56gTp06shfGQ4YMgampKaZOnapVejm9MBwyZAgSEhIQHByMuLg4lClTBjt27JB9nQ4Arq6usi/388Ld3R2jR4/WGNaiRQsMGzYMgwYNQkpKCpo2bYrQ0FBMmDBBbf1t2rRBkyZN8Pr1azRr1gyLFy/Odp1+fn7o1KkTevbsiePHj8PY2BgnTpxASEgI2rRpg3fv3sHe3h4NGjTIU48NSUlJmDZtGvT19bVe5p+iVatWmDdvHmbOnImhQ4eiZMmSCA8PV+v9Y+LEiVi/fj0GDBgAOzs7rFu3LsfhHDKbNm0aMjIy0K1bN7x79w6VK1fG/v371Xq7UPW8UbhwYXz77beYPn06AGDYsGFwcHDA7NmzoVAoNK7j5MmTmDhxIk6dOgULC4s8loJm2u4/DRo0gJubG+rWrYuUlBR07txZti9PnjwZRYoUwY8//og//vgDlpaWqFixIr7//nsAn3rzCAoKwqNHj2BpaQkfHx/MnDlT63yWL18eY8eORc+ePREdHQ0vLy/Mnj0bP/30E8aMGSP1YpK5h43cjBs3Dn/88Qd8fX1hbGyMPn36oFWrVkhISAAArF27Fvv378e2bdvUenbJTNu6JyIiIiIiyg8KIYTI70wQERERERERFXQREREICgpCfHx8fmelwJgwYQK2b9+OqKio/M7Kf55CocC2bdvQqlWr/M5KgRMQEID4+Hhs3749v7Pyn/T27VtYWFjgz9EDYW6o/Grr0Q/T3AsFEREREREVDKpng4SEhDx9wKDepyURERERERERERERERERERFRPmODBiIiIiIiIiIiIiIiIiIiIipwOOQEERERERERERERfRUccoKIiIiIiAAOOUFERERERERERERERERERET/ImzQQERERERERERERERERERERAUOGzQQERERERERERERERERERFRgaOX3xkgIiIiIiIiIiKifzf9MVOhn4dxcomIiIiIiAD20EBEREREREREREREREREREQFEBs0EBERERERERERERERERERUYHDBg1ERERERERERERERERERERU4LBBAxERERERERERERERERERERU4bNBAREREREREREREREREREREBQ4bNBAREREREREREREREREREVGBwwYNREREREREREREREREREREVOCwQQMREREREREREREREREREREVOGzQQERERERERERERERERERERAUOGzQQERERERERERERERERERFRgcMGDURERERERERERERERERERFTgsEEDERERERERERERERERERERFThs0EBEREREREREREREREREREQFDhs0EBERERERERERERERERERUYGjl98ZICIiIiIiIiIion8nIQQA4O3bt/mcEyIiIiIiyk+qZwLVM4K22KCBiIiIiIiIiIiIvopXr14BABwdHfM5J0REREREVBC8e/cOFhYWWsdngwYiIiIiIiIiIiL6KqytrQEAsbGxefqjJX15b9++haOjIx49egRzc/P8zs5/GuuiYGF9FBysi4KF9VFwsC4KFtbH5xNC4N27dyhWrFielmODBiIiIiIiIiIiIvoqdHR0AAAWFhb8g28BYW5uzrooIFgXBQvro+BgXRQsrI+Cg3VRsLA+Ps/nNHLW+Qr5ICIiIiIiIiIiIiIiIiIiIvpL2KCBiIiIiIiIiIiIiIiIiIiIChw2aCAiIiIiIiIiIqKvQqlUIiwsDEqlMr+z8p/Huig4WBcFC+uj4GBdFCysj4KDdVGwsD7+fgohhMjvTBARERERERERERERERERERFlxh4aiIiIiIiIiIiIiIiIiIiIqMBhgwYiIiIiIiIiIiIiIiIiIiIqcNiggYiIiIiIiIiIiIiIiIiIiAocNmggIiIiIiIiIiIiIiIi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Hr1790aRIkVgbm6Ob775BtHR0bI4Dx480NjTQ3x8PABgwoQJ8Pb21piHY8eOaVxWNQHAq1ev0LlzZ9jb28PY2Bienp5Yt27dly0MIiIqUNiggYiIiIiIiIiIiIiI6D8sJSUFAKBUKrON0759e8TFxWHv3r24dOkSKlasiAYNGuD169dSHCEEAODQoUN49uwZtmzZonUeatasKfUOoVpO9fvZs2cAgOTkZFSqVAm7d+/G9evX0adPH3Tr1g3nz5/P8zYTEdE/g15+Z4CIiIiIiIiIiIiIiIjyj6pRgpmZmcbwU6dO4fz584iLi5MaPcycORPbt2/H5s2b0adPHwBAWloaAEi9PFhbW2udBwMDA9ja2gKAtJzqt4q9vT1GjBgh/R48eDD279+PjRs3omrVqlqvi4iI/jnYoIGIiIiIiIiIiIiIiOg/7MmTJwAAOzs7jeHR0dFITExEoUKFZPM/fPiAe/fuSb/fvn0LADAxMcl2XdeuXYOpqSl0dXVRrFgx+Pv7Y/To0VrlMz09HVOnTsXGjRvx5MkTpKamIiUlBcbGxlotT0RE/zxs0EBERERERERERERERPQfdvPmTRQpUiTbHhUSExNhZ2eHY8eOqYVZWlpK/3/69Cl0dHTUelbIzN3dHTt27EB6ejrOnj2LwMBAuLq6ol27drnmc8aMGZg3bx7mzp0LT09PmJiYICgoCKmpqbkuS0RE/0xs0EBERERERERERERERPQfdvjwYdSsWTPb8IoVK+L58+fQ09ODk5NTtvEuXLiA0qVLw9DQMNs4BgYGcHV1BfCpccPChQsRFRWlVYOGyMhItGzZEl27dgUAZGRk4Pbt2yhTpkyuyxIR0T+TTn5ngIiIiIiIiIiIiIiIiP5+Hz58wMqVK7F37174+vri+fPn0pSQkAAhBJ4/f45vvvkGNWrUQKtWrXDgwAE8ePAAp0+fxtixY3Hx4kWkpqbi559/xuzZs9GjR48c1ymEQHJyMpKSknDkyBHcvHkT5cqV0yq/bm5uOHjwIE6fPo2YmBj07dsXL168+BJFQUREBRR7aCAiIiIiIiIiIiIiIvoP2rBhA3r37g0AGDBgAAYMGKAWx87ODvfv38eePXswduxY9OjRAy9fvoStrS3q1q2LokWL4tq1a5gwYQJCQ0MxfPjwHNd59epVGBkZQUdHB/b29ggODkanTp20yu+4cePwxx9/wNfXF8bGxujTpw9atWqFhISEvG88ERH9IyiEECK/M0FERERERERERERERER/r4iICERERODYsWPZxlEoFLh//36OQ00QERF9LRxygoiIiIiIiIiIiIiI6D/IyMgI1tbWOcYpWrQodHV1/6YcERERybGHBiIiIiIiIiIiIiIiIiIiIipw2EMDERERERERERERERERERERFThs0EBEREREREREREREREREREQFDhs0EBERERERERERERERERERUYHDBg1ERERERERERERERERERERU4LBBAxERERERERERERERERERERU4bNBAREREREREREREREREREREBQ4bNBAREREREREREREREREREVGBwwYNREREREREREREREREREREVOD8P8WLf06b/joYAAAAAElFTkSuQmCC"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Вывод: Т.к. мы вычитали из значений с gender 0 значения с gender 1, отрицательные значения получены в случае, где количество mcc транзакций преобладают в gender 1.</p>
<p>Исходя из того, что в отрицательных значениях получили:</p>
<ol>
<li>Станции техобслуживания</li>
<li>Автозапчасти и аксессуары</li>
<li>Горючее топливо — уголь, нефть, разжиженный бензин, дрова</li>
<li>Лесо- и строительный материал</li>
</ol>
<p>А в положительных:</p>
<ol>
<li>Бакалейные магазины, супермаркеты</li>
<li>Магазины косметики</li>
<li>Магазины мужской и женской одежды</li>
</ol>
<p>Простите мой сексизм, но можно сделать вывод, что gender 0 - женщины, а gender 1 - мужчины.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="5.-ML-%D1%81%D0%B5%D0%BA%D1%86%D0%B8%D1%8F">5. ML секция<a class="anchor-link" href="#5.-ML-%D1%81%D0%B5%D0%BA%D1%86%D0%B8%D1%8F">¶</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Переименуем названия фичей, т.к. некоторые модели не принимают кирилические символы</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Разделение датасета на признаки (X) и целевую переменную (y)</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Разделение на обучающий и тестовый сеты</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noOutputs jp-mod-noInput">
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Обучим несколько моделей на датасетах с отфильтрованными фичами и без и оценим точность предсказания. В качестве мооделей выбраны:</p>
<ul>
<li>logistic regression, как быстрый инструмент, который может показать хорошие результаты на разреженной матрице</li>
<li>random forest, как представитель моделей бэггинга</li>
<li>catboot, LGBM, XGB, как классическая тройка моделей бустинга</li>
</ul>
<p>Для скаляции данных используется MinMaxScaler, т.к. размах некоторых фичей отличается на 5-6 порядков.</p>
<p>Начнем с отфильтрованных данных.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
</div>
</div>
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>accuracy</th>
<th>roc_auc</th>
</tr>
</thead>
<tbody>
<tr>
<th>RandomForest</th>
<td>0.761</td>
<td>0.835</td>
</tr>
<tr>
<th>CatBoost</th>
<td>0.791</td>
<td>0.874</td>
</tr>
<tr>
<th>LightGBM</th>
<td>0.740</td>
<td>0.822</td>
</tr>
<tr>
<th>XGBoost</th>
<td>0.774</td>
<td>0.860</td>
</tr>
<tr>
<th>LogisticRegression</th>
<td>0.722</td>
<td>0.822</td>
</tr>
<tr>
<th>Vot_CB+LR</th>
<td>0.730</td>
<td>NaN</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Повторим для данных без фильтра.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
</div>
</div>
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>accuracy</th>
<th>roc_auc</th>
</tr>
</thead>
<tbody>
<tr>
<th>RandomForest</th>
<td>0.756</td>
<td>0.832</td>
</tr>
<tr>
<th>CatBoost</th>
<td>0.792</td>
<td>0.875</td>
</tr>
<tr>
<th>LightGBM</th>
<td>0.742</td>
<td>0.823</td>
</tr>
<tr>
<th>XGBoost</th>
<td>0.776</td>
<td>0.859</td>
</tr>
<tr>
<th>LogisticRegression</th>
<td>0.722</td>
<td>0.818</td>
</tr>
<tr>
<th>Vot_CB+LR</th>
<td>0.729</td>
<td>NaN</td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Из полученных метрик делаем вывод, что стат тест привел к сохранению точности при снижении размерности в 2 раза и сокращении времени расчета на 27%.</p>
<p>Дальнейшие расчеты будут производиться на данных полученных после проведения t-теста.</p>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Проведем тюнинг самой удачной модели</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Посмотрим лучшие параметры</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>Лучшие параметры: {'iterations': 198, 'learning_rate': 0.06932899177419524, 'max_depth': 7}
Лучшее значение: 0.8712663940621267
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Обучим модель с использованием параметров, которые показали лучшие результаты</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>0:	learn: 0.6787292	total: 5.27ms	remaining: 1.04s
197:	learn: 0.3337256	total: 910ms	remaining: 0us
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Сделаем предсказание для валидационной выборки и построим кривую ROC-AUC</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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"/>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Подход, который выбран изначально удовлетворяет условиям задачи.</p>
<p>Обучим модель на данных после тюнинга на максимальном объеме данных (тренировочные + валидационные) для формирования предсказания для тестовой выборки.</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
<pre>0:	learn: 0.6753451	total: 6.1ms	remaining: 1.2s
197:	learn: 0.3397343	total: 954ms	remaining: 0us
</pre>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>Сделаем предсказания для тестовой выборки и соединим полученный данные с customer_id</p>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child jp-OutputArea-executeResult">
<div class="jp-RenderedHTMLCommon jp-RenderedHTML jp-OutputArea-output jp-OutputArea-executeResult" data-mime-type="text/html" tabindex="0">
<div>
<style scoped="">
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
<th>customer_id</th>
<th>predict</th>
</tr>
</thead>
<tbody>
<tr>
<th>0</th>
<td>6815</td>
<td>0.0</td>
</tr>
<tr>
<th>7</th>
<td>49101</td>
<td>0.0</td>
</tr>
<tr>
<th>8</th>
<td>49793</td>
<td>1.0</td>
</tr>
<tr>
<th>15</th>
<td>85327</td>
<td>0.0</td>
</tr>
<tr>
<th>18</th>
<td>114348</td>
<td>1.0</td>
</tr>
<tr>
<th>...</th>
<td>...</td>
<td>...</td>
</tr>
<tr>
<th>14992</th>
<td>99969946</td>
<td>1.0</td>
</tr>
<tr>
<th>14993</th>
<td>99977292</td>
<td>1.0</td>
</tr>
<tr>
<th>14994</th>
<td>99980396</td>
<td>0.0</td>
</tr>
<tr>
<th>14995</th>
<td>99984336</td>
<td>0.0</td>
</tr>
<tr>
<th>14996</th>
<td>99985917</td>
<td>0.0</td>
</tr>
</tbody>
</table>
<p>6600 rows × 2 columns</p>
</div>
</div>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<h3 id="%D0%9E%D0%B1%D1%89%D0%B8%D0%B9-%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82">Общий результат<a class="anchor-link" href="#%D0%9E%D0%B1%D1%89%D0%B8%D0%B9-%D1%80%D0%B5%D0%B7%D1%83%D0%BB%D1%8C%D1%82%D0%B0%D1%82">¶</a></h3>
</div>
</div>
</div>
</div>
<div class="jp-Cell jp-MarkdownCell jp-Notebook-cell">
<div class="jp-Cell-inputWrapper" tabindex="0">
<div class="jp-Collapser jp-InputCollapser jp-Cell-inputCollapser">
</div>
<div class="jp-InputArea jp-Cell-inputArea"><div class="jp-RenderedHTMLCommon jp-RenderedMarkdown jp-MarkdownOutput" data-mime-type="text/markdown">
<p>В процессе работы с данными:</p>
<ul>
<li>была снижена размерность с 34 246 730 элементов до 1 950 000 элементов</li>
<li>категорией 0 в таргете обозначены женщины, а 1 - мужчины</li>
<li>лучшие результаты по метрикам Accuracy и ROC-AUC показала модель CatBoost</li>
<li>итоговая модель делает предсказания с точностью 0.95 по метрике ROC_AUC_SCORE, что удовлетворяет условиям поставленной задачи</li>
<li>фичи наиболее влияющие на таргет, а также их распределение указаны ниже</li>
</ul>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="application/vnd.jupyter.stderr" tabindex="0">
<pre> 99%|===================| 6640/6720 [00:50&lt;00:00]        </pre>
</div>
</div>
<div class="jp-OutputArea-child">
<div class="jp-RenderedImage jp-OutputArea-output" tabindex="0">
<img alt="No description has been provided for this image" class="" src="data:image/png;base64,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2JEjRwgICCgz4AcIDQ2ttrJWrFhBWloaY8eO5cEHH6SgoICvv/66Uvu4/fbbATh69Gi5eT755BMURWH58uVO62w2GxEREQ6td6tXr+bee++lUaNGuLm54evry2233VbhPruxsbFER0c7pScmJqIoCq+88opDuqqqfPLJJ3Tu3Bl3d3c8PT25+eabnbpSlcdisfDDDz/Qt29fpxb9svphX5g2a9YsmjdvjqurK23btmXlypUA7Nu3jzvuuANvb28CAgKYPHkyZrO5zOM8fvw4Q4YMwcfHB29vb4YNG8bx48cd8tpsNl5//XV69+5NaGgoBoOBqKgoHn/8cTIyMso8rqVLlxIbG4uvry/u7u40b96cyZMnYzKZmD9/vv2O07hx4+zdvirS+puYmMgDDzxASEgILi4uNG7cmOeff57CwkKHfK+88gqKopCQkMDzzz9PREQELi4utG/fnp9++umy5cD5fvS//vorr776Kg0bNsTNzY1u3bqxbds2ANavX89NN92Eh4cHYWFhvPbaa2Xu64cffqBnz554eHjg6elJz549WbZsWZl558yZQ4sWLXBxcaFJkya8//775XY9ycnJYdq0aTRp0gQXFxeCgoK47777nN7Dyqroeb7UuBhFUXjwwQeBkr/bmJgYoKRxovQ9L/2sXfj5+vLLL2nXrh2urq5ERUXxyiuvYLFYHPZd0c9pRf7WFEXh9ttvZ9WqVeTn51fyTAlRd0lLvxB1WOPGjUlISOC7777jrrvuqtA2Vqu13D77xcXF5W732WefERMTQ69evVAUhY4dOzJv3jzGjx9f4foeOXIEgMDAwHLzjBw5kqeffprPP/+cwYMHO6z79ddfSUpKsncbgpKLfGZmJmPGjCEiIoKkpCTmzp3Lrbfeyu+//37JLkhV8cADD/Dll18yfPhwxo0bR3FxMYsXL6Zfv3589913TnW+2K5du8jPz6dr166VKvfjjz8mKyuL8ePH4+rqyocffsiwYcP49ttvmTBhAvfddx9Dhw5l9erVzJw5k+DgYP71r3857KOgoIDY2Fi6devGG2+8wZEjR5g1axbbtm1jz5499h+JJpOJ//73v9x9990MGTIEDw8PduzYwWeffcamTZucume98MIL/Oc//6FVq1Y8/fTThIWFcezYMZYuXcqrr75K7969ef755/nPf/7DI488Yn9PQkJCLnnM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"/>
</div>
</div>
</div>
</div>
</div><div class="jp-Cell jp-CodeCell jp-Notebook-cell jp-mod-noInput">
<div class="jp-Cell-outputWrapper">
<div class="jp-Collapser jp-OutputCollapser jp-Cell-outputCollapser">
</div>
<div class="jp-OutputArea jp-Cell-outputArea">
<div class="jp-OutputArea-child">
<div class="jp-RenderedText jp-OutputArea-output" data-mime-type="text/plain" tabindex="0">
</div>
</div>
</div>
</div>
</div>
</main>
</body>
</html>
