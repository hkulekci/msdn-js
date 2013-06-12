---
title: Debug.setNonUserCodeExceptions Property
isChild: false
---

## Debug.setNonUserCodeExceptions Property {debugsetnonusercodeexceptions_property_title}

### Introduction 

 Determines whether any try-catch blocks in this scope are to be treated by the debugger as user-unhandled. Exceptions can be classified as thrown, user-unhandled or unhandled. If this property is set
to true in a given scope, the debugger can then determine to take some action (for example, break) on exceptions thrown inside that scope if the developer wishes to break on user-unhandled
exceptions. If this property is set to false is the same as if the property was never set. For more information on debugging, see Active Script Debugging Overview.

### Syntax 

```
Debug.setNonUserCodeExceptions [= bool];
```

#### Example 

<p xmlns:util="util">
  The following code shows how to set this property.
</p>

```
(function () { Debug.setNonUserCodeExceptions = true; try{ var x = null; x.y(); } catch (e) { // Catch the exception. } })();
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the Internet Explorer 10 standards document mode. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards.
  </p>
</div>

