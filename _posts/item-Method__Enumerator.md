---
title: item Method (Enumerator) (JavaScript)
isChild: false
---

## item Method (Enumerator) (JavaScript) {item_method_enumerator_javascript_title}

### Introduction 

 Returns the current item in the collection. Caution This object is supported in Internet Explorer only.

### Syntax 

```
enumObj .item()
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <i>enumObj</i> reference is any <b>Enumerator</b> object.
  </p>
  <p xmlns:util="util">
    The <b>item</b> method returns the current item. If the collection is empty or the current item is undefined, it returns <b>undefined</b>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  In following code, the <b>item</b> method is used to return a member of the <b>Drives</b> collection.
</p>

```
function ShowDrives() { var s = ""; var bytesPerGB = 1024 * 1024 * 1024; var fso = new ActiveXObject("Scripting.FileSystemObject"); var e = new Enumerator(fso.Drives); e.moveFirst(); while (e.atEnd()
== false) { var drv = e.item(); s += drv.Path + " - "; if (drv.IsReady) { var freeGB = drv.FreeSpace / bytesPerGB; var totalGB = drv.TotalSize / bytesPerGB; s += freeGB.toFixed(3) + " GB free of "; s
+= totalGB.toFixed(3) + " GB"; } else { s += "Not Ready"; } s += "&lt;br /&gt;"; e.moveNext(); } return(s); }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, and Internet
    Explorer 10 standards. Not supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="63f03c21-d58c-47db-a728-4d8d88b0a422.htm">Enumerator Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="326808fb-9a0f-428e-aff1-b11b237913f1.htm">atEnd Method (Enumerator) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="96eedc66-7974-443c-b0cd-55373a7c0e59.htm">moveFirst Method (Enumerator) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="59aa339b-f375-450a-8276-37896a55a824.htm">moveNext Method (Enumerator) (JavaScript)</a></span>
  </div>
</div>

