---
title: toLocaleString Method (Object) (JavaScript)
---

### Introduction 

 Returns a date converted to a string using the current locale.

### Syntax 

```
dateObj .toLocaleString()
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">dateObj</span> is any <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
  </p>
  <p xmlns:util="util">
    The <b>toLocaleString</b> method returns a <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object that contains the date written in the current locale's long
    default format.
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        For dates between 1601 and 1999 A.D., the date is formatted according to the user's Control Panel Regional Settings.
      </p>
    </li>
    <li>
      <p>
        For dates outside this range, the default format of the <b>toString</b> method is used.
      </p>
    </li>
  </ul>
  <p xmlns:util="util">
    For example, in the United States, <b>toLocaleString</b> returns "01/05/96 00:00:00" for January 5. In Europe, it returns "05/01/96 00:00:00" for the same date, as European convention puts the
    day before the month.
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
            <b>toLocaleString</b> should only be used to display results to a user; it should never be used as the basis for computation within a script as the returned result is machine-specific.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>toLocaleString</b> method.
</p>

```
function toLocaleStrDemo(){ var d, s; //Declare variables. d = new Date(); //Create Date object. s = "Current setting is "; s += d.toLocaleString() ; //Convert to current locale. return(s); //Return
converted date }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>| <span sdata="link"><a href=
    "ce2202bb-7ec9-4f5a-bf48-3a04feff283e.htm">Date Object (JavaScript)</a></span>| <span sdata="link"><a href="76e87c37-cf6c-46cc-bafa-04be1fe3d78d.htm">Number Object (JavaScript)</a></span>|
    <span sdata="link"><a href="d24ef8fc-217b-4828-94e1-19f72780bae0.htm">Object Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="0b83715c-8ced-4bd7-8940-a8007d002d10.htm">toLocaleDateString Method (Date) (JavaScript)</a></span>
  </div>
</div>

