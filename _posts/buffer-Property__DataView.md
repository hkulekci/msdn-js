---
title: buffer Property (DataView)
isChild: false
---

## buffer Property (DataView) {buffer_property_dataview_title}

### Introduction 

 Read-only. Gets the ArrayBuffer that is referenced by this view.

### Syntax 

```
var arrayBuffer = dataView.buffer;
```

#### Example 

<p xmlns:util="util">
  The following example shows how to get the length of the ArrayBuffer underlying the DataView.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); alert(dataView.buffer.byteLength) } }
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

