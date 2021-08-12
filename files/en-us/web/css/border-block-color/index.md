---
title: border-block-color
slug: Web/CSS/border-block-color
tags:
  - CSS
  - CSS Logical Property
  - CSS Property
  - Experimental
  - Reference
  - 'recipe:css-property'
browser-compat: css.properties.border-block-color
---
<div>{{CSSRef}}</div>

<p>The <strong><code>border-block-color</code></strong> <a href="/en-US/docs/Web/CSS">CSS</a> property defines the color of the logical block borders of an element, which maps to a physical border color depending on the element's writing mode, directionality, and text orientation. It corresponds to the {{cssxref("border-top-color")}} and {{cssxref("border-bottom-color")}}, or {{cssxref("border-right-color")}} and {{cssxref("border-left-color")}} property depending on the values defined for {{cssxref("writing-mode")}}, {{cssxref("direction")}}, and {{cssxref("text-orientation")}}.</p>

<div>{{EmbedInteractiveExample("pages/css/border-block-color.html")}}</div>

<p>The border color in the other dimension can be set with {{cssxref("border-inline-color")}} which sets {{cssxref("border-inline-start-color")}}, and {{cssxref("border-inline-end-color")}}.</p>

<h2 id="Syntax">Syntax</h2>

<pre class="brush:css no-line-numbers">border-block-color: yellow;
border-block-color: #F5F6F7;

/* Global values */
border-block-color: inherit;
border-block-color: initial;
border-block-color: revert;
border-block-color: unset;</pre>

<h3 id="Values">Values</h3>

<dl>
 <dt><code>&lt;'color'&gt;</code></dt>
 <dd>The color of the border. See {{cssxref("color")}}.</dd>
</dl>

<h2 id="Formal_definition">Formal definition</h2>

<p>{{CSSInfo}}</p>

<h2 id="Formal_syntax">Formal syntax</h2>

{{csssyntax}}

<h2 id="Examples">Examples</h2>

<h3 id="Border_with_vertical_text">Border with vertical text</h3>

<h4 id="HTML">HTML</h4>

<pre class="brush: html">&lt;div&gt;
  &lt;p class="exampleText"&gt;Example text&lt;/p&gt;
&lt;/div&gt;
</pre>

<h4 id="CSS">CSS</h4>

<pre class="brush: css">div {
  background-color: yellow;
  width: 120px;
  height: 120px;
}

.exampleText {
  writing-mode: vertical-lr;
  border: 10px solid blue;
  border-block-color: red;
}</pre>

<h4 id="Results">Results</h4>

<p>{{EmbedLiveSample("Border_with_vertical_text", 140, 140)}}</p>

<h2 id="Specifications">Specifications</h2>

{{Specifications}}

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{Compat}}</p>

<h2 id="See_also">See also</h2>

<ul>
 <li>This property maps to the physical border properties: {{cssxref("border-top-color")}}, {{cssxref("border-right-color")}}, {{cssxref("border-bottom-color")}}, or {{cssxref("border-left-color")}}.</li>
 <li>{{cssxref("writing-mode")}}, {{cssxref("direction")}}, {{cssxref("text-orientation")}}+ bug 1297097</li>
</ul>