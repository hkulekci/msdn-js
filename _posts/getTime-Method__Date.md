---
title: getTime Method (Date) (JavaScript)
isChild: false
---

## getTime Method (Date) (JavaScript) {gettime_method_date_javascript_title}

### Introduction 

 Gets the time value in milliseconds.

### Syntax 

```
dateObj .getTime()
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">dateObj</span> reference is a <b>Date</b> object.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Returns the number of milliseconds between midnight, January 1, 1970 and the time value in the <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object. The range of
    dates is approximately 285,616 years from either side of midnight, January 1, 1970. Negative numbers indicate dates prior to 1970.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    When doing multiple date and time calculations, you may want to define variables equal to the number of milliseconds in a day, hour, or minute. For example:
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          JavaScript&nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 var minute = 1000 * 60; var hour = minute * 60; var day = hour * 24; 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    See <span sdata="link">Date and Time Calculations (Windows Scripting - JScript)</span> for more information about how to use the <b>getTime</b> method.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>getTime</b> method.
</p>

```
var minute = 1000 * 60; var hour = minute * 60; var day = hour * 24; date = new Date("1/1/2001"); var time = date.getTime(); document.write(Math.round(time / day) + " days from 1/1/1970 to
1/1/2001"); // Output: 11323 days from 1/1/1970 to 1/1/2001
```

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
    <span sdata="link" xmlns:util="util"><a href="86584748-7219-495b-bf56-e27f5782778c.htm">setTime Method (Date) (JavaScript)</a></span>
  </div>
</div>

