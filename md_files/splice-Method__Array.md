## [splice Method (Array) (JavaScript)](splice-Method__Array.html)

### Introduction 

 Removes elements from an array and, if necessary, inserts new elements in their place, returning the deleted elements.

### Syntax 

```
arrayObj .splice(start, deleteCount, [item1 [, item2 [, . . . [,itemN ]]]])
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
        Required. The zero-based location in the array from which to start removing elements.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">deleteCount</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The number of elements to remove.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">item1, item2,. . ., itemN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Elements to insert into the array in place of the deleted elements.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>splice</b> method modifies <span class="parameter" sdata="paramReference">arrayObj</span> by removing the specified number of elements from position <span class="parameter" sdata=
    "paramReference">start</span> and inserting new elements. The deleted elements are returned as a new <b>Array</b> object.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use the <b>splice</b> method.
</p>

```
var arr = new Array("4", "11", "2", "10", "3", "1"); arr.splice(2, 2, "21", "31"); document.write(arr); // Output: 4,11,21,31,3,1
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
    <span sdata="link" xmlns:util="util"><a href="3c122219-14de-4126-b091-809659c026d6.htm">slice Method (Array) (JavaScript)</a></span>
  </div>
</div>

