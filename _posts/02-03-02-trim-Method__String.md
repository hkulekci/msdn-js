---
title: trim Method (String) (JavaScript)
---

### Introduction 

 Removes the leading and trailing white space and line terminator characters from a string.

### Syntax 

```
stringObj .trim()
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal. This string is not modified by the <b>trim</b> method.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The original string with leading and trailing white space and line terminator characters removed.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The characters that are removed include space, tab, form feed, carriage return, and line feed. See <span sdata="link">Special Characters (Windows Scripting - JScript)</span> for a comprehensive
    list of white space and line terminator characters.
  </p>
  <p xmlns:util="util">
    For an example that shows how to implement your own trim method, see <span sdata="link">Prototypes and Prototype Inheritance</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>trim</b> method.
</p>

```
var message = " abc def \r\n "; document.write("[" + message.trim() + "]"); document.write("&lt;br/&gt;"); document.write("length: " + message.trim().length); // Output: // [abc def] // length: 7
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Internet Explorer 9 standards and Internet Explorer 10 standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Special Characters (Windows Scripting - JScript)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

