## [VBArray Object (JavaScript)](VBArray-Object.html)

### Introduction 

 Provides access to Visual Basic safe arrays. Caution This object is supported in Internet Explorer only, not in Windows Store apps.

### Syntax 

```
varName = new VBArray(safeArray )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">varName</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the VBArray is assigned.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">safeArray</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A VBArray value.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    VBArrays are read-only, and cannot be created directly. The <i>safeArray</i> argument must have obtained a VBArray value before being passed to the VBArray constructor. This can only be done by
    retrieving the value from an existing ActiveX or other object.
  </p>
  <p xmlns:util="util">
    VBArrays can have multiple dimensions. The indices of each dimension can be different. The <b>dimensions</b> method retrieves the number of dimensions in the array; the <b>lbound</b> and
    <b>ubound</b> methods retrieve the range of indices used by each dimension.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example consists of three parts. The first part is VBScript code to create a Visual Basic safe array. The second part is JavaScript code that converts the Visual Basic safe array to a
  JavaScript array. Both of these parts go into the &lt;HEAD&gt; section of an HTML page. The third part is the JavaScript code that goes in the &lt;BODY&gt; section to run the other two parts.
</p>

```
&lt;head&gt; &lt;script type="text/vbscript"&gt; &lt;!-- Function CreateVBArray() Dim i, j, k Dim a(2, 2) k = 1 For i = 0 To 2 For j = 0 To 2 a(j, i) = k document.writeln(k) k = k + 1 Next
document.writeln("&lt;br /&gt;") Next CreateVBArray = a End Function --&gt; &lt;/script&gt; &lt;script type="text/javascript"&gt; &lt;!-- function VBArrayTest(vbarray){ var a = new VBArray( vbarray)
; var b = a.toArray(); var i; for (i = 0; i &lt; 9; i++) { document.writeln(b[i]); } } --&gt; &lt;/script&gt; &lt;/head&gt; &lt;body&gt; &lt;script type="text/javascript"&gt; &lt;!--
VBArrayTest(CreateVBArray()); --&gt; &lt;/script&gt; &lt;/body&gt;
```

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The <b>VBArray</b> object has no properties.
  </p>
</div>

#### Methods 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    dimensions Method | getItem Method | lbound Method | toArray Method | ubound Method
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, and Internet
    Explorer 10 standards. Not supported in Windows Store apps. See Version Information.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>
  </div>
</div>

