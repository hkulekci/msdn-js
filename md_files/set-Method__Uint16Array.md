## [set Method (Uint16Array)](set-Method__Uint16Array.html)

### Introduction 

 Sets a value or an array of values.

### Syntax 

```
int8Array.set(index, value); 
int8Array.set(array, offset);
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">index</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The index of the location to set.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">value</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The value to set.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">array</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        A typed or untyped array of values to set.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">offset</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The index in the current array at which the values are to be written.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the input array is a TypedArray, the two arrays may use the same underlying ArrayBuffer. In this situation, setting the values takes place as if all the data is first copied into a temporary
    buffer that does not overlap either of the arrays, and then the data from the temporary buffer is copied into the current array.
  </p>
  <p xmlns:util="util">
    If the offset plus the length of the given array is out of range for the current TypedArray, an exception is raised.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to set the first element of the array.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); var intArr = new Uint16Array(buffer.byteLength / 2); intArr.set(0, 9); } }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the Internet Explorer 10 standards document mode. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards.
  </p>
</div>

