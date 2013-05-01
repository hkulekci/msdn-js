## [Uint16Array Object](Uint16Array-Object.html)

### Introduction 

 A typed array of 16-bit unsigned integer values. The contents are initialized to 0. If the requested number of bytes could not be allocated an exception is raised.

### Syntax 

```
uint16Array = new Uint16Array( length ); 
uint16Array = new Uint16Array( array ); 
uint16Array = new Uint16Array( buffer , byteOffset , length );
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">uint16Array</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <b>Uint16Array</b> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">length</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Specifies the length (in bytes) of the array.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">array</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The array (or typed array) that is contained in this array.. The contents are initialized to the contents of the given array or typed array, with each element converted to the Uint16 type.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">buffer</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The ArrayBuffer that the Uint16Array represents.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">byteOffset</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Specifies the offset in bytes from the start of the buffer at which the Uint16Array should begin.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">length</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The length of the array.
      </p>
    </dd>
  </dl>
</div>

#### Constants 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the constants of the <b>Uint16Array</b>object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Constant
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
            BYTES_PER_ELEMENT Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The size in bytes of each element in the array.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Properties 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the constants of the <b>Uint16Array</b>object.
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
            Read-only. Gets the ArrayBuffer that is referenced by this array.
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
            Read-only. The length of this array from the start of its ArrayBuffer, in bytes, as fixed at construction time.
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
            Read-only. The offset of this array from the start of its ArrayBuffer, in bytes, as fixed at construction time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            length Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The length of the array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Methods 

<div id="sectionSection3" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the methods of the <b>Uint16Array</b>object.
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
            get Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Omittable. Gets the element at the specified index.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="5bfbc50b-d786-4c0d-918a-ae1241a32626.htm">set Method (Uint16Array)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets a value or an array of values.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link"><a href="00b7d3d0-0b47-4da0-95fa-44c9b419d7d0.htm">subarray Method (Uint16Array)</a></span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets a new Uint16Array view of the ArrayBuffer store for this array.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use a Uint16Array object to process the binary data acquired from an XmlHttpRequest:
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataview = new DataView(buffer); var ints = new Uint16Array(buffer.byteLength / 2); for (var i = 0; i &lt; ints.length; i++) { ints[i] = dataview.getUint16(i * 2); }
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

