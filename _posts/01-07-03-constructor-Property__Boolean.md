---
title: constructor Property (Boolean)
---

### Introduction 

 Specifies the function that creates a Boolean.

### Syntax 

```
boolean .constructor([[value ])
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">boolean</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The name of the Boolean.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">value</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Specifies the value of the Boolean. This can be the numbers 1 or 0, or the strings "true" or "false".
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>constructor</b> property contains a reference to the function that constructs instances of the Boolean object.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the constructor property.
</p>

```
var x = new Boolean("true"); if (x.constructor == Boolean) document.write("Object is a Boolelan."); // Output: // Object is a Boolean.
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

