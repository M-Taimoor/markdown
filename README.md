# markdown
<!DOCTYPE html>
<html>
<head>
<title>mark_down_cheatsheet.md</title>
<meta http-equiv="Content-type" content="text/html;charset=UTF-8">

<style>
/* https://github.com/microsoft/vscode/blob/master/extensions/markdown-language-features/media/markdown.css */
/*---------------------------------------------------------------------------------------------
 *  Copyright (c) Microsoft Corporation. All rights reserved.
 *  Licensed under the MIT License. See License.txt in the project root for license information.
 *--------------------------------------------------------------------------------------------*/

body {
	font-family: var(--vscode-markdown-font-family, -apple-system, BlinkMacSystemFont, "Segoe WPC", "Segoe UI", "Ubuntu", "Droid Sans", sans-serif);
	font-size: var(--vscode-markdown-font-size, 14px);
	padding: 0 26px;
	line-height: var(--vscode-markdown-line-height, 22px);
	word-wrap: break-word;
}

#code-csp-warning {
	position: fixed;
	top: 0;
	right: 0;
	color: white;
	margin: 16px;
	text-align: center;
	font-size: 12px;
	font-family: sans-serif;
	background-color:#444444;
	cursor: pointer;
	padding: 6px;
	box-shadow: 1px 1px 1px rgba(0,0,0,.25);
}

#code-csp-warning:hover {
	text-decoration: none;
	background-color:#007acc;
	box-shadow: 2px 2px 2px rgba(0,0,0,.25);
}

body.scrollBeyondLastLine {
	margin-bottom: calc(100vh - 22px);
}

body.showEditorSelection .code-line {
	position: relative;
}

body.showEditorSelection .code-active-line:before,
body.showEditorSelection .code-line:hover:before {
	content: "";
	display: block;
	position: absolute;
	top: 0;
	left: -12px;
	height: 100%;
}

body.showEditorSelection li.code-active-line:before,
body.showEditorSelection li.code-line:hover:before {
	left: -30px;
}

.vscode-light.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(0, 0, 0, 0.15);
}

.vscode-light.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(0, 0, 0, 0.40);
}

.vscode-light.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

.vscode-dark.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(255, 255, 255, 0.4);
}

.vscode-dark.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(255, 255, 255, 0.60);
}

.vscode-dark.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

.vscode-high-contrast.showEditorSelection .code-active-line:before {
	border-left: 3px solid rgba(255, 160, 0, 0.7);
}

.vscode-high-contrast.showEditorSelection .code-line:hover:before {
	border-left: 3px solid rgba(255, 160, 0, 1);
}

.vscode-high-contrast.showEditorSelection .code-line .code-line:hover:before {
	border-left: none;
}

img {
	max-width: 100%;
	max-height: 100%;
}

a {
	text-decoration: none;
}

a:hover {
	text-decoration: underline;
}

a:focus,
input:focus,
select:focus,
textarea:focus {
	outline: 1px solid -webkit-focus-ring-color;
	outline-offset: -1px;
}

hr {
	border: 0;
	height: 2px;
	border-bottom: 2px solid;
}

h1 {
	padding-bottom: 0.3em;
	line-height: 1.2;
	border-bottom-width: 1px;
	border-bottom-style: solid;
}

h1, h2, h3 {
	font-weight: normal;
}

table {
	border-collapse: collapse;
}

table > thead > tr > th {
	text-align: left;
	border-bottom: 1px solid;
}

table > thead > tr > th,
table > thead > tr > td,
table > tbody > tr > th,
table > tbody > tr > td {
	padding: 5px 10px;
}

table > tbody > tr + tr > td {
	border-top: 1px solid;
}

blockquote {
	margin: 0 7px 0 5px;
	padding: 0 16px 0 10px;
	border-left-width: 5px;
	border-left-style: solid;
}

code {
	font-family: Menlo, Monaco, Consolas, "Droid Sans Mono", "Courier New", monospace, "Droid Sans Fallback";
	font-size: 1em;
	line-height: 1.357em;
}

body.wordWrap pre {
	white-space: pre-wrap;
}

pre:not(.hljs),
pre.hljs code > div {
	padding: 16px;
	border-radius: 3px;
	overflow: auto;
}

pre code {
	color: var(--vscode-editor-foreground);
	tab-size: 4;
}

/** Theming */

.vscode-light pre {
	background-color: rgba(220, 220, 220, 0.4);
}

.vscode-dark pre {
	background-color: rgba(10, 10, 10, 0.4);
}

.vscode-high-contrast pre {
	background-color: rgb(0, 0, 0);
}

.vscode-high-contrast h1 {
	border-color: rgb(0, 0, 0);
}

.vscode-light table > thead > tr > th {
	border-color: rgba(0, 0, 0, 0.69);
}

.vscode-dark table > thead > tr > th {
	border-color: rgba(255, 255, 255, 0.69);
}

.vscode-light h1,
.vscode-light hr,
.vscode-light table > tbody > tr + tr > td {
	border-color: rgba(0, 0, 0, 0.18);
}

.vscode-dark h1,
.vscode-dark hr,
.vscode-dark table > tbody > tr + tr > td {
	border-color: rgba(255, 255, 255, 0.18);
}

</style>

<style>
/* Tomorrow Theme */
/* http://jmblog.github.com/color-themes-for-google-code-highlightjs */
/* Original theme - https://github.com/chriskempson/tomorrow-theme */

/* Tomorrow Comment */
.hljs-comment,
.hljs-quote {
	color: #8e908c;
}

/* Tomorrow Red */
.hljs-variable,
.hljs-template-variable,
.hljs-tag,
.hljs-name,
.hljs-selector-id,
.hljs-selector-class,
.hljs-regexp,
.hljs-deletion {
	color: #c82829;
}

/* Tomorrow Orange */
.hljs-number,
.hljs-built_in,
.hljs-builtin-name,
.hljs-literal,
.hljs-type,
.hljs-params,
.hljs-meta,
.hljs-link {
	color: #f5871f;
}

/* Tomorrow Yellow */
.hljs-attribute {
	color: #eab700;
}

/* Tomorrow Green */
.hljs-string,
.hljs-symbol,
.hljs-bullet,
.hljs-addition {
	color: #718c00;
}

/* Tomorrow Blue */
.hljs-title,
.hljs-section {
	color: #4271ae;
}

/* Tomorrow Purple */
.hljs-keyword,
.hljs-selector-tag {
	color: #8959a8;
}

.hljs {
	display: block;
	overflow-x: auto;
	color: #4d4d4c;
	padding: 0.5em;
}

.hljs-emphasis {
	font-style: italic;
}

.hljs-strong {
	font-weight: bold;
}
</style>

<style>
/*
 * Markdown PDF CSS
 */

 body {
	font-family: -apple-system, BlinkMacSystemFont, "Segoe WPC", "Segoe UI", "Ubuntu", "Droid Sans", sans-serif, "Meiryo";
	padding: 0 12px;
}

pre {
	background-color: #f8f8f8;
	border: 1px solid #cccccc;
	border-radius: 3px;
	overflow-x: auto;
	white-space: pre-wrap;
	overflow-wrap: break-word;
}

pre:not(.hljs) {
	padding: 23px;
	line-height: 19px;
}

blockquote {
	background: rgba(127, 127, 127, 0.1);
	border-color: rgba(0, 122, 204, 0.5);
}

.emoji {
	height: 1.4em;
}

code {
	font-size: 14px;
	line-height: 19px;
}

/* for inline code */
:not(pre):not(.hljs) > code {
	color: #C9AE75; /* Change the old color so it seems less like an error */
	font-size: inherit;
}

/* Page Break : use <div class="page"/> to insert page break
-------------------------------------------------------- */
.page {
	page-break-after: always;
}

</style>

<script src="https://unpkg.com/mermaid/dist/mermaid.min.js"></script>
</head>
<body>
  <script>
    mermaid.initialize({
      startOnLoad: true,
      theme: document.body.classList.contains('vscode-dark') || document.body.classList.contains('vscode-high-contrast')
          ? 'dark'
          : 'default'
    });
  </script>
<h1 id="1--headings">1- Headings</h1>
<p>How to use heading in markdown files?</p>
<h1 id="heading-1">Heading 1</h1>
<h2 id="heading-2">Heading 2</h2>
<h3 id="heading-3">Heading 3</h3>
<h4 id="heading-4">Heading 4</h4>
<h5 id="heading-5">heading 5</h5>
<h6 id="heading-6">heading 6</h6>
<h1 id="2--block-of-words">2- Block of words</h1>
<p>This is the normal text of markdonw</p>
<blockquote>
<p>This is the special block in markdown</p>
<p>This is the special line</p>
</blockquote>
<h1 id="3--line-break">3- Line break</h1>
<p>This is a 40 days long course of Data scince with python AKA python_ka_chila_with_Dr ammar.</p>
<p>This is the second line.<br>
This is a 40 days long course of Data scince with python AKA python_ka_chila_with_Dr ammar.</p>
<p>This is the second line.</p>
<h1 id="4--combine-two-things">4- combine two things</h1>
<p>Block of word and headings</p>
<blockquote>
<h2 id="heading-2">Heading 2</h2>
</blockquote>
<h1 id="5-face-of-text">5-Face of text</h1>
<p><strong>Bold</strong></p>
<p><em>Italic</em></p>
<p><em><strong>Bold &amp; italic</strong></em></p>
<p><em>italic</em></p>
<p><em><strong>Blod and italic</strong></em>
or you can use symbols</p>
<p>_(under score)</p>
<p><strong>BOLD</strong></p>
<p><em>italic</em></p>
<p><em><strong>bold and italic</strong></em></p>
<h1 id="6--bullet-points-or-lists">6- Bullet points or lists</h1>
<ul>
<li>Day 1</li>
<li>Day 2</li>
<li>Day 3</li>
<li>Day 4</li>
<li>Day 5
<ul>
<li>Day 5a
<ul>
<li>Sublist/heading</li>
</ul>
</li>
<li>Day 5b</li>
</ul>
</li>
<li>Day 6</li>
<li>Day 7</li>
</ul>
<blockquote>
<p><strong>Using *  or +</strong></p>
</blockquote>
<ul>
<li>one
<ul>
<li>two</li>
</ul>
</li>
</ul>
<blockquote>
<p>Number of list</p>
</blockquote>
<ol>
<li>Day 1</li>
<li>Day 2</li>
<li>Day 3</li>
<li>Day 4</li>
<li>Day 5
<ol>
<li>Day 5a
<ol>
<li>Sub heading / sublist</li>
</ol>
</li>
<li>Day 5b</li>
</ol>
</li>
</ol>
<h1 id="7--line-break-or-page-break">7- Line break or page break</h1>
<p>This is a line 1.</p>
<hr>
<hr>
<hr>
<p>This is a line 2</p>
<h1 id="8-links-and-hyperlinks">8 Links and Hyperlinks</h1>
<p>link of google</p>
<p><a href="https://www.google.com">https://www.google.com</a></p>
<p><a href="https://www.google.com">Link text</a></p>
<p>click <a href="https://www.google.com">here</a></p>
<h1 id="9-images-and-figure-with-link">9 Images and figure with link</h1>
<p>Here is the image to show you for testing and learning step.
Link of a picute
<a href="Snap.jpg">Snap</a></p>
<p>Use use ! to saw the image
<a href="Snap.jpg">Image description</a></p>
<blockquote>
<p>Task : How to comment a markdown line? and its sortcut?</p>
</blockquote>
<p>Oneline picture links</p>
<p><img src="https://www.google.com/url?sa=i&amp;url=https://codanics.com/&amp;psig=AOvVaw0N6l8yuK7cWBrhaOJTdRMJ&amp;ust=1698934006542000&amp;source=images&amp;cd=vfe&amp;opi=89978449&amp;ved=0CBMQjRxqFwoTCNiDkMP8ooIDFQAAAAAdAAAAABAE" alt="Codanics"></p>
<h1 id="10--adding-code-or-code-block">10- Adding code or code block</h1>
<p>To print a string  use <code>print(&quot;Taimoor&quot;)</code></p>
<p><code>print(&quot;Hello Baba g Dr ammar&quot;)</code></p>
<pre class="hljs"><code><div>x = 5+6
y  = 3-2
z = x+y
print(z)
</div></code></pre>
<blockquote>
<p>This code will how you color according to Python language syntax</p>
</blockquote>
<pre class="hljs"><code><div>x = <span class="hljs-number">5</span>+<span class="hljs-number">6</span>
y  = <span class="hljs-number">3</span><span class="hljs-number">-2</span>
z = x+y
print(z)
</div></code></pre>
<blockquote>
<p>This code will how you color according to R language syntax</p>
</blockquote>
<pre class="hljs"><code><div>x = <span class="hljs-number">5</span>+<span class="hljs-number">6</span>
y  = <span class="hljs-number">3</span>-<span class="hljs-number">2</span>
z = x+y
print(z)
</div></code></pre>
<h1 id="11--adding-tables">11- Adding Tables</h1>
<table>
<thead>
<tr>
<th style="text-align:center">species</th>
<th style="text-align:center">petal_length</th>
<th style="text-align:center">sepal_length</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:center">virginica</td>
<td style="text-align:center">18.2</td>
<td style="text-align:center">19.2</td>
</tr>
<tr>
<td style="text-align:center">setosa</td>
<td style="text-align:center">15.1</td>
<td style="text-align:center">17.2</td>
</tr>
<tr>
<td style="text-align:center">versicolor</td>
<td style="text-align:center">12.2</td>
<td style="text-align:center">12.2</td>
</tr>
<tr>
<td style="text-align:center">virginica</td>
<td style="text-align:center">18.2</td>
<td style="text-align:center">19.2</td>
</tr>
<tr>
<td style="text-align:center">setosa</td>
<td style="text-align:center">15.1</td>
<td style="text-align:center">17.2</td>
</tr>
<tr>
<td style="text-align:center">versicolor</td>
<td style="text-align:center">12.2</td>
<td style="text-align:center">12.2</td>
</tr>
</tbody>
</table>
<h1 id="12--content">12- content</h1>
<p><a href="#1--headings">1-Headings</a><br>
<a href="#2--block-of-words">2- block of word</a><br>
<a href="#3--line-break">3-Line break</a><br>
<a href="#4--combine-two-things">4-combine two things</a><br>
<a href="#5-face-of-text">5- face of text</a><br>
<a href="#6--bullet-points-or-lists">6-Bullet point or list</a><br>
<a href="#7--line-break-or-page-break">7- Line break or page break</a><br>
<a href="#8-links-and-hyperlinks">8- Links and hyperlinks</a><br>
<a href="#9-images-and-figure-with-link">9-Images and figure with link</a><br>
<a href="#10--adding-code-or-code-block">10-Adding code or code block</a><br>
<a href="#11--adding-tables">11-Adding tables</a></p>
<h1 id="13-install-extenstions">13 Install extenstions</h1>
<p><strong>sample text</strong></p>
<p><strong>bold</strong></p>
<p><em>Italic</em></p>
<p><em><strong>bold and italic</strong></em></p>
<p><a href="www.google.com">link</a></p>
<p><img src="Snap.jpg" alt="Snap.jpgimage"></p>
<blockquote>
<p>this is a citation</p>
</blockquote>
<table>
<thead>
<tr>
<th>Column A</th>
<th>Column B</th>
<th>Column C</th>
</tr>
</thead>
<tbody>
<tr>
<td>A1</td>
<td>B1</td>
<td>C1</td>
</tr>
<tr>
<td>A2</td>
<td>B2</td>
<td>C2</td>
</tr>
<tr>
<td>A3</td>
<td>B3</td>
<td>C3</td>
</tr>
</tbody>
</table>
<table>
<thead>
<tr>
<th>Column A</th>
<th>Column B</th>
<th>Column C</th>
</tr>
</thead>
<tbody>
<tr>
<td>A1</td>
<td>B1</td>
<td>C1</td>
</tr>
<tr>
<td>A2</td>
<td>B2</td>
<td>C2</td>
</tr>
<tr>
<td>A3</td>
<td>B3</td>
<td>C3</td>
</tr>
</tbody>
</table>

</body>
</html>

