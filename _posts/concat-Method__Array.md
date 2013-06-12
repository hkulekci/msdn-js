---
title: concat Method (Array) (JavaScript)
isChild: false
---

## concat Method (Array) (JavaScript) {concat_method_array_javascript_title}

### Introduction 

 Combines two or more arrays.

### Syntax 

```
array1 .concat([item1 [, item2 [, . . . [, itemN ]]]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">array1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The <b>Array</b> object to which the other arrays are concatenated.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">item1,. . ., itemN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Additional items to add to the end of <span class="parameter" sdata="paramReference">array1</span>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>concat</b> method returns an <b>Array</b> object containing the concatenation of <span class="parameter" sdata="paramReference">array1</span> and any other supplied items.
  </p>
  <p xmlns:util="util">
    The items to be added (<i>item1 itemN</i>) to the array are added, in order, starting from the first item in the list. If one of the items is an array, its contents are added to the end of
    <span class="parameter" sdata="paramReference">array1</span>. If the item is anything other than an array, it is added to the end of the array as a single array element.
  </p>
  <p xmlns:util="util">
    Elements of source arrays are copied to the resulting array as follows:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        If an object is copied from any of the arrays being concatenated to the new array, the object reference continues to point to the same object. A change in either the new array or the original
        array will result in a change to the other.
      </p>
    </li>
    <li>
      <p>
        If a number or string value is added to the new array, only the value is copied. Changing the value in one array does not affect the value in the other.
      </p>
    </li>
  </ul>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>concat</b> method when used with an array:
</p>

```
var a, b, c, d; a = new Array(1,2,3); b = "dog"; c = new Array(42, "cat"); d = a.concat(b, c); document.write(d); //Output: 1, 2, 3, "dog", 42, "cat"
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
    <span sdata="link" xmlns:util="util"><a href="5d28ebb2-d534-4179-9297-a4c821ee9f24.htm">concat Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="20f8fde1-014b-488e-9008-464a86e6b21f.htm">join Method (Array) (JavaScript)</a></span>
  </div>
</div>

