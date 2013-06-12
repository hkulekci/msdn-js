---
title: decodeURIComponent Function (JavaScript)
isChild: false
---

## decodeURIComponent Function (JavaScript) {decodeuricomponent_function_javascript_title}

### Introduction 

 Gets the unencoded version of an encoded component of a Uniform Resource Identifier (URI).

### Syntax 

```
decodeURIComponent(encodedURIString )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">encodedURIString</span> argument is a value representing an encoded URI component.
  </p>
  <p xmlns:util="util">
    A URIComponent is part of a complete URI.
  </p>
  <p xmlns:util="util">
    If the <span class="parameter" sdata="paramReference">encodedURIString</span> is not valid, a URIError occurs.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code first encodes and then decodes a URI.
</p>

```
var uriEncode = encodeURI ("http://www.Not a URL.com"); var uriDecode = decodeURIComponent(uriEncode); document.write (uriEncode); document.write("&lt;br/&gt;"); document.write (uriDecode); //
Output: // http://www.Not%20a%20URL.com // http://www.Not a URL.com
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
    <span sdata="link" xmlns:util="util"><a href="af6c81dc-10f4-4243-a7ce-d18ae3ea0fb8.htm">decodeURI Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="17bab5a2-bcd4-46c2-8b52-b2b5a0ed98a3.htm">encodeURI Function (JavaScript)</a></span>
  </div>
</div>

