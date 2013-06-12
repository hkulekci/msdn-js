---
title: pop Method (Array) (JavaScript)
isChild: false
---

## pop Method (Array) (JavaScript) {pop_method_array_javascript_title}

### Introduction 

 Removes the last element from an array and returns it.

### Syntax 

```
arrayObj .pop( )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The push and <b>pop</b> methods enable you to simulate a stack, which uses the principle of last in, first out (LIFO) to store data.
  </p>
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">arrayObj</span> reference is an <b>Array</b> object.
  </p>
  <p xmlns:util="util">
    If the array is empty, <span sdata="langKeyword" value="undefined"><span class="keyword">undefined</span></span> is returned.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="pop"><span class="keyword">pop</span></span> method.
</p>

```
var number; var my_array = new Array(); my_array.push (5, 6, 7); my_array.push (8, 9); number = my_array.pop(); while (number != undefined) { document.write (number + " "); number = my_array.pop(); }
// Output: 9 8 7 6 5
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
    <span sdata="link" xmlns:util="util"><a href="fa6e5799-dabe-4b3d-bd1f-0afc68c77134.htm">push Method (Array) (JavaScript)</a></span>
  </div>
</div>

