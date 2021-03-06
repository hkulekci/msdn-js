---
title: buffer Property (Int32Array)
isChild: false
---

## buffer Property (Int32Array) {buffer_property_int32array_title}

### Introduction 

 Read-only. Gets the ArrayBuffer that is referenced by this array.

### Syntax 

```
var arrayBuffer = int32Array.buffer;
```

#### Example 

<p xmlns:util="util">
  The following example shows how to get the ArrayBuffer of the array.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); var intArr = new Int32Array(buffer.byteLength / 4); alert(intArr.buffer.byteLength); } }
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

