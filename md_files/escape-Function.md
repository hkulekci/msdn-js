---
title: escape Function (JavaScript)
isChild: false
---

## escape Function (JavaScript) {escape_function_javascript_title}

### Introduction 

 Encodes strings so they can be read on all computers. Deprecated.

### Syntax 

```
escape(charString )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">charString</span> argument is any <b>String</b> object or literal to be encoded.
  </p>
  <p xmlns:util="util">
    The <b>escape</b> function returns a string value (in Unicode format) that contains the contents of <span class="parameter" sdata="paramReference">charstring</span>. All spaces, punctuation,
    accented characters, and any other non-ASCII characters are replaced with <span sdata="langKeyword" value="%"><span class="keyword">%</span></span><i>xx</i> encoding, where <i>xx</i> is
    equivalent to the hexadecimal number representing the character. For example, a space is returned as "%20."
  </p>
  <p xmlns:util="util">
    Characters with a value greater than 255 are stored using the <b>%u</b><i>xxxx</i> format.
  </p>
  <div class="alert">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th align="left">
          <img class="note" alt="Note" title="Note" src="../icons/alert_note.gif" /><b>Note</b>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            The <b>escape</b> function should not be used to encode Uniform Resource Identifiers (URI). Use <b>encodeURI</b> and <b>encodeURIComponent</b> functions instead.
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="81a40cad-9354-4e38-8ad0-83fc4257baee.htm">Global Object (JavaScript)</a></span>
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
    <span sdata="link" xmlns:util="util"><a href="17bab5a2-bcd4-46c2-8b52-b2b5a0ed98a3.htm">encodeURI Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8202bce6-1342-40dc-a5ef-ac6d210a7d15.htm">encodeURIComponent Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4adf0270-88b5-4d54-8110-d879d6ae97c2.htm">unescape Function (JavaScript)</a></span>
  </div>
</div>

