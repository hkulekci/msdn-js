---
title: byteLength Property (DataView)
---

### Introduction 

 Read-only. The length of this view from the start of its ArrayBuffer, in bytes, as fixed at construction time.

### Syntax 

```
var byteLength = dataView.byteLength;
```

#### Example 

<p xmlns:util="util">
  The following example shows how get the length of a DataView from an XMLHttpRequest.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = dataView.buffer; alert(dataView.byteLength); } }
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

