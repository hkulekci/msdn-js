---
title: description Property (Error) (JavaScript)
isChild: false
---

## description Property (Error) (JavaScript) {description_property_error_javascript_title}

### Introduction 

 Returns or sets the descriptive string associated with a specific error.

### Syntax 

```
object .description [= stringExpression ]
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">object</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any instance of an <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringExpression</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A string expression containing a description of the error.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>description</b> property contains the error message string associated with a specific error. Use the value contained in this property to alert a user to an error.
  </p>
  <p xmlns:util="util">
    The <b>description</b> and <b>message</b> properties provide the same functionality; the <b>description</b> property provides backward compatibility; the <b>message</b> property complies with the
    ECMA standard.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>description</b> property.
</p>

```
try { // Cause an error: x = y } catch(e) { // Prints "[object Error]": document.write(e) document.write (" "); // Prints 5009: document.write((e.number &amp; 0xFFFF)) document.write (" "); // Prints
"'y' is undefined": document.write(e.description); document.write (" "); // Prints "'y' is undefined": document.write(e.message) }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
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
    <span sdata="link" xmlns:util="util"><a href="8697e20b-a2b0-4e26-85c0-ab07ddfe8281.htm">number Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8cab0392-e0db-4714-827c-47ab04e8b4f2.htm">message Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="94df2d6b-f1a1-4931-a956-0a930cb87f76.htm">name Property (Error) (JavaScript)</a></span>
  </div>
</div>

