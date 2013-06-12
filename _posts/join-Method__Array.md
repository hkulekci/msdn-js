---
title: join Method (Array) (JavaScript)
isChild: false
---

## join Method (Array) (JavaScript) {join_method_array_javascript_title}

### Introduction 

 Adds all the elements of an array separated by the specified separator string.

### Syntax 

```
arrayObj .join([separator ])
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">separator</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A string used to separate one element of an array from the next in the resulting <span sdata="langKeyword" value="String"><span class="keyword">String</span></span>. If omitted, the
        array elements are separated with a comma.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If any element of the array is <b>undefined</b> or <span sdata="langKeyword" value="null"><span class="keyword">null</span></span>, it is treated as an empty string.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>join</b> method.
</p>

```
var a, b; a = new Array(0,1,2,3,4); b = a.join( "-") ; document.write(b); // Output: // 0-1-2-3-4
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
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

