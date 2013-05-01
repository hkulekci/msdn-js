## [Object.getPrototypeOf Function (JavaScript)](Object.getPrototypeOf-Function.html)

### Introduction 

 Returns the prototype of an object.

### Syntax 

```
Object.getPrototypeOf(object )
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The object that references the prototype.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The prototype of the <span class="parameter" sdata="paramReference">object</span> argument. The prototype is also an object.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the <span class="parameter" sdata="paramReference">object</span> argument is not an object, a <span sdata="langKeyword" value="TypeError"><span class="keyword">TypeError</span></span>
    exception is thrown.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>Object.getPrototypeOf</b> function.
</p>

```
// Create a constructor function. function Pasta(grain, width) { this.grain = grain; this.width = width; } // Create an object from the pasta constructor. var spaghetti = new Pasta("wheat", 0.2); //
Obtain the prototype from the object. var proto = Object.getPrototypeOf(spaghetti); // Add a property to the prototype and validate that // the original object has the property. proto.foodgroup =
"carbohydrates"; document.write(spaghetti.foodgroup + " "); // Verify that the prototype obtained from the object // is the same as the prototype of the constructor. var result = (proto ===
Pasta.prototype); document.write(result + " "); // Verify that prototype obtained from the object // is a prototype of the original object. var result = proto.isPrototypeOf(spaghetti);
document.write(result); // Output: carbohydrates true true
```

<p xmlns:util="util">
  The following example uses the <b>Object.getPrototypeOf</b> function to validate data types.
</p>

```
var reg = /a/; var result = (Object.getPrototypeOf(reg) === RegExp.prototype); document.write(result + " "); var err = new Error("an error"); var result = (Object.getPrototypeOf(err) ===
Error.prototype); document.write(result); // Output: true true
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Internet Explorer 9 standards and Internet Explorer 10 standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards.
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
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="9c821319-c208-480f-915e-565ef6e017b6.htm">isPrototypeOf Method (Object) (JavaScript)</a></span>
  </div>
</div>

