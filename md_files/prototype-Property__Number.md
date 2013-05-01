## [prototype Property (Number)](prototype-Property__Number.html)

### Introduction 

 Returns a reference to the prototype for a class of number.

### Syntax 

```
number .prototype
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">number</span> argument is the name of a number.
  </p>
  <p xmlns:util="util">
    Use the <b>prototype</b> property to provide a base set of functionality to a class of objects. New instances of an object "inherit" the behavior of the prototype assigned to that object.
  </p>
  <p xmlns:util="util">
    For example, to add a method to the <b>Number</b> object that returns the number of (integer) digits, declare the function, add it to <b>Number.prototype</b>, and then use it.
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
 function number_digits() {     var digits = 0;     var num = this;     while (num) &gt;= 1) {         digits++;         num /= 10;     }     return digits; }  Number.prototype.digits = number_digits; var myNumber = new Number(3456.789); document.write(myNumber.digits()); // Output: // 4 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    All intrinsic JavaScript objects have a <b>prototype</b> property that is read-only. Properties and methods may be added to the prototype, but the object may not be assigned a different
    prototype. However, user-defined objects may be assigned a new prototype.
  </p>
  <p xmlns:util="util">
    The method and property lists for each intrinsic object in this language reference indicate which ones are part of the object's prototype, and which are not.
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

