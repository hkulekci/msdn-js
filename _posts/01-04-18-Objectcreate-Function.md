---
title: Object.create Function (JavaScript)
---

### Introduction 

 Creates an object that has the specified prototype, and that optionally contains specified properties.

### Syntax 

```
Object.create(prototype , descriptors )
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">prototype</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The object to use as a prototype. May be <span sdata="langKeyword" value="null"><span class="keyword">null</span></span>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">descriptors</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A JavaScript object that contains one or more property descriptors.
      </p>
      <p xmlns:util="util">
        A <span class="term">data property</span> is a property that can get and set a value. A data property descriptor contains a <span sdata="langKeyword" value="value"><span class=
        "keyword">value</span></span> attribute, plus <span sdata="langKeyword" value="writable"><span class="keyword">writable</span></span>, <span sdata="langKeyword" value=
        "enumerable"><span class="keyword">enumerable</span></span>, and <span sdata="langKeyword" value="configurable"><span class="keyword">configurable</span></span> attributes. If the last three
        attributes are not specified, they default to <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>. An <span class="term">accessor property</span> calls a
        user-provided function every time the value is retrieved or set. An accessor property descriptor contains a <span sdata="langKeyword" value="set"><span class="keyword">set</span></span>
        attribute, a <span sdata="langKeyword" value="get"><span class="keyword">get</span></span> attribute, or both. For more information, see <span sdata="link"><a href=
        "c5d05346-940a-40c2-b12a-e8b25abc8d46.htm">Object.defineProperty Function (JavaScript)</a></span>.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    A new object that has the specified internal prototype and contains the specified properties, if any.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    A <span sdata="langKeyword" value="TypeError"><span class="keyword">TypeError</span></span> exception is thrown if any of the following conditions is true:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        The <span class="parameter" sdata="paramReference">prototype</span> argument is not an object and is not <span sdata="langKeyword" value="null"><span class="keyword">null</span></span>.
      </p>
    </li>
    <li>
      <p>
        A descriptor in the <span class="parameter" sdata="paramReference">descriptors</span> argument has a <span sdata="langKeyword" value="value"><span class="keyword">value</span></span> or
        <span sdata="langKeyword" value="writable"><span class="keyword">writable</span></span> attribute, and has a <span sdata="langKeyword" value="get"><span class="keyword">get</span></span> or
        <span sdata="langKeyword" value="set"><span class="keyword">set</span></span> attribute.
      </p>
    </li>
    <li>
      <p>
        A descriptor in the <span class="parameter" sdata="paramReference">descriptors</span> argument has a <span sdata="langKeyword" value="get"><span class="keyword">get</span></span> or
        <span sdata="langKeyword" value="set"><span class="keyword">set</span></span> attribute that is not a function.
      </p>
    </li>
  </ul>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You can use this function using a <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> <span class="parameter" sdata="paramReference">prototype</span> parameter in
    order to stop the prototype chain. The object created will have no prototype.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example creates an object using a <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> prototype and adds two enumerable properties.
</p>

```
var newObj = Object.create(null, { size: { value: "large", enumerable: true }, shape: { value: "round", enumerable: true } }); document.write(newObj.size + "&lt;br/&gt;"); document.write(newObj.shape
+ "&lt;br/&gt;"); document.write(Object.getPrototypeOf(newObj)); // Output: // large // round // null
```

<p xmlns:util="util">
  The following example creates an object that has the same internal prototype as the Object object. You can see that it has the same prototype as an object created by using an object literal. The
  Object.getPrototypeOf function gets the prototype of the original object. To get the object's property descriptor, you can use <span sdata="link"><a href=
  "8f0e1c90-c4f9-44c4-bf76-726bacecbc14.htm">Object.getOwnPropertyDescriptor Function (JavaScript)</a></span>.
</p>

```
var firstLine = { x: undefined, y: undefined }; var secondLine = Object.create(Object.prototype, { x: { value: undefined, writable: true, configurable: true, enumerable: true }, y: { value:
undefined, writable: true, configurable: true, enumerable: true } }); var firstLine = { x: undefined, y: undefined }; var secondLine = Object.create(Object.prototype, { x: { value: undefined,
writable: true, configurable: true, enumerable: true }, y: { value: undefined, writable: true, configurable: true, enumerable: true } }); document.write("first line prototype = " +
Object.getPrototypeOf(firstLine)); document.write("&lt;br/&gt;"); document.write("second line prototype = " + Object.getPrototypeOf(secondLine)); // Output: // first line prototype = [object Object]
// second line prototype = [object Object]
```

<p xmlns:util="util">
  The following example creates an object that has the same internal prototype as the Shape object.
</p>

```
// Create the shape object. var Shape = { twoDimensional: true, color: undefined, hasLineSegments: undefined }; var Square = Object.create(Object.getPrototypeOf(Shape));
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
    <span sdata="link" xmlns:util="util"><a href="1c59cd7a-a7e2-4c5c-83ec-e6bd2b104d9f.htm">Object.getPrototypeOf Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="9c821319-c208-480f-915e-565ef6e017b6.htm">isPrototypeOf Method (Object) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Creating Your Own Objects (Windows Scripting - JScript)</span>
  </div>
</div>

