## [ubound Method (VBArray) (JavaScript)](ubound-Method__VBArray.html)

### Introduction 

 Returns the highest index value used in the specified dimension of the VBArray.

### Syntax 

```
safeArray .ubound(dimension )
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">dimension</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The dimension of the VBArray for which the higher bound index is wanted. If omitted, <b>ubound</b> behaves as if a 1 was passed.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the VBArray is empty, the <b>ubound</b> method returns undefined. If <span class="parameter" sdata="paramReference">dim</span> is greater than the number of dimensions in the VBArray, or is
    negative, the method generates a "Subscript out of range" error.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example consists of three parts. The first part is VBScript code to create a Visual Basic safe array. The second part is JavaScript code that determines the number of dimensions in
  the safe array and the upper bound of each dimension. Both of these parts go into the &lt;HEAD&gt; section of an HTML page. The third part is the JavaScript code that goes in the &lt;BODY&gt;
  section to run the other two parts.
</p>

```
&lt;head&gt; &lt;script type="text/vbscript"&gt; &lt;!-- Function CreateVBArray() Dim i, j, k Dim a(2, 2) k = 1 For i = 0 To 2 For j = 0 To 2 a(j, i) = k k = k + 1 Next Next CreateVBArray = a End
Function --&gt; &lt;/script&gt; &lt;script type="text/javascript"&gt; &lt;!-- function VBArrayTest(vba) { var i; var a = new VBArray(vba); var s = ""; for (i = 1; i &lt;= a.dimensions(); i++) { s +=
"The upper bound of dimension "; s += i + " is "; s += a.ubound( i) ; s += ".&lt;br /&gt;"; } return (s); } --&gt; &lt;/script&gt; &lt;/head&gt; &lt;body&gt; &lt;script type="text/javascript"&gt;
document.write(VBArrayTest(CreateVBArray())); &lt;/script&gt; &lt;/body&gt;
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
    <span sdata="link" xmlns:util="util"><a href="664de44c-2039-4289-82f6-948e9d744d80.htm">toArray Method (VBArray) (JavaScript)</a></span>
  </div>
</div>

