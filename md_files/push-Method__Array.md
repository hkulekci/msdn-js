## [push Method (Array) (JavaScript)](push-Method__Array.html)

### Introduction 

 Appends new elements to an array, and returns the new length of the array.

### Syntax 

```
arrayObj .push([item1 [item2 [. . . [itemN ]]]])
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">item, item2,. . ., itemN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. New elements of the <b>Array</b>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>push</b> and <b>pop</b> methods allow you to simulate a last in, first out stack.
  </p>
  <p xmlns:util="util">
    The <b>push</b> method appends elements in the order in which they appear. If one of the arguments is an array, it is added as a single element. Use the <b>concat</b> method to join the elements
    from two or more arrays.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>push</b> method.
</p>

```
var number; var my_array = new Array(); my_array.push (5, 6, 7); my_array.push (8, 9); number = my_array.pop(); while (number != undefined) { document.write (number + " "); number = my_array.pop(); }
// Output: // 9 8 7 6 5
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
    <span sdata="link" xmlns:util="util"><a href="bc2b4a6a-209e-4d59-8c24-59db01d53b1e.htm">concat Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4fae7f98-29f1-4041-ba43-601f2e5145ec.htm">pop Method (Array) (JavaScript)</a></span>
  </div>
</div>

