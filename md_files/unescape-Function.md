## [unescape Function (JavaScript)](unescape-Function.html)

### Introduction 

 Decodes String objects encoded with the escape function. Deprecated.

### Syntax 

```
unescape(charString )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">charString</span> argument is a <b>String</b> object or literal to be decoded.
  </p>
  <p xmlns:util="util">
    The <b>unescape</b> function returns a string value that contains the contents of <span class="parameter" sdata="paramReference">charstring</span>. All characters encoded with the %<i>xx</i>
    hexadecimal form are replaced by their ASCII character set equivalents.
  </p>
  <p xmlns:util="util">
    Characters encoded in <b>%u</b><i>xxxx</i> format (Unicode characters) are replaced with the Unicode character with hexadecimal encoding <i>xxxx</i>.
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
            The <b>unescape</b> function should not be used to decode Uniform Resource Identifiers (URI). Use <b>decodeURI</b> and <b>decodeURIComponent</b> functions instead.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="81a40cad-9354-4e38-8ad0-83fc4257baee.htm">Global Object (JavaScript)</a></span>
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
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="caa92bea-ba69-4109-a68a-6e2debda463a.htm">escape Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

