---
title: BYTES_PER_ELEMENT Constant (Float64Array)
isChild: false
---

## BYTES_PER_ELEMENT Constant (Float64Array) {bytes_per_element_constant_float64array_title}

### Introduction 

 The size in bytes of each element in the array.

### Syntax 

```
var arraySize = int8Array.BYTES_PER_ELEMENT;
```

#### Example 

<p xmlns:util="util">
  The following example shows how to get the size of the array elements.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); var floatArr = new Float64Array(buffer.byteLength / 8); alert(floatArr.BYTES_PER_ELEMENT); } }
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

