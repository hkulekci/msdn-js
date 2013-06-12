---
title: encodeURI Function (JavaScript)
---

### Introduction 

 Encodes a text string as a valid Uniform Resource Identifier (URI)

### Syntax 

```
encodeURI(URIString )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">URIString</span> argument is a value representing an encoded URI.
  </p>
  <p xmlns:util="util">
    The <b>encodeURI</b> function returns an encoded URI. If you pass the result to <b>decodeURI</b>, the original string is returned. The <b>encodeURI</b> function does not encode the following
    characters: ":", "/", ";", and "?". Use <b>encodeURIComponent</b> to encode these characters.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code first encodes and then decodes a URI.
</p>

```
var uriEncode = encodeURI ("http://www.Not a URL.com"); var uriDecode = decodeURIComponent(uriEncode); document.write(uriEncode); document.write("&lt;br/&gt;"); document.write(uriDecode); // Output:
// http://www.Not%20a%20URL.com // http://www.Not a URL.com
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
    <span sdata="link" xmlns:util="util"><a href="486ccee2-afd7-4863-97ce-4adb50cf39c0.htm">decodeURIComponent Function (JavaScript)</a></span>
  </div>
</div>

