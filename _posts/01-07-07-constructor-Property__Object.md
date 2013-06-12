---
title: constructor Property (Object) (JavaScript)
---

### Introduction 

 Specifies the function that creates an object.

### Syntax 

```
object .constructor
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">object</span> is the name of an object or function.
  </p>
  <p xmlns:util="util">
    The <b>constructor</b> property is a member of the prototype of every object that has a prototype. This includes all intrinsic JavaScript objects except the <b>Global</b> and <b>Math</b> objects.
    The <b>constructor</b> property contains a reference to the function that constructs instances of that particular object.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the constructor property.
</p>

```
// A constructor function. function MyObj() { this.number = 1; } var x = new String("Hi"); if (x.constructor == String) document.write("Object is a String."); document.write ("&lt;br /&gt;"); var y =
new MyObj; if (y.constructor == MyObj) document.write("Object constructor is MyObj."); // Output: // Object is a String. // Object constructor is MyObj.
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
    <span sdata="link" xmlns:util="util"><a href="9fc434a1-5995-4fcb-a4e8-00e7f615aaa2.htm">prototype Property (Object) (JavaScript)</a></span>
  </div>
</div>

