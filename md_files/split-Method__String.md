---
title: split Method (String) (JavaScript)
isChild: false
---

## split Method (String) (JavaScript) {split_method_string_javascript_title}

### Introduction 

 Split a string into substrings using the specified separator and return them as an array.

### Syntax 

```
stringObj .split([separator[, limit ]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal to be split. This object is not modified by the <b>split</b> method.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">separator</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A string or a <b>Regular Expression</b> object that identifies character or characters to use in separating the string. If omitted, a single-element array containing the entire
        string is returned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">limit</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A value used to limit the number of elements returned in the array.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The result of the <b>split</b> method is an array of strings split at each point where <span class="parameter" sdata="paramReference">separator</span> occurs in <span class="parameter" sdata=
    "paramReference">stringObj</span>. The <span class="parameter" sdata="paramReference">separator</span> is not returned as part of any array element.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>split</b> method.
</p>

```
var s = "The quick brown fox jumps over the lazy dog."; var ss = s.split(" "); for (i in ss) { document.write(ss[i]; document.write("&lt;br/&gt;"); } // Output: // The // quick // brown // fox //
jumps // over // the // lazy // dog.
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="5d28ebb2-d534-4179-9297-a4c821ee9f24.htm">concat Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7f6b1073-8cbb-49ed-94b6-56833ba663c5.htm">RegExp Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="346aa83e-a045-47ea-acae-b42c7b121534.htm">Regular Expression Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
</div>

