---
title: delete Operator (JavaScript)
isChild: false
---

## delete Operator (JavaScript) {delete_operator_javascript_title}

### Introduction 

 Deletes a property from an object, or removes an element from an array.

### Syntax 

```
delete expression
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">expression</span> argument is a valid JavaScript expression that usually results in a property name or array element.
  </p>
  <p xmlns:util="util">
    If the result of <span class="parameter" sdata="paramReference">expression</span> is an object, the property specified in <span class="parameter" sdata="paramReference">expression</span> exists,
    and the object will not allow it to be deleted, <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> is returned.
  </p>
  <p xmlns:util="util">
    In all other cases, <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> is returned.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to remove an element from an array.
</p>

```
// Create an array. var ar = new Array (10, 11, 12, 13, 14); // Remove an element from the array. delete ar[1]; // Print the results. document.write ("element 1: " + ar[1]); document.write ("&lt;br
/&gt;"); document.write ("array: " + ar); // Output: // element 1: undefined // array: 10,,12,13,14
```

<p xmlns:util="util">
  The following example shows how to delete properties from an object.
</p>

```
// Create an object and add expando properties. var myObj = new Object(); myObj.name = "Fred"; myObj.count = 42; // Delete the properties from the object. delete myObj.name; delete myObj["count"]; //
Print the results. document.write ("name: " + myObj.name); document.write ("&lt;br /&gt;"); document.write ("count: " + myObj.count); // Output: // name: undefined // count: undefined
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

