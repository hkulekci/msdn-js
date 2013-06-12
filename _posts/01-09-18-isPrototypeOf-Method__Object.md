---
title: isPrototypeOf Method (Object) (JavaScript)
---

### Introduction 

 Determines whether an object exists in another object's prototype chain.

### Syntax 

```
object1 . isPrototypeOf(object2 )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Instance of an object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object2</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Another object whose prototype chain is to be checked.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>isPrototypeOf</b> method returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if <span class="parameter" sdata="paramReference">object2</span> has
    <span class="parameter" sdata="paramReference">object1</span> in its prototype chain. The prototype chain is used to share functionality between instances of the same object type. The
    <b>isPrototypeOf</b> method returns <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> when <span class="parameter" sdata="paramReference">object2</span> is not an
    object or when <span class="parameter" sdata="paramReference">object1</span> does not appear in the prototype chain of the <span class="parameter" sdata="paramReference">object2</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>isPrototypeOf</b> method.
</p>

```
var re = new RegExp(); document.write(RegExp.prototype.isPrototypeOf(re)); // Output: true
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

