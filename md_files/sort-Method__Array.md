## [sort Method (Array) (JavaScript)](sort-Method__Array.html)

### Introduction 

 Sorts an Array.

### Syntax 

```
arrayobj .sort(sortFunction )
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
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">sortFunction</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The name of the function used to determine the order of the elements. If omitted, the elements are sorted in ascending, ASCII character order.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The sorted array.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>sort</b> method sorts the <b>Array</b> object in place; no new <b>Array</b> object is created during execution.
  </p>
  <p xmlns:util="util">
    If you supply a function in the <span class="parameter" sdata="paramReference">sortFunction</span> argument, it must return one of the following values:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        A negative value if the first argument passed is less than the second argument.
      </p>
    </li>
    <li>
      <p>
        Zero if the two arguments are equivalent.
      </p>
    </li>
    <li>
      <p>
        A positive value if the first argument is greater than the second argument.
      </p>
    </li>
  </ul>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>sort</b> method.
</p>

```
var a = new Array(4, 11, 2, 10, 3, 1); var b = a.sort(); document.write(b); document.write("&lt;br/&gt;"); // This is ASCII character order. // Output: 1,10,11,2,3,4) // Sort the array elements with
a function that compares array elements. b = a.sort(CompareForSort); document.write(b); document.write("&lt;br/&gt;"); // Output: 1,2,3,4,10,11. // Sorts array elements in ascending order
numerically. function CompareForSort(first, second) { if (first == second) return 0; if (first &lt; second) return -1; else return 1; }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

