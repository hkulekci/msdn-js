---
title: stackTraceLimit Property (Error) (JavaScript)
---

### Introduction 

 Gets or sets the stack trace limit, which is equivalent to the number of error frames to display. The default limit is 10.

### Syntax 

```
Error .stackTraceLimit
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You can set the <b>stackTraceLimit</b> property to any positive value between 0 and <span sdata="langKeyword" value="Infinity"><span class="keyword">Infinity</span></span>. If the
    <b>stackTraceLimit</b> property is set to 0 at the time an error is thrown, no stack trace is shown. If the property is set to a negative value or a non-numeric value, the value is converted to
    0. If the stackTraceLimit is set to <span sdata="langKeyword" value="Infinity"><span class="keyword">Infinity</span></span>, the entire stack is shown. Otherwise, <span sdata="langKeyword" value=
    "ToUint32"><span class="keyword">ToUint32</span></span> is used to convert the value.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to set and then get the stack trace limit.
</p>

```
try { var err = new Error("my error"); Error.stackTraceLimit = 7; throw err; } catch(e) { document.write ("Error stack trace limit: ") document.write (Error.stackTraceLimit); }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in Internet Explorer 10 and in Windows Store apps.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="0b27d6ec-3997-4e91-a6c0-5afbaf494db7.htm">Error Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ea727f1e-2041-4400-965c-67e6d47a1ff0.htm">description Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8cab0392-e0db-4714-827c-47ab04e8b4f2.htm">message Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="94df2d6b-f1a1-4931-a956-0a930cb87f76.htm">name Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1dc21fdd-853c-4664-bf1c-24eb1f6f2daf.htm">stack Property (Error) (JavaScript)</a></span>
  </div>
</div>

