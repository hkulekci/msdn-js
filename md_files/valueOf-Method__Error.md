## [valueOf Method (Error)](valueOf-Method__Error.html)

### Introduction 

 Returns the string value of an error.

### Syntax 

```
error .valueOf()
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">error</span> object is any instance of an Error.
  </p>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The string "Error: " plus the error message.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>valueOF</b> method with a date.
</p>

```
var myError = new Error(); myError.message = "This is an error."; var value = myError.valueOf(); document.write(value); // Output: Error: This is an error.
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

