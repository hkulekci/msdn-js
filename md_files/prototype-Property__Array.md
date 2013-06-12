---
title: prototype Property (Array)
isChild: false
---

## prototype Property (Array) {prototype_property_array_title}

### Introduction 

 Returns a reference to the prototype for a class of array.

### Syntax 

```
array .prototype
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">array</span> argument is the name of an array.
  </p>
  <p xmlns:util="util">
    Use the <b>prototype</b> property to provide a base set of functionality to a class of objects. New instances of an object "inherit" the behavior of the prototype assigned to that object.
  </p>
  <p xmlns:util="util">
    For example, to add a method to the <b>Array</b> object that returns the value of the largest element of the array, declare the function, add it to <b>Array.prototype</b>, and then use it.
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
 function array_max( ){     var i, max = this[0];     for (i = 1; i &lt; this.length; i++)     {     if (max &lt; this[i])     max = this[i];     }     return max; } Array.prototype.max = array_max; var myArray = new Array(7, 1, 3, 11, 25, 9 ); document.write(myArray.max());  // Output: 25 
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

