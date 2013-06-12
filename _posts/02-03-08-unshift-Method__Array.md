---
title: unshift Method (Array) (JavaScript)
---

### Introduction 

 Inserts new elements at the start of an array.

### Syntax 

```
arrayObj .unshift([item1 [, item2 [, . . . [, itemN]]]])
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">item1, item2,. . ., itemN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Elements to insert at the start of the <b>Array</b>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>unshift</b> method inserts elements into the start of an array, so they appear in the same order in which they appear in the argument list.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="unshift"><span class="keyword">unshift</span></span> method.
</p>

```
var ar = new Array(); ar.unshift(10, 11); ar.unshift(12, 13, 14); document.write(ar.toString()); // Output: 12,13,14,10,11
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
    <span sdata="link" xmlns:util="util"><a href="f33baec5-f67e-4760-b7c1-553727bd0423.htm">shift Method (Array) (JavaScript)</a></span>
  </div>
</div>

