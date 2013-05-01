## [setYear Method (Date) (JavaScript)](setYear-Method__Date.html)

### Introduction 

 Sets the year value in the Date object.

### Syntax 

```
dateObj .setYear(numYear )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">dateObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numYear</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. For the years 1900 through 1999, this is a numeric value equal to the year minus 1900. For dates outside that range, this is a 4-digit numeric value.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    This method is obsolete, and is maintained for backwards compatibility only. Use the <b>setFullYear</b> method instead.
  </p>
  <p xmlns:util="util">
    To set the year of a <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object to 1997, call <b>setYear(97)</b>. To set the year to 2010, call <b>setYear(2010)</b>.
    Finally, to set the year to a year in the range 0-99, use the <b>setFullYear</b> method.
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
            For JavaScript version 1.0, <b>setYear</b> uses a value that is the result of the addition of 1900 to the year value provided by <span class="parameter" sdata=
            "paramReference">numYear</span>, regardless of the value of the year. For example, to set the year to 1899 <span class="parameter" sdata="paramReference">numYear</span> is -1 and to set
            the year 2000 <span class="parameter" sdata="paramReference">numYear</span> is 100.
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
    <span sdata="link" xmlns:util="util"><a href="0e23e832-acd4-49a9-a175-515d0094f172.htm">getYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="635e4f5a-0210-4c01-8152-b0da4146f6ff.htm">setFullYear Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e6c51b49-0149-4f9a-aa74-c73c0306f98e.htm">setUTCFullYear Method (Date) (JavaScript)</a></span>
  </div>
</div>

