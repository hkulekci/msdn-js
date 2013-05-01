## [get Method (Uint32Array)](get-Method__Uint32Array.html)

### Introduction 

 Omittable. Gets the element at the specified index.

### Syntax 

```
var value = uint32Array.get(index);
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">value</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The value returned by this method.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">index</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The index at which to get the element of the array.
      </p>
    </dd>
  </dl>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to get the first element of the array.
</p>

```
var req = new XMLHttpRequest(); req.open('GET', "http://www.example.com"); req.responseType = "arraybuffer"; req.send(); req.onreadystatechange = function () { if (req.readyState === 4) { var buffer
= req.response; var dataView = new DataView(buffer); var intArr = new Int32Array(buffer.byteLength / 4); var element = intArr.get(0); } }
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

