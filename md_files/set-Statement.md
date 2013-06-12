---
title: @set Statement (JavaScript)
isChild: false
---

## @set Statement (JavaScript) {@set_statement_javascript_title}

### Introduction 

 Creates variables used with conditional compilation statements. Caution Conditional compilation is supported in Internet Explorer only, not in Windows Store apps.

### Syntax 

```
@set @varname = term
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">varname</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Valid JavaScript variable name. Must be preceded by an "@" character at all times.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">term</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Zero or more unary operators followed by a constant, conditional compilation variable, or parenthesized expression.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Numeric and Boolean variables are supported for conditional compilation. Strings are not. Variables created using <span sdata="langKeyword" value="@set"><span class="keyword">@set</span></span>
    are generally used in conditional compilation statements, but can be used anywhere in JavaScript code.
  </p>
  <p xmlns:util="util">
    Examples of variable declarations look like this:
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
 <span class="label">@set</span> @myvar1 = 12  <span class="label">@set</span> @myvar2 = (@myvar1 * 20)  <span class="label">@set</span> @myvar3 = @_jscript_version 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    The following operators are supported in parenthesized expressions:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        <span class="code">! ~</span>
      </p>
    </li>
    <li>
      <p>
        <span class="code">* / %</span>
      </p>
    </li>
    <li>
      <p>
        <span class="code">+ -</span>
      </p>
    </li>
    <li>
      <p>
        <span class="code">&lt;&lt; &gt;&gt; &gt;&gt;&gt;</span>
      </p>
    </li>
    <li>
      <p>
        <span class="code">&lt; &lt;= &gt; &gt;=</span>
      </p>
    </li>
    <li>
      <p>
        <span class="code">== != === !==</span>
      </p>
    </li>
    <li>
      <p>
        <span class="code">&amp; ^ |</span>
      </p>
    </li>
    <li>
      <p>
        <span class="code">&amp;&amp; | |</span>
      </p>
    </li>
  </ul>
  <p xmlns:util="util">
    If a variable is used before it has been defined, its value is <b>NaN</b>. <b>NaN</b> can be checked for using the <span sdata="langKeyword" value="@if"><span class="keyword">@if</span></span>
    statement:
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
 @if (@newVar != @newVar)    ... 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    This works because <b>NaN</b> is the only value not equal to itself.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in all versions of Internet Explorer, but not in Windows Store apps.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Conditional Compilation</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Conditional Compilation Variables</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="fdeda7ee-b9f4-4e52-8aa2-21c90c02a332.htm">@cc_on Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ff11b29d-c06a-4276-b11d-db73e2da98ac.htm">@if Statement (JavaScript)</a></span>
  </div>
</div>

