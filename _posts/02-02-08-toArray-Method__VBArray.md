---
title: toArray Method (VBArray) (JavaScript)
---

### Introduction 

 Returns a standard JavaScript array converted from a VBArray.

### Syntax 

```
safeArray .toArray( )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <i>safeArray</i> reference is a VBArray object.
  </p>
  <p xmlns:util="util">
    The conversion translates the multidimensional VBArray into a single dimensional JavaScript array. Each successive dimension is appended to the end of the previous one. For example, a VBArray
    with three dimensions and three elements in each dimension is converted into a JavaScript array as follows:
  </p>
  <p xmlns:util="util">
    Suppose the VBArray contains: (1, 2, 3), (4, 5, 6), (7, 8, 9). After translation, the JavaScript array contains: 1, 2, 3, 4, 5, 6, 7, 8, 9.
  </p>
  <p xmlns:util="util">
    There is currently no way to convert a JavaScript array into a VBArray.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example consists of three parts. The first part is VBScript code to create a Visual Basic safe array. The second part is JavaScript code that converts the Visual Basic safe array to a
  JavaScript array. Both of these parts go into the &lt;HEAD&gt; section of an HTML page. The third part is the JavaScript code that goes in the &lt;BODY&gt; section to run the other two parts.
</p>

```
&lt;head&gt; &lt;script type="text/vbscript"&gt; &lt;!-- Function CreateVBArray() Dim i, j, k Dim a(2, 2) k = 1 For i = 0 To 2 For j = 0 To 2 a(j, i) = k document.writeln(k) k = k + 1 Next
document.writeln("&lt;BR&gt;") Next CreateVBArray = a End Function --&gt; &lt;/script&gt; &lt;script type="text/javascript"&gt; &lt;!-- function VBArrayTest(vbarray) { var a = new VBArray(vbarray);
var b = a.toArray() ; var i; for (i = 0; i &lt; 9; i++) { document.writeln(b[i]); } } --&gt; &lt;/script&gt; &lt;/head&gt; &lt;body&gt; &lt;script type="text/javascript"&gt; &lt;!--
VBArrayTest(CreateVBArray()); --&gt; &lt;/script&gt; &lt;/body&gt;
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
    <span sdata="link" xmlns:util="util"><a href="f62964ad-8b2f-4596-95d0-b20e587ecea5.htm">getItem Method (VBArray) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="30ff5e8a-8165-494b-bce8-0a562ec2eec3.htm">lbound Method (VBArray) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="761811c5-9a3d-4cb3-bfe0-0a8749f34496.htm">ubound Method (VBArray) (JavaScript)</a></span>
  </div>
</div>

