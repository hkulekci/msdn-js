---
title: substr Method (String) (JavaScript)
isChild: false
---

## substr Method (String) (JavaScript) {substr_method_string_javascript_title}

### Introduction 

 Gets a substring beginning at the specified location and having the specified length.

### Syntax 

```
stringvar .substr(start [, length ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringvar</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A string literal or <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object from which the substring is extracted.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">start</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The starting position of the desired substring. The index of the first character in the string is zero.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">length</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The number of characters to include in the returned substring.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">length</span> is zero or negative, an empty string is returned. If not specified, the substring continues to the end of <span class="parameter"
    sdata="paramReference">stringvar</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>substr</b> method.
</p>

```
var s = "The quick brown fox jumps over the lazy dog."; var ss = s.substr(10, 5); document.write("[" + ss + "] &lt;br&gt;"); ss = s.substr(10); document.write("[" + ss + "] &lt;br&gt;"); ss =
s.substr(10, -5); document.write("[" + ss + "] &lt;br&gt;"); // Output: // [brown] // [brown fox jumps over the lazy dog.] // []
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
    <span sdata="link" xmlns:util="util"><a href="9cf9a005-cbe3-42fd-828b-57a39f54224c.htm">substring Method (String) (JavaScript)</a></span>
  </div>
</div>

