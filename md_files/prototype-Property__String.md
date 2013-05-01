## [prototype Property (String)](prototype-Property__String.html)

### Introduction 

 Returns a reference to the prototype for a class of string.

### Syntax 

```
string .prototype
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">string</span> argument is the name of a string.
  </p>
  <p xmlns:util="util">
    Use the <b>prototype</b> property to provide a base set of functionality to a class of objects. New instances of an object "inherit" the behavior of the prototype assigned to that object.
  </p>
  <p xmlns:util="util">
    For example, to add a method to the <b>String</b> object that returns the value of the last element of the string, declare the function, add it to <b>String.prototype</b>, and then use it.
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
 function string_last( ){     return this.charAt(this.length - 1); } String.prototype.last = string_last; var myString = new String("every good boy does fine"); document.write(myString.last());  // Output: // e 
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

