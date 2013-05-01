## [Object.defineProperties Function (JavaScript)](Object.defineProperties-Function.html)

### Introduction 

 Adds one or more properties to an object, and/or modifies attributes of existing properties.

### Syntax 

```
object .defineProperties(object , descriptors )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The object on which to add or modify the properties. This can be a native JavaScript object or a DOM object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">descriptors</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A JavaScript object that contains one or more descriptor objects. Each descriptor object describes a data property or an accessor property.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The object that was passed to the function.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">descriptors</span> argument is an object that contains one or more descriptor objects.
  </p>
  <p xmlns:util="util">
    A <span class="term">data property</span> is a property that can store and retrieve a value. A data property descriptor contains a <span sdata="langKeyword" value="value"><span class=
    "keyword">value</span></span> attribute, a <span sdata="langKeyword" value="writable"><span class="keyword">writable</span></span> attribute, or both. For more information, see <span sdata=
    "link">Data Properties and Accessor Properties</span>.
  </p>
  <p xmlns:util="util">
    An <span class="term">accessor property</span> calls a user-provided function every time the property value is set or retrieved. An accessor property descriptor contains a <span sdata=
    "langKeyword" value="set"><span class="keyword">set</span></span> attribute, a <span sdata="langKeyword" value="get"><span class="keyword">get</span></span> attribute, or both.
  </p>
  <p xmlns:util="util">
    If the object already has a property that has the specified name, the property attributes are modified. For more information, see <span sdata="link"><a href=
    "c5d05346-940a-40c2-b12a-e8b25abc8d46.htm">Object.defineProperty Function (JavaScript)</a></span>.
  </p>
  <p xmlns:util="util">
    To create an object and add properties to the new object, you can use the <span sdata="link"><a href="0ad31f36-a9ee-444e-b0fe-c87843d03196.htm">Object.create Function (JavaScript)</a></span>.
  </p>
</div>

#### Adding Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    In the following example, the <b>Object.defineProperties</b> function adds a data property and an accessor property to a user-defined object.
  </p>
  <p xmlns:util="util">
    The example uses an object literal to create the <span class="parameter" sdata="paramReference">descriptors</span> object with the <span class="code">newDataProperty</span> and <span class=
    "code">newAccessorProperty</span> descriptor objects.
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
 var newLine = "&lt;br /&gt;";  var obj = {}; Object.defineProperties(obj, {     newDataProperty: {         value: 101,         writable: true,         enumerable: true,         configurable: true     },     newAccessorProperty: {         set: function (x) {             document.write("in property set accessor" + newLine);             this.newaccpropvalue = x;         },         get: function () {             document.write("in property get accessor" + newLine);             return this.newaccpropvalue;         },         enumerable: true,         configurable: true     }});  // Set the accessor property value. obj.newAccessorProperty = 10; document.write ("newAccessorProperty value: " + obj.newAccessorProperty + newLine);  // Output: // in property set accessor // in property get accessor // newAccessorProperty value: 10 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    Like the earlier example, the following example adds properties dynamically instead of with an object literal.
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
 var newLine = "&lt;br /&gt;";  // Create the descriptors object. var descriptors = new Object();  // Add a data property descriptor to the descriptors object. descriptors.newDataProperty = new Object(); descriptors.newDataProperty.value = 101; descriptors.newDataProperty.writable = true; descriptors.newDataProperty.enumerable = true; descriptors.newDataProperty.configurable = true;  // Add an accessor property descriptor to the descriptors object. descriptors.newAccessorProperty = new Object(); descriptors.newAccessorProperty.set = function (x) {     document.write("in property set accessor" + newLine);     this.newaccpropvalue = x; }; descriptors.newAccessorProperty.get = function () {     document.write("in property get accessor" + newLine);     return this.newaccpropvalue; }; descriptors.newAccessorProperty.enumerable = true; descriptors.newAccessorProperty.configurable = true;  // Call the Object.defineProperties function. var obj = new Object(); Object.defineProperties(obj, descriptors);  // Set the accessor property value. obj.newAccessorProperty = 10; document.write ("newAccessorProperty value: " + obj.newAccessorProperty + newLine);  // Output: // in property set accessor // in property get accessor // newAccessorProperty value: 10 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Modifying Properties 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util"></p>
  <p xmlns:util="util">
    To modify property attributes for the object, add the following code. The <b>Object.defineProperties</b> function modifies the <span sdata="langKeyword" value="writable"><span class=
    "keyword">writable</span></span> attribute of <span class="code">newDataProperty</span>, and modifies the <span sdata="langKeyword" value="enumerable"><span class=
    "keyword">enumerable</span></span> attribute of <span class="code">newAccessorProperty</span>. It adds <span class="code">anotherDataProperty</span> to the object because that property name does
    not already exist.
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          &nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
     Object.defineProperties(obj, {         newDataProperty: { writable: false },         newAccessorProperty: { enumerable: false },         anotherDataProperty: { value: "abc" }     }); 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in Internet Explorer 9 standards, Internet Explorer 10 standards, and Windows Store apps. Supported in Internet Explorer 8 for DOM objects only, otherwise not supported.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8f0e1c90-c4f9-44c4-bf76-726bacecbc14.htm">Object.getOwnPropertyDescriptor Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="59f4b6b1-02be-44b3-a06c-a5ca8f70c3d8.htm">Object.getOwnPropertyNames Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="c5d05346-940a-40c2-b12a-e8b25abc8d46.htm">Object.defineProperty Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="0ad31f36-a9ee-444e-b0fe-c87843d03196.htm">Object.create Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d24ef8fc-217b-4828-94e1-19f72780bae0.htm">Object Object (JavaScript)</a></span>
  </div>
</div>

