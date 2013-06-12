---
title: @cc_on Statement (JavaScript)
isChild: false
---

## @cc_on Statement (JavaScript) {@cc_on_statement_javascript_title}

### Introduction 

 Activates conditional compilation support within comments in a script. Caution Conditional compilation is supported in Internet Explorer only, not in Windows Store apps.

### Syntax 

```
@cc_on
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="@cc_on"><span class="keyword">@cc_on</span></span> statement activates conditional compilation within comments in a script.
  </p>
  <p xmlns:util="util">
    It is not common to use conditional compilation variables in scripts written for ASP or ASP.NET pages or command-line programs because the capabilities of the compilers can be determined by using
    other methods.
  </p>
  <p xmlns:util="util">
    When you write a script for a Web page, always put conditional compilation code in comments. This enables hosts that do not support conditional compilation to ignore it.
  </p>
  <p xmlns:util="util">
    It is strongly recommended that you use the <span sdata="langKeyword" value="@cc_on"><span class="keyword">@cc_on</span></span> statement in a comment, so that browsers that do not support
    conditional compilation will accept your script as valid syntax:
  </p>
  <p xmlns:util="util">
    An <span sdata="langKeyword" value="@if"><span class="keyword">@if</span></span> or <span sdata="langKeyword" value="@set"><span class="keyword">@set</span></span> statement outside of a comment
    also activates conditional compilation.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="@cc_on"><span class="keyword">@cc_on</span></span> statement.
</p>

```
/*@cc_on @*/ /*@ document.write("JavaScript version: " + @_jscript_version + "."); document.write("&lt;br /&gt;"); @if (@_win32) document.write("Running on the 32-bit version of Windows."); @elif
(@_win16) document.write("Running on the 16-bit version of Windows."); @else document.write("Running on a different operating system."); @end @*/
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
    <span sdata="link" xmlns:util="util"><a href="ff11b29d-c06a-4276-b11d-db73e2da98ac.htm">@if Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="36f15926-3e69-422d-82a2-d186dc088203.htm">@set Statement (JavaScript)</a></span>
  </div>
</div>

