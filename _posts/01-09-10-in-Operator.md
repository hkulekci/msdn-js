---
title: in Operator (JavaScript)
---

### Introduction 

 Tests for the existence of a property in an object.

### Syntax 

```
result = property in object
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">result</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any variable.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">property</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An expression that evaluates to a string expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any object.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>in</b> operator determines whether an object has a property named <span class="parameter" sdata="paramReference">property</span>. It also determines whether the property is part of the
    object's prototype chain. For more information about object prototypes, see <span sdata="link">Prototypes and Prototype Inheritance</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>in</b> operator:
</p>

```
// Create an object that has some properties. var myObject = new Object(); myObject.name = "James"; myObject.age = "22"; myObject.phone = "555 0234"; if ("phone" in myObject) document.write
("property is present"); else document.write ("property is not present"); // Output: property is present
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

