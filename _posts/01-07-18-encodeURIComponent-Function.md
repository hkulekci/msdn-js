---
title: encodeURIComponent Function (JavaScript)
---

### Introduction 

 Encodes a text string as a valid component of a Uniform Resource Identifier (URI).

### Syntax 

```
encodeURIComponent(encodedURIString )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">encodedURIString</span> argument is a value representing an encoded URI component.
  </p>
  <p xmlns:util="util">
    The <b>encodeURIComponent</b> function returns an encoded URI. If you pass the result to <b>decodeURIComponent</b>, the original string is returned. Because the <b>encodeURIComponent</b> function
    encodes all characters, be careful if the string represents a path such as <span class="input">/folder1/folder2/default.html</span>. The slash characters will be encoded and will not be valid if
    sent as a request to a web server. Use the <b>encodeURI</b> function if the string contains more than a single URI component.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code first encodes a URI component and then decodes it.
</p>

```
var uriEncode = encodeURIComponent ("www.Not a URL.com"); var uriDecode = decodeURIComponent(uriEncode); document.write(uriEncode); document.write("&lt;br/&gt;"); document.write(uriDecode); //
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
    <span sdata="link" xmlns:util="util"><a href="af6c81dc-10f4-4243-a7ce-d18ae3ea0fb8.htm">decodeURI Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="486ccee2-afd7-4863-97ce-4adb50cf39c0.htm">decodeURIComponent Function (JavaScript)</a></span>
  </div>
</div>

