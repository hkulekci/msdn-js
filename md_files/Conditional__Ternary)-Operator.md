---
title: Conditional (Ternary) Operator (?:) (JavaScript)
isChild: false
---

## Conditional (Ternary) Operator (?:) (JavaScript) {conditional_ternary_operator_--_javascript_title}

### Introduction 

 Returns one of two expressions depending on a condition.

### Syntax 

```
test ? expression1 : expression2
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">test</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any Boolean expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        An expression returned if <span class="parameter" sdata="paramReference">test</span> is <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>. May be a comma
        expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression2</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        An expression returned if <span class="parameter" sdata="paramReference">test</span> is <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>. More than one
        expression may be a linked by a comma expression.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="?:"><span class="keyword">?:</span></span> operator can be used as a shortcut for an <span sdata="langKeyword" value="if...else"><span class=
    "keyword">if...else</span></span> statement. It is typically used as part of a larger expression where an <span sdata="langKeyword" value="if...else"><span class="keyword">if...else</span></span>
    statement would be awkward. For example:
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          JavaScript&nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 var now = new Date(); var greeting = "Good" + ((now.getHours() &gt; 17) <span class="label">?</span> " evening." <span class="label">:</span> " day."); 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    The example creates a string containing "Good evening." if it is after 6pm. The equivalent code using an <span sdata="langKeyword" value="if...else"><span class="keyword">if...else</span></span>
    statement would look as follows:
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          JavaScript&nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 var now = new Date(); var greeting = "Good"; if (now.getHours() &gt; 17)    greeting += " evening."; else    greeting += " day."; 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="dfbe86e8-9c1e-4ef5-bb9c-7d1db7ce2506.htm">if...else Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

