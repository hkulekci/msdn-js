---
title: Object.defineProperty Function (JavaScript)
isChild: false
---

## Object.defineProperty Function (JavaScript) {objectdefineproperty_function_javascript_title}

### Introduction 

 Adds a property to an object, or modifies attributes of an existing property.

### Syntax 

```
Object.defineProperty(object , propertyname , descriptor )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The object on which to add or modify the property. This can be a native JavaScript object (that is, a user-defined object or a built in object) or a DOM object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">propertyname</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A string that contains the property name.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">descriptor</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A descriptor for the property. It can be for a data property or an accessor property.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The modified object.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You can use the <b>Object.defineProperty</b> function to do the following:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        Add a new property to an object. This occurs when the object does not have the specified property name.
      </p>
    </li>
    <li>
      <p>
        Modify attributes of an existing property. This occurs when the object already has the specified property name.
      </p>
    </li>
  </ul>
  <p xmlns:util="util">
    The property definition is provided in a descriptor object, which describes the attributes of a data property or an accessor property. The descriptor object is a parameter of the
    <b>Object.defineProperty</b> function.
  </p>
  <p xmlns:util="util">
    To add multiple properties to an object, or to modify multiple existing properties, you can use the <span sdata="link"><a href="2dae6658-a1c9-495f-bf06-bb3e964e6762.htm">Object.defineProperties
    Function (JavaScript)</a></span>.
  </p>
</div>

#### Exceptions 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    A <span sdata="langKeyword" value="TypeError"><span class="keyword">TypeError</span></span> exception is thrown if any one of the following conditions is true:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        The <span class="parameter" sdata="paramReference">object</span> argument is not an object.
      </p>
    </li>
    <li>
      <p>
        The object is not extensible and the specified property name does not exist..
      </p>
    </li>
    <li>
      <p>
        The <span class="parameter" sdata="paramReference">descriptor</span> has a <span sdata="langKeyword" value="value"><span class="keyword">value</span></span> or <span sdata="langKeyword"
        value="writable"><span class="keyword">writable</span></span> attribute, and has a <span sdata="langKeyword" value="get"><span class="keyword">get</span></span> or <span sdata="langKeyword"
        value="set"><span class="keyword">set</span></span> attribute.
      </p>
    </li>
    <li>
      <p>
        The <span class="parameter" sdata="paramReference">descriptor</span> has a <span sdata="langKeyword" value="get"><span class="keyword">get</span></span> or <span sdata="langKeyword" value=
        "set"><span class="keyword">set</span></span> attribute that is not a function or undefined.
      </p>
    </li>
    <li>
      <p>
        The specified property name already exists, the existing property has a <span sdata="langKeyword" value="configurable"><span class="keyword">configurable</span></span> attribute of
        <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>, and the <span class="parameter" sdata="paramReference">descriptor</span> contains one or more attributes
        that are different from those in the existing property. However, when the existing property has a <span sdata="langKeyword" value="configurable"><span class=
        "keyword">configurable</span></span> attribute of <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> and a <span sdata="langKeyword" value=
        "writable"><span class="keyword">writable</span></span> attribute of <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>, it is permitted for the <span sdata=
        "langKeyword" value="value"><span class="keyword">value</span></span> or <span sdata="langKeyword" value="writable"><span class="keyword">writable</span></span> attribute to be different.
      </p>
    </li>
  </ul>
</div>

#### Adding a Data Property 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    In the following example, the <b>Object.defineProperty</b> function adds a data property to a user-defined object. To instead add the property to an existing DOM object, uncomment the
    <span class="code">var = window.document</span> line.
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
 var newLine = "&lt;br /&gt;";  // Create a user-defined object. var obj = {};  // Add a data property to the object. Object.defineProperty(obj, "newDataProperty", {     value: 101,     writable: true,     enumerable: true,     configurable: true });  // Set the property value. obj.newDataProperty = 102; document.write("Property value: " + obj.newDataProperty + newLine);  // Output: // Property value: 102 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    To list the object properties, add the following code to this example.
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
 var names = Object.getOwnPropertyNames(obj); for (var i = 0; i &lt; names.length; i++) {     var prop = names[i];      document.write(prop + ': ' + obj[prop]);     document.write(newLine); }  // Output: //  newDataProperty: 102 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Modifying a Data Property 

<div id="sectionSection3" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    To modify a property attribute for the object, add the following code to the <span class="code">addDataProperty</span> function shown earlier. The <span class="parameter" sdata=
    "paramReference">descriptor</span> parameter contains only a <span sdata="langKeyword" value="writable"><span class="keyword">writable</span></span> attribute. The other data property attributes
    remain the same.
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
 // Modify the writable attribute of the property. Object.defineProperty(obj, "newDataProperty", { writable: false });  // List the property attributes by using a descriptor. // Get the descriptor with Object.getOwnPropertyDescriptor. var descriptor = Object.getOwnPropertyDescriptor(obj, "newDataProperty"); for (var prop in descriptor) {     document.write(prop + ': ' + descriptor[prop]);     document.write(newLine); }  // Output // writable: false // value: 102 // configurable: true // enumerable: true 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Adding an Accessor Property 

<div id="sectionSection4" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    In the following example, the <b>Object.defineProperty</b> function adds an accessor property to a user-defined object.
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
 var newLine = "&lt;br /&gt;";  // Create a user-defined object. var obj = {};  // Add an accessor property to the object. Object.defineProperty(obj, "newAccessorProperty", {     set: function (x) {         document.write("in property set accessor" + newLine);         this.newaccpropvalue = x;     },     get: function () {         document.write("in property get accessor" + newLine);         return this.newaccpropvalue;     },     enumerable: true,     configurable: true });  // Set the property value. obj.newAccessorProperty = 30; document.write("Property value: " + obj.newAccessorProperty + newLine);  // Output: // in property set accessor // in property get accessor // Property value: 30 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    To list the object properties, add the following code to this example.
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
 var names = Object.getOwnPropertyNames(obj); for (var i = 0; i &lt; names.length; i++) {     var prop = names[i];      document.write(prop + ': ' + obj[prop]);     document.write(newLine); } // Output: // in property get accessor // newAccessorProperty: 30 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Modifying an Accessor Property 

<div id="sectionSection5" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    To modify a property attribute for the object, add the following code to the code shown earlier. The <span class="parameter" sdata="paramReference">descriptor</span> parameter contains only a
    <span sdata="langKeyword" value="get"><span class="keyword">get</span></span> accessor definition. The other property attributes remain the same.
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
 // Modify the get accessor. Object.defineProperty(obj, "newAccessorProperty", {     get: function () { return this.newaccpropvalue; } });  // List the property attributes by using a descriptor. // Get the descriptor with Object.getOwnPropertyDescriptor. var descriptor = Object.getOwnPropertyDescriptor(obj, "newAccessorProperty"); for (var prop in descriptor) {     document.write(prop + ': ' + descriptor[prop]);     document.write(newLine); }  // Output: // get: function () { return this.newaccpropvalue; } // set: function (x) { document.write("in property set accessor" + newLine); this.newaccpropvalue = x; } // configurable: true // enumerable: true 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Modifying a Property on a DOM Element 

<div id="sectionSection6" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following example demonstrates how to customize built-in DOM properties by using the <b>Object.getOwnPropertyDescriptor</b> function to get and modify the property's property descriptor. For
    this example, there must by a DIV element with an ID of "div".
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
 // Get the querySelector property descriptor. var descriptor = Object.getOwnPropertyDescriptor(Element.prototype, "querySelector");  // Make the property read-only. descriptor.value = "query"; descriptor.writable = false; // Apply the changes to the Element prototype. Object.defineProperty(Element.prototype, "querySelector", descriptor);  // Get a DOM element from the HTML body. var elem = document.getElementById("div");  // Attempt to change the value. This causes the revised value attribute to be called. elem.querySelector = "anotherQuery"; document.write(elem.querySelector);  // Output: // query 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Internet Explorer 9 standards mode and Internet Explorer 10 standards mode, as well as Windows Store apps, support all features.
  </p>
  <p xmlns:util="util">
    Internet Explorer 8 standards mode supports DOM objects but not user-defined objects. The <span sdata="langKeyword" value="enumerable"><span class="keyword">enumerable</span></span> and
    <span sdata="langKeyword" value="configurable"><span class="keyword">configurable</span></span> attributes can be specified, but they are not used.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Reference
  </h4>
  <div class="seeAlsoStyle">
    Document Object Model Prototypes, Part 2: Accessor (getter/setter) Support
  </div>
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="2dae6658-a1c9-495f-bf06-bb3e964e6762.htm">Object.defineProperties Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="0ad31f36-a9ee-444e-b0fe-c87843d03196.htm">Object.create Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8f0e1c90-c4f9-44c4-bf76-726bacecbc14.htm">Object.getOwnPropertyDescriptor Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="59f4b6b1-02be-44b3-a06c-a5ca8f70c3d8.htm">Object.getOwnPropertyNames Function (JavaScript)</a></span>
  </div>
</div>

