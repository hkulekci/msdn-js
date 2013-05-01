## [Error Object (JavaScript)](Error-Object.html)

### Introduction 

 Contains information about errors.

### Syntax 

```
errorObj = new Error() errorObj = new Error([number ]) errorObj = new Error([number [, description ]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">errorObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">number</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Numeric value assigned to an error. Zero if omitted.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">description</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Brief string that describes an error. Empty string if omitted.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Whenever a run-time error occurs, an instance of the <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> object is created to describe the error. This instance has
    two intrinsic properties that contain the description of the error (<b>description</b> property) and the error number (<b>number</b> property).
  </p>
  <p xmlns:util="util">
    An error number is a 32-bit value. The upper 16-bit word is the facility code, while the lower word is the actual error code.
  </p>
  <p xmlns:util="util">
    <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> objects can also be explicitly created, using the syntax shown above, or thrown using the <span sdata=
    "langKeyword" value="throw"><span class="keyword">throw</span></span> statement. In both cases, you can add any properties you choose to expand the capability of the <span sdata="langKeyword"
    value="Error"><span class="keyword">Error</span></span> object.
  </p>
  <p xmlns:util="util">
    Typically, the local variable that is created in a <b>try...catch</b> statement refers to the implicitly created <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span>
    object. As a result, you can use the error number and description in any way you choose.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> object.
</p>

```
function checkInput(x) { try { if (isNaN(parseInt(x))) { throw new Error("Input is not a number."); } } catch(e) { document.write(e.description); } }
```

<p xmlns:util="util">
  The following example illustrates the use of the implicitly created <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> object.
</p>

```
try { // Cause an error. x = y; } catch(e) { document.write(e); document.write ("&lt;br /&gt;"); document.write ("Number: "); document.write (e.number &amp; 0xFFFF); document.write ("&lt;br /&gt;");
document.write ("Facility Code: "); document.write(e.number&gt;&gt;16 &amp; 0x1FFF); document.write ("&lt;br /&gt;"); document.write ("Description: "); document.write (e.description); } // Output: //
ReferenceError: 'y' is undefined // Facility Code: 10 // Number: 5009 // Description: 'y' is undefined
```

#### Methods 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    <span sdata="link"><a href="5d6d9712-c06d-4b31-9bc9-e46f6bb5cd38.htm">toString Method (Error)</a></span> | <span sdata="link"><a href="39a1f96e-14b0-4db2-b53d-cdfd67cbb208.htm">valueOf Method
    (Date)</a></span>
  </p>
</div>

#### Properties 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    <span sdata="link"><a href="18aea278-2bd5-457b-83a5-d8d8f1226e0c.htm">constructor Property (Error)</a></span> | description Property | message Property | name Property | number Property |
    <span sdata="link"><a href="6c268a51-1a3d-4397-abf8-e54ca4e598fe.htm">prototype Property (Error)</a></span> | <span sdata="link"><a href="1dc21fdd-853c-4664-bf1c-24eb1f6f2daf.htm">stack Property
    (Error) (JavaScript)</a></span> | <span sdata="link"><a href="127ef8e8-892e-4263-9ebc-03364af01212.htm">stackTraceLimit Property (Error) (JavaScript)</a></span>
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="5ea556ba-7ae6-426c-8430-9032eee5a0a5.htm">new Operator (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="75cbade0-fb81-4ffe-b187-b71be380bb05.htm">throw Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="b7a0a54e-dfaa-4e41-bf25-bcaa43e601fb.htm">try...catch...finally Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="56f900af-a5c4-4667-9664-5956d30f0aae.htm">var Statement (JavaScript)</a></span>
  </div>
</div>

