---
title: stack Property (Error) (JavaScript)
isChild: false
---

## stack Property (Error) (JavaScript) {stack_property_error_javascript_title}

### Introduction 

 Gets or sets the error stack as a string that contains the stack trace frames.

### Syntax 

```
object .stack
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>stack</b> property is set to <span sdata="langKeyword" value="undefined"><span class="keyword">undefined</span></span> when the error is constructed, and gets the trace information when
    the error is raised. If an error is raised multiple times, the <b>stack</b> property is updated each time the error is raised.
  </p>
  <p xmlns:util="util">
    Stack frames are displayed in the following format: <span class="input">at FunctionName (&lt;Fully-qualified name/URL&gt;:&lt;line number&gt;:&lt;column number&gt;)</span>
  </p>
  <p xmlns:util="util">
    If you create your own Error object and set the stack trace to a value, the value won't be overwritten when the error is thrown.
  </p>
  <p xmlns:util="util">
    The <b>stack</b> property does not show inline functions in its frames. It shows only the physical stack.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to get the stack when you're catching an error.
</p>

```
try { var x = y.name; } catch(e) { document.write ("Error stack: ") document.write (e.stack); }
```

<p xmlns:util="util">
  The following example shows how to set and then get the stack.
</p>

```
try { var err = Error("my error"); err.stack = "my stack trace"; throw err; } catch(e) { document.write ("Error stack: ") document.write (e.stack); }
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
    <span sdata="link" xmlns:util="util"><a href="127ef8e8-892e-4263-9ebc-03364af01212.htm">stackTraceLimit Property (Error) (JavaScript)</a></span>
  </div>
</div>

