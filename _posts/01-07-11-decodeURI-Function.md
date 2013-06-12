---
title: decodeURI Function (JavaScript)
---

### Introduction 

 Gets the unencoded version of an encoded Uniform Resource Identifier (URI).

### Syntax 

```
decodeURI(URIstring )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">URIstring</span> argument is a value representing an encoded URI.
  </p>
  <p xmlns:util="util">
    Use the <b>decodeURI</b> function instead of the deprecated <b>unescape</b> function.
  </p>
  <p xmlns:util="util">
    The <b>decodeURI</b> function returns a string value.
  </p>
  <p xmlns:util="util">
    If the <span class="parameter" sdata="paramReference">URIString</span> is not valid, a URIError occurs.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="81a40cad-9354-4e38-8ad0-83fc4257baee.htm">Global Object (JavaScript)</a></span>
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code first encodes a URI component and then decodes it.
</p>

```
var uriEncode = encodeURIComponent ("www.Not a URL.com"); var uriDecode = decodeURIComponent(uriEncode); document.write (uriEncode); document.write ("&lt;br/&gt;"); document.write (uriDecode); //
Output: // www.Not%20a%20URL.com // www.Not a URL.com
```

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
    <span sdata="link" xmlns:util="util"><a href="486ccee2-afd7-4863-97ce-4adb50cf39c0.htm">decodeURIComponent Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="17bab5a2-bcd4-46c2-8b52-b2b5a0ed98a3.htm">encodeURI Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="81a40cad-9354-4e38-8ad0-83fc4257baee.htm">Global Object (JavaScript)</a></span>
  </div>
</div>

