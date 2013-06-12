---
title: valueOf Method (Object) (JavaScript)
isChild: false
---

## valueOf Method (Object) (JavaScript) {valueof_method_object_javascript_title}

### Introduction 

 Returns the primitive value of the specified object.

### Syntax 

```
object .valueOf( )
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">object</span> reference is any intrinsic JavaScript object.
  </p>
  <p xmlns:util="util">
    The <b>valueOf</b> method is defined differently for each intrinsic JavaScript object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Object
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Return Value
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Array
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the array instance.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Boolean
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The Boolean value.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Date
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The stored time value in milliseconds since midnight, January 1, 1970 UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The function itself.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Number
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The numeric value.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The object itself. This is the default.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            String
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The string value.
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    The <b>Math</b> and <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> objects do not have a <b>valueOf</b> method.
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
    <b>Applies To</b>: <span sdata="link"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>| <span sdata="link"><a href=
    "d67748f2-7bf5-4889-8269-e777616cc5f0.htm">Boolean Object (JavaScript)</a></span>| <span sdata="link"><a href="ce2202bb-7ec9-4f5a-bf48-3a04feff283e.htm">Date Object (JavaScript)</a></span>|
    <span sdata="link"><a href="d3834767-203c-475e-848c-95c423ba15b6.htm">Function Object (JavaScript)</a></span>| <span sdata="link"><a href="76e87c37-cf6c-46cc-bafa-04be1fe3d78d.htm">Number Object
    (JavaScript)</a></span>| <span sdata="link"><a href="d24ef8fc-217b-4828-94e1-19f72780bae0.htm">Object Object (JavaScript)</a></span>| <span sdata="link"><a href=
    "8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="c4ae9da2-60c9-486f-b00a-9df03fda4a35.htm">toString Method (Object) (JavaScript)</a></span>
  </div>
</div>

