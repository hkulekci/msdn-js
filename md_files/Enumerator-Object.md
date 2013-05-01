## [Enumerator Object (JavaScript)](Enumerator-Object.html)

### Introduction 

 Enables enumeration of items in a collection. Caution This object is supported in Internet Explorer only, not in Windows Store apps.

### Syntax 

```
enumObj = new Enumerator([collection ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">enumObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <b>Enumerator</b> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">collection</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Any Collection object.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Collections differ from arrays in that the members of a collection are not directly accessible. Instead of using indexes, as you would with arrays, you can move the current item pointer only to
    the first or next element of a collection.
  </p>
  <p xmlns:util="util">
    The <b>Enumerator</b> object provides a way to access any member of a collection and behaves similarly to the <b>For...Each</b> statement in VBScript.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows the usage of the <b>Enumerator</b> object:
</p>

```
var bytesPerGB = 1024 * 1024 * 1024; var fso = new ActiveXObject("Scripting.FileSystemObject"); document.write(fso.Drives); var e = new Enumerator(fso.Drives); var driveString = ""; e.moveFirst();
while (e.atEnd() == false) { var drv = e.item(); driveString += drv.Path + " - "; if (drv.IsReady){ var freeGB = drv.FreeSpace / bytesPerGB; var totalGB = drv.TotalSize / bytesPerGB; driveString +=
freeGB.toFixed(3) + " GB free of "; driveString += totalGB.toFixed(3) + " GB"; } else{ driveString += "Not Ready"; } driveString += "&lt;br /&gt;";; e.moveNext(); } document.write(driveString); //
Output: &lt;drive information
```

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The <b>Enumerator</b> object has no properties.
  </p>
</div>

#### Methods 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    atEnd Method | item Method | moveFirst Method | moveNext Method
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, and Internet
    Explorer 10 standards. Not supported in Windows Store apps. See Version Information.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d67748f2-7bf5-4889-8269-e777616cc5f0.htm">Boolean Object (JavaScript)</a></span>
  </div>
</div>

