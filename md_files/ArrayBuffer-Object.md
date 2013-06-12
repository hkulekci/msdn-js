---
title: ArrayBuffer Object
isChild: false
---

## ArrayBuffer Object {arraybuffer_object_title}

### Introduction 

 Represents a raw buffer of binary data, which is used to store data for the different typed arrays. ArrayBuffers cannot be read from or written to directly, but can be passed to a typed array or
DataView Object to interpret the raw buffer as needed. For more information about typed arrays, see Typed Arrays .

### Syntax 

```
arrayBuffer = new ArrayBuffer(length);
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arrayBuffer</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <b>ArrayBuffer</b> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">length</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The length of the buffer. The contents of the ArrayBuffer are initialized to 0. If the requested number of bytes could not be allocated an exception is raised.
      </p>
    </dd>
  </dl>
</div>

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the properties of the <b>ArrayBuffer</b> object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Property
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Description
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            byteLength Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Read-only. The length of the ArrayBuffer (in bytes).
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use an ArrayBuffer object to process the binary data acquired from an <span sdata="link">XmlHttpRequest</span>. You can use a <span sdata="link"><a href=
  "250ec067-7505-4ee0-82ab-bfd3c2820afa.htm">DataView Object</a></span> to get the individual values.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataview = new DataView(buffer); var ints = new Int32Array(buffer.byteLength / 4); for (var i = 0; i &lt; ints.length; i++) { ints[i] = dataview.getInt32(i * 4); }
alert(ints[10]); } }
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    For more information about using <span sdata="link">XmlHttpRequest</span>, see <span sdata="link">XMLHttpRequest enhancements</span>.
  </p>
</div>

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

