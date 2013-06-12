---
title: slice Method (Array) (JavaScript)
isChild: false
---

## slice Method (Array) (JavaScript) {slice_method_array_javascript_title}

### Introduction 

 Returns a section of an array.

### Syntax 

```
arrayObj .slice(start , [end ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arrayObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An <b>Array</b> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">start</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The beginning of the specified portion of <span class="parameter" sdata="paramReference">arrayObj</span>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">end</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The end of the specified portion of <span class="parameter" sdata="paramReference">arrayObj</span>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>slice</b> method returns an <b>Array</b> object containing the specified portion of <span class="parameter" sdata="paramReference">arrayObj</span>.
  </p>
  <p xmlns:util="util">
    The <b>slice</b> method copies up to, but not including, the element indicated by <span class="parameter" sdata="paramReference">end</span>. If <span class="parameter" sdata=
    "paramReference">start</span> is negative, it is treated as <span class="parameter" sdata="paramReference">length</span> + <span class="parameter" sdata="paramReference">start</span>, where
    <span class="parameter" sdata="paramReference">length</span> is the length of the array. If <span class="parameter" sdata="paramReference">end</span> is negative, it is treated as <span class=
    "parameter" sdata="paramReference">length</span> + <span class="parameter" sdata="paramReference">end</span> where <span class="parameter" sdata="paramReference">length</span> is the length of
    the array. If <span class="parameter" sdata="paramReference">end</span> is omitted, extraction continues to the end of <span class="parameter" sdata="paramReference">arrayObj</span>. If
    <span class="parameter" sdata="paramReference">end</span> occurs before <span class="parameter" sdata="paramReference">start</span>, no elements are copied to the new array.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following examples show how to use the <span sdata="langKeyword" value="slice"><span class="keyword">slice</span></span> method. In the first example, all but the last element of <span class=
  "code">myArray</span> is copied into <span class="code">newArray</span>. In the second example, only the last two elements of <span class="code">myArray</span> are copied into <span class=
  "code">newArray</span>.
</p>

```
var origArray = [3, 5, 7, 9]; var newArray = origArray. slice(0, -1); document.write(origArray); document.write("&lt;br/&gt;"); newArray = origArray. slice(-2); document.write(newArray); // Output:
// 3,5,7,9 // 7,9
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="80cd77a6-3718-492e-8e96-f909d8721d91.htm">slice Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

