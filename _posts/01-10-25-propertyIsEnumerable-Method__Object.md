---
title: propertyIsEnumerable Method (Object) (JavaScript)
---

### Introduction 

 Determines whether a specified property is enumerable.

### Syntax 

```
object . propertyIsEnumerable(proName )
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
    The <b>propertyIsEnumerable</b> method returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if <span class="parameter" sdata="paramReference">proName</span>
    exists in <span class="parameter" sdata="paramReference">object</span> and can be enumerated using a <span sdata="langKeyword" value="For"><span class="keyword">For</span></span> loop. The
    <b>propertyIsEnumerable</b> method returns <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> if <span class="parameter" sdata="paramReference">object</span> does
    not have a property of the specified name or if the specified property is not enumerable. Typically, predefined properties are not enumerable, but user-defined properties are always enumerable.
  </p>
  <p xmlns:util="util">
    The <b>propertyIsEnumerable</b> method does not consider objects in the prototype chain.
  </p>
</div>

#### Example 

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

