---
title: indexOf Method (String) (JavaScript)
---

### Introduction 

 Returns the position of the first occurrence of a substring.

### Syntax 

```
strObj . indexOf(subString [, startIndex ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">strObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">subString</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The substring to search for in the string
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">startIndex</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The index at which to begin searching the <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object. If omitted, search starts at the beginning of
        the string.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>indexOf</b> method returns the beginning of the substring in the <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object. If the substring is not found,
    -1 is returned.
  </p>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">startindex</span> is negative, <span class="parameter" sdata="paramReference">startindex</span> is treated as zero. If it is greater than the
    highest index, it is treated as the highest index.
  </p>
  <p xmlns:util="util">
    Searching is performed from left to right. Otherwise, this method is identical to <b>lastIndexOf</b>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>indexOf</b> method.
</p>

```
var str = "original equipment manufacturer"; var s = "equip is at position " + str.indexOf("equip"); s += "&lt;br /&gt;"; s += "abc is at position " + str.indexOf("abc"); document.write(s); //
Output: // equip is at position 9 // abc is at position -1
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
    <span sdata="link" xmlns:util="util"><a href="1ed36ccd-0f0b-4f16-be45-0567207670af.htm">lastIndexOf Method (String) (JavaScript)</a></span>
  </div>
</div>

