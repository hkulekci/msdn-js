---
title: @if Statement (JavaScript)
---

### Introduction 

 Conditionally executes a group of statements, depending on the value of an expression. Caution Conditional compilation is supported in Internet Explorer only, not in Windows Store apps.

### Syntax 

```
@if ( condition1 ) text1 [@elif ( condition2 ) text2 ] [@else text3 ] @end
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">condition1, condition2</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. An expression that can be coerced into a Boolean expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">text1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Text to be parsed if <span class="parameter" sdata="paramReference">condition1</span> is <b>true</b>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">text2</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Text to be parsed if <span class="parameter" sdata="paramReference">condition1</span> is <b>false</b> and <span class="parameter" sdata="paramReference">condition2</span> is
        <b>true</b>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">text3</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Text to be parsed if both <span class="parameter" sdata="paramReference">condition1</span> and <span class="parameter" sdata="paramReference">condition2</span> are <b>false</b>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    When you write an <span sdata="langKeyword" value="@if"><span class="keyword">@if</span></span> statement, you do not have to place each clause on a separate line. You can use multiple
    <b>@elif</b> clauses. However, all <b>@elif</b> clauses must come before an <b>@else</b> clause.
  </p>
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="@if"><span class="keyword">@if</span></span> statement is typically used to determine which text among several options should be used for text output.
  </p>
  <p xmlns:util="util">
    It is not common to use conditional compilation variables in scripts written for ASP or ASP.NET pages or command-line programs. This is because the capabilities of the compilers can be determined
    by using other methods.
  </p>
  <p xmlns:util="util">
    When you write a script for a Web page, always add conditional compilation code in comments. This enables hosts that do not support conditional compilation to ignore it.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>@if...@elif&hellip;@else...@end</b> statement.
</p>

```
/*@cc_on @*/ /*@ document.write("JavaScript version: " + @_jscript_version + "."); document.write("&lt;br /&gt;"); @if (@_win32) document.write("Running on a 32-bit version of Windows."); @elif
(@_win16) document.write("Running on a 16-bit version of Windows."); @else document.write("Running on a different operating system."); @end @*/
```

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
    <span sdata="link" xmlns:util="util"><a href="36f15926-3e69-422d-82a2-d186dc088203.htm">@set Statement (JavaScript)</a></span>
  </div>
</div>

