---
title: length Property (Uint8Array)
isChild: false
---

## length Property (Uint8Array) {length_property_uint8array_title}

### Introduction 

 The length of the array.

### Syntax 

```
var arrayLength = uint8Array.length;
```

#### Example 

<p xmlns:util="util">
  The following example shows how to get the length of the array.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); var intArr = new Uint8Array(buffer.byteLength); alert(intArr.length); } }
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

