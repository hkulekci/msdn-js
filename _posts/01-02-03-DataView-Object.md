---
title: DataView Object
---

### Introduction 

 You can use a DataView object to read and write the different kinds of binary data to any location in the ArrayBuffer.

### Syntax 

```
dataView = new DataView(DataView(buffer , byteOffset , byteLength ));
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">dataView</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <b>DataView</b> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">buffer</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The ArrayBuffer that the DataView represents.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">byteOffset</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Specifies the offset in bytes from the start of the buffer at which the DataView should begin.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">byteLength</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Specifies the length (in bytes) of the section of the buffer that the DataView should represent.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If both byteOffset and byteLength are omitted, the DataView spans the entire ArrayBuffer range. If the byteLength is omitted, the DataView extends from the given byteOffset until the end of the
    ArrayBuffer. If the given byteOffset and byteLength references an area beyond the end of the ArrayBuffer, an exception is raised.
  </p>
</div>

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the properties of the <b>DataView</b> object.
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
            buffer Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Read-only. Gets the ArrayBuffer that is referenced by this view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            byteLength Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Read-only. The length of this view from the start of its ArrayBuffer, in bytes, as fixed at construction time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            byteOffset Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Read-only. The offset of this view from the start of its ArrayBuffer, in bytes, as fixed at construction time.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Methods 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the methods of the <b>DataView</b>object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Method
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
            getInt8 Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets the Int8 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="9fbf4be3-4c0b-4963-a7a1-d57f1501b4cf.htm">getUint8 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets the Uint8 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="d364cbe0-48a6-4350-a6ca-9f563d7ae571.htm">getInt16 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets the Int16 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="3c0d9ad8-30b0-42a3-b0fe-aa805398c396.htm">getUint16 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets the Uint16 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="7a985681-ddb1-4c2b-815c-514c17392e82.htm">getInt32 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets the Int32 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="266ee6b6-c0b6-417e-a64b-c8cda48fde86.htm">getUint32 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets the Uint32 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="adecf671-bde4-46be-a875-33b6d6e970b1.htm">getFloat32 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets the Float32 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="347adeb6-b24c-4e7d-8b6b-8e36aacdcae1.htm">getFloat64 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets the Float64 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="0a0e1450-e0c4-4778-8706-4d332442d882.htm">setInt8 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Stores a Int8 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="b294262b-3f4b-4183-a292-5a6982cbdd27.htm">setUint8 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Stores a Uint8 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="901c6cf5-63fb-45bd-9ea8-185c1d892060.htm">setInt16 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Stores a Int16 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="bdf47cda-7fa5-4aaa-8aa2-8cf9a8d56cb3.htm">setUint16 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Stores a Uint16 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="07e5f068-0e3f-4c23-84b3-c72658d7f194.htm">setInt32 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Stores a Int32 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="ab2894fe-4cdc-40c8-9503-951e42ca61e7.htm">setUint32 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Stores a Uint32 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="b3f68048-c817-48d2-bc17-945e3bcc94d7.htm">setFloat32 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Stores a Float32 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="63d2c631-876f-4d4b-b3b6-62b0aaffe6c5.htm">setFloat64 Method (DataView)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Stores a Float64 value at the specified byte offset from the start of the view.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use a DataView object to process the binary data acquired from an XmlHttpRequest:
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); var ints = new Int32Array(dataView.byteLength / 4); for (var i = 0; i &lt; ints.length; i++) { ints[i] = dataview.getInt32(i * 4); }
alert(ints[10]); } }
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

