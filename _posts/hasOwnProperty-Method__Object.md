---
title: hasOwnProperty Method (Object) (JavaScript)
isChild: false
---

## hasOwnProperty Method (Object) (JavaScript) {hasownproperty_method_object_javascript_title}

### Introduction 

 Determines whether an object has a property with the specified name.

### Syntax 

```
object. hasOwnProperty(proName )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Instance of an object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">proName</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. String value of a property name.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>hasOwnProperty</b> method returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if <span class="parameter" sdata="paramReference">object</span> has a
    property of the specified name, <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> if it does not. This method does not check the properties in the object's
    prototype chain; the property must be a member of the object itself.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  In the following example, all <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> objects share a common split method. The following code will display <b>false</b>
  and <b>true</b>.
</p>

```
var s = new String("Sample"); document.write(s.hasOwnProperty("split")); document.write("&lt;br/&gt;"); document.write(String.prototype.hasOwnProperty("split")); // Output: // false // true
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
    <span sdata="link" xmlns:util="util"><a href="dcd8f901-96b8-4c91-848b-b1ec0ab1c11c.htm">in Operator (JavaScript)</a></span>
  </div>
</div>

