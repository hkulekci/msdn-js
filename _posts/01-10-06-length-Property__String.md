---
title: length Property (String) (JavaScript)
---

### Introduction 

 Returns the length of a String object. Caution JavaScript strings are immutable, so the length of a string cannot be modified.

### Syntax 

```
strVariable .length "String Literal".length
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>length</b> property contains an integer that indicates the number of characters in the <b>String</b> object. The last character in the <b>String</b> object has an index of i<b>length</b> -
    1.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use <b>length</b>. JavaScript strings are immutable and cannot be modified in place. However, you can write the reversed string to an array and then call <b>join</b>
  with the empty character, which produces a string with no separator characters.
</p>

```
var str = "every good boy does fine"; var start = 0; var end = str.length - 1; var tmp = ""; var arr = new Array(end); while (end &gt;= 0) { arr[start++] = str.charAt(end--); } // Join the elements
of the array with a var str2 = arr.join(''); document.write(str2); // Output: enif seod yob doog yreve
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

