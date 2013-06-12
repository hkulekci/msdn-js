---
title: buffer Property (Int16Array)
isChild: false
---

## buffer Property (Int16Array) {buffer_property_int16array_title}

### Introduction 

 Read-only. Gets the ArrayBuffer that is referenced by this array.

### Syntax 

```
var arrayBuffer = int16Array.buffer;
```

#### Example 

<p xmlns:util="util">
  The following example shows how to get the ArrayBuffer of the array.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); var intArr = new Int16Array(buffer.byteLength / 2); alert(intArr.buffer.byteLength); } }
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

