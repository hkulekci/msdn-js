---
title: subarray Method (Int8Array)
isChild: false
---

## subarray Method (Int8Array) {subarray_method_int8array_title}

### Introduction 

 Gets a new Int8Array view of the ArrayBuffer store for this array, referencing the elements at begin, inclusive, up to end, exclusive.

### Syntax 

```
var newInt8Array = int8Array.subset(begin, end);
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">newInt8Array</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The subarray returned by this method.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">begin</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The index of the beginning of the array.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">end</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The index of the end of the array.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If either begin or end is negative, it refers to an index from the end of the array, as opposed to from the beginning. If end is unspecified, the subarray contains all elements from begin to the
    end of the TypedArray. The range specified by the begin and end values is clamped to the valid index range for the current array. If the computed length of the new TypedArray would be negative,
    it is clamped to zero. The returned TypedArray will be of the same type as the array on which this method is invoked.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to get a subarray three elements long, starting with the first element of the array.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); var intArr = new Int8Array(buffer.byteLength); var subArr = intArr.subarray(0, 2); } }
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

