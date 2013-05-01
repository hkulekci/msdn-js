## [Object.getOwnPropertyDescriptor Function (JavaScript)](Object.getOwnPropertyDescriptor-Function.html)

### Introduction 

 Gets the own property descriptor of the specified object. An own property descriptor is one that is defined directly on the object and is not inherited from the object's prototype.

### Syntax 

```
Object.getOwnPropertyDescriptor(object , propertyname )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The object that contains the property.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">propertyname</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The name of the property.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The descriptor of the property.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You can use the <b>Object.getOwnPropertyDescriptor</b> function to obtain a descriptor object that describes attributes of the property.
  </p>
  <p xmlns:util="util">
    The <span sdata="link"><a href="c5d05346-940a-40c2-b12a-e8b25abc8d46.htm">Object.defineProperty Function (JavaScript)</a></span> is used to add or modify properties.
  </p>
</div>

#### Data Property Example 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following example gets a data property descriptor and uses it to make the property read-only.
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
 // Create a user-defined object. var obj = {};  // Add a data property. obj.newDataProperty = "abc";  // Get the property descriptor. var descriptor = Object.getOwnPropertyDescriptor(obj, "newDataProperty");  // Change a property attribute. descriptor.writable = false; Object.defineProperty(obj, "newDataProperty", descriptor); 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    To list the property attributes, you can add the following code to this example.
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
 // Get the descriptor from the object. var desc2 = Object.getOwnPropertyDescriptor(obj, "newDataProperty");  // List the descriptor attributes. for (var prop in desc2) {     document.write(prop + ': ' + desc2[prop]);     document.write("&lt;br /&gt;"); }  // Output: // value: abc // writable: false // enumerable: true // configurable: true 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    All features are supported in Internet Explorer 9 standards mode, Internet Explorer 10 standards mode, and win8_appname_long apps.
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
    <span sdata="link" xmlns:util="util"><a href="c5d05346-940a-40c2-b12a-e8b25abc8d46.htm">Object.defineProperty Function (JavaScript)</a></span>
  </div>
</div>

