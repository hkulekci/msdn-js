---
title: toString Method (Boolean)
isChild: false
---

## toString Method (Boolean) {tostring_method_boolean_title}

### Introduction 

 Returns a string representation of an object.

### Syntax 

```
boolean .toString()
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">boolean</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An object for which to get a string representation.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the Boolean value is <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>, returns "true". Otherwise, returns "false".
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>toString</b> method.
</p>

```
var s = new Boolean(0); document.write(s.toString()); // Output: false;
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

