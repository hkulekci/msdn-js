## [WinRTError Object (JavaScript)](WinRTError-Object.html)

### Introduction 

 When a Windows Runtime call returns an HRESULT that indicates a failure, JavaScript converts it to a special Windows Runtime error. It is available only in Windows Store apps, when the Windows
Runtime is available, as part of the global JavaScript namespace.

### Syntax 

```
errorObj = new WinRTError();
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The WinRTError error type is used only for errors that originate in Windows Runtime APIs.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how a WinRTError is thrown and caught.
</p>

```
try { Windows.Storage.KnownFolders.documentsLibrary.createFileAsync("sample.txt"); } catch (err) { var n = err; }
```

#### Methods 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The WinRTError object has no methods.
  </p>
</div>

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The WinRTError object has the same properties as the <span sdata="link"><a href="0b27d6ec-3997-4e91-a6c0-5afbaf494db7.htm">Error Object (JavaScript)</a></span> object.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The WinRTError object is supported only in Windows Store apps, not in Internet Explorer.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="0b27d6ec-3997-4e91-a6c0-5afbaf494db7.htm">Error Object (JavaScript)</a></span>
  </div>
</div>

