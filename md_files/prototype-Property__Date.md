## [prototype Property (Date)](prototype-Property__Date.html)

### Introduction 

 Returns a reference to the prototype for a date.

### Syntax 

```
date .prototype
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">date</span> argument is the name of an object.
  </p>
  <p xmlns:util="util">
    Use the <b>prototype</b> property to provide a base set of functionality to a Date. New instances of an object "inherit" the behavior of the prototype assigned to that object.
  </p>
  <p xmlns:util="util">
    For example, to add a method to the <b>Date</b> object that returns the value of the largest element of the array, declare the function, add it to <b>Date.prototype</b>, and then use it.
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
 function max( ){     var max = new Date();     max.setFullYear(2200, 01, 01);     return max; } Date.prototype.maxDate = max; var myDate = new Date();  if (myDate &lt; myDate.maxDate())     document.write("today isn't the max"); else if (myDate == myDate.maxDate())     document.write("today is the max");   // Output: // today isn't the max 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    All intrinsic JavaScript objects have a <b>prototype</b> property that is read-only. Properties and methods may be added to the prototype, but the object may not be assigned a different
    prototype. However, user-defined objects may be assigned a new prototype.
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

