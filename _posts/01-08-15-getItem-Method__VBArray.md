---
title: getItem Method (VBArray) (JavaScript)
---

### Introduction 

 Returns the item at the specified location.

### Syntax 

```
safeArray .getItem(dimension1 [, dimension2 , ...], dimensionN )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">safeArray</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A VBArray object.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">dimension1, ..., dimensionN</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Specifies the exact location of the desired element of the VBArray. <i>n</i> equals the number of dimensions in the VBArray.
      </p>
    </dd>
  </dl>
</div>

#### Example 

<p xmlns:util="util">
  The following example consists of three parts. The first part is VBScript code to create a Visual Basic safe array. The second part is JavaScript code that iterates the Visual Basic safe array and
  prints out the contents of each element. Both of these parts go into the &lt;HEAD&gt; section of an HTML page. The third part is the JavaScript code that goes in the &lt;BODY&gt; section to run the
  other two parts.
</p>

```
&lt;head&gt; &lt;script type="text/vbscript"&gt; &lt;!-- Function CreateVBArray() Dim i, j, k Dim a(2, 2) k = 1 For i = 0 To 2 For j = 0 To 2 a(i, j) = k document.writeln(k) k = k + 1 Next
document.writeln("&lt;BR&gt;") Next CreateVBArray = a End Function --&gt; &lt;/script&gt; &lt;script type="text/javascript"&gt; &lt;!-- function GetItemTest(vbarray) { var i, j; var a = new
VBArray(vbarray); for (i = 0; i &lt;= 2; i++) { for (j =0; j &lt;= 2; j++) { document.writeln(a.getItem( i, j) ); } } } --&gt; &lt;/script&gt; &lt;/head&gt; &lt;body&gt; &lt;script
type="text/javascript"&gt; &lt;!-- GetItemTest(CreateVBArray()); --&gt; &lt;/script&gt; &lt;/body&gt;
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, and Internet
    Explorer 10 standards. Not supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="f0b767f1-ea8a-4726-962b-2708d4742518.htm">VBArray Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ac83589e-85d9-48cb-b28d-c579e65fd604.htm">dimensions Method (VBArray) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="30ff5e8a-8165-494b-bce8-0a562ec2eec3.htm">lbound Method (VBArray) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="664de44c-2039-4289-82f6-948e9d744d80.htm">toArray Method (VBArray) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="761811c5-9a3d-4cb3-bfe0-0a8749f34496.htm">ubound Method (VBArray) (JavaScript)</a></span>
  </div>
</div>

