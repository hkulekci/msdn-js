## [number Property (Error) (JavaScript)](number-Property__Error.html)

### Introduction 

 Returns or sets the numeric value associated with a specific error. The Error object's default property is number.

### Syntax 

```
object .number [= errorNumber ]
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">Object</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any instance of the <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> object.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">errorNumber</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        An integer representing an error.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    An error number is a 32-bit value. The upper 16-bit word is the facility code, and the lower word is the error code. To determine the error code, use the <span sdata="langKeyword" value=
    "&amp;"><span class="keyword">&amp;</span></span> (bitwise And) operator to combine the number property with the hexadecimal number <span class="code">0xFFFF</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example causes an exception to be thrown and displays the error code that is derived from the error number.
</p>

```
try { // Cause an error. var x = y; } catch(e) { document.write ("Error Code: "); document.write (e.number &amp; 0xFFFF) document.write ("&lt;br /&gt;"); document.write ("Facility Code: ")
document.write(e.number&gt;&gt;16 &amp; 0x1FFF) document.write ("&lt;br /&gt;"); document.write ("Error Message: ") document.write (e.message) }
```

<p xmlns:util="util">
  The output of this code is as follows.
</p>

```
Error Code: 5009 Facility Code: 10 Error Message: 'y' is undefined
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="0b27d6ec-3997-4e91-a6c0-5afbaf494db7.htm">Error Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ea727f1e-2041-4400-965c-67e6d47a1ff0.htm">description Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8cab0392-e0db-4714-827c-47ab04e8b4f2.htm">message Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="94df2d6b-f1a1-4931-a956-0a930cb87f76.htm">name Property (Error) (JavaScript)</a></span>
  </div>
</div>

