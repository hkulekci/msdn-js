---
title: getYear Method (Date) (JavaScript)
---

### Introduction 

 Gets the year of a Date object.

### Syntax 

```
dateObj .getYear()
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">dateObj</span> reference is a <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns the year.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <div class="alert">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th align="left">
          <img class="note" alt="Important note" title="Important note" src="../icons/alert_caution.gif" /><b>Important</b>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            This method is obsolete, and is provided for backward compatibility only. Use the <b>getFullYear</b> method instead.
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    In Internet Explorer 3.0, and then in Internet Explorer versions starting with Internet Explorer 9 standards mode, the value returned is the stored year minus 1900. For example, the year 1899 is
    returned as -1 and the year 2000 is returned as 100.
  </p>
  <p xmlns:util="util">
    In Internet Explorer 4.0 through Internet Explorer 8 standards mode, the formula depends on the year. For the years 1900 through 1999, the value returned is a 2-digit value that is the stored
    year minus 1900. For dates outside that range, the 4-digit year is returned. For example, 1996 is returned as 96, but 1825 and 2025 are returned as is.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="ce2202bb-7ec9-4f5a-bf48-3a04feff283e.htm">Date Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="f9ec1262-02e9-4791-90b5-48f33b1dc4bc.htm">getFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="f11e5363-ef8a-48dd-9d56-4ee7290c7c48.htm">getUTCFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="635e4f5a-0210-4c01-8152-b0da4146f6ff.htm">setFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e6c51b49-0149-4f9a-aa74-c73c0306f98e.htm">setUTCFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="36431050-e0ec-45ee-830d-0d7c20e207ea.htm">setYear Method (Date) (JavaScript)</a></span>
  </div>
</div>

