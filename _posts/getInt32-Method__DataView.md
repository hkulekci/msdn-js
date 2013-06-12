---
title: getInt32 Method (DataView)
isChild: false
---

## getInt32 Method (DataView) {getint32_method_dataview_title}

### Introduction 

 Gets the Int32 value at the specified byte offset from the start of the view. There is no alignment constraint; multi-byte values may be fetched from any offset.

### Syntax 

```
var testInt = dataView.getInt32(byteOffset, littleEndian);
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">testInt</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The Int32 value that is returned from the method.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">byteOffset</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The place in the buffer at which the value should be retrieved.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">littleEndian</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. If false or undefined, a big-endian value should be read, otherwise a little-endian value should be read.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    These methods raise an exception if they would read beyond the end of the view.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to get the first Int32 in the DataView.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); alert(dataView.getInt32(0)); } }
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

