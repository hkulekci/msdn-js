## [message Property (Error) (JavaScript)](message-Property__Error.html)

### Introduction 

 Returns an error message string.

### Syntax 

```
errorObj .message
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">errorObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Instance of <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> object.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="message"><span class="keyword">message</span></span> property returns a string that contains an error message associated with a specific error.
  </p>
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="description"><span class="keyword">description</span></span> and <span sdata="langKeyword" value="message"><span class="keyword">message</span></span>
    properties provide the same functionality. The <span sdata="langKeyword" value="description"><span class="keyword">description</span></span> property provides backwards compatibility; the
    <span sdata="langKeyword" value="message"><span class="keyword">message</span></span> property complies with the ECMA standard.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example causes a TypeError exception to be thrown and displays the name of the error and its message.
</p>

```
try { // Cause an error. var x = y; } catch(e) { document.write ("Error Message: " + e.message); document.write ("&lt;br /&gt;"); document.write ("Error Code: "); document.write (e.number &amp;
0xFFFF) document.write ("&lt;br /&gt;"); document.write ("Error Name: " + e.name); }
```

<p xmlns:util="util">
  The output of this code is as follows.
</p>

```
Error Message: 'y' is undefined Error Code: 5009 Error Name: TypeError
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
    <span sdata="link" xmlns:util="util"><a href="94df2d6b-f1a1-4931-a956-0a930cb87f76.htm">name Property (Error) (JavaScript)</a></span>
  </div>
</div>

