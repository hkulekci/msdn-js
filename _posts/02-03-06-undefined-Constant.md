---
title: undefined Constant (JavaScript)
---

### Introduction 

 A value that has never been defined, such as a variable that has not been initialized.

### Syntax 

```
undefined
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>undefined</b> constant is a member of the <b>Global</b> object, and becomes available when the scripting engine is initialized. When a variable has been declared but not initialized, its
    value is <b>undefined</b>.
  </p>
  <p xmlns:util="util">
    If a variable has not been declared, you cannot compare it to <b>undefined</b>, but you can compare the type of the variable to the string "undefined".
  </p>
  <p xmlns:util="util">
    The <b>undefined</b> constant is useful when explicitly testing or setting a variable to undefined.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>undefined</b> constant.
</p>

```
// A variable that has not been initialized. var declared; if (declared == undefined) document.write("declared has not been given a value &lt;br/&gt;"); else document.write("declared has been given a
value &lt;br/&gt;"); document.write("typeof declared is " + typeof(declared) + "&lt;br/&gt;"); // An undeclared variable cannot be compared to undefined, // so the next line would generate an error.
// if (notDeclared == undefined); document.write("typeof notDeclared is " + typeof(notDeclared)); // Output: // declared has not been given a value // typeof declared is undefined // typeof
notDeclared is undefined
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>undefined</b> property was introduced in Internet Explorer before Internet Explorer 6, and was made read-only in Internet Explorer 9 standards mode.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="81a40cad-9354-4e38-8ad0-83fc4257baee.htm">Global Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ee8a1036-119f-486f-b034-b07bdba87f0c.htm">typeof Operator (JavaScript)</a></span>
  </div>
</div>

