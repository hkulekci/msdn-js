## [reverse Method (JavaScript)](reverse-Method.html)

### Introduction 

 Reverses the elements in an Array.

### Syntax 

```
arrayObj .reverse()
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arrayObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any <b>Array</b> object.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The reversed array.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">arrayObj</span> reference is an <b>Array</b> object.
  </p>
  <p xmlns:util="util">
    The <b>reverse</b> method reverses the elements of an <b>Array</b> object in place. It does not create a new <b>Array</b> object during execution.
  </p>
  <p xmlns:util="util">
    If the array is not contiguous, the <b>reverse</b> method creates elements in the array that fill the gaps in the array. Each of these created elements has the value <span sdata="langKeyword"
    value="undefined"><span class="keyword">undefined</span></span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>reverse</b> method.
</p>

```
var arr = new Array(0,1,2,3,4); var reverseArr = arr.reverse(); document.write(reverseArr); // Output: // 4,3,2,1,0
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
</div>

