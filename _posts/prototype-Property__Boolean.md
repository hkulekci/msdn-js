---
title: prototype Property (Boolean)
isChild: false
---

## prototype Property (Boolean) {prototype_property_boolean_title}

### Introduction 

 Returns a reference to the prototype for a Boolean.

### Syntax 

```
boolean .prototype
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">boolean</span> argument is the name of an object.
  </p>
  <p xmlns:util="util">
    The <b>prototype</b> property provides a base set of functionality to a class of objects. New instances of an object "inherit" the behavior of the prototype assigned to that object. Properties
    and methods may be added to the prototype, but builtin objects may not be assigned a different prototype.
  </p>
  <p xmlns:util="util">
    For example, to add a method to the <b>Boolean</b> object that returns the value of the largest element of the array, declare the function, add it to <b>Array.prototype</b>, and then use it.
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
 function isFalse( ){     if (this.toString() == "false")          return true;     else         return false; } Boolean.prototype.isFalse = isFalse; var bool = new Boolean(1); document.write(bool.isFalse());  // Output: // false 
</pre>
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
</div>

