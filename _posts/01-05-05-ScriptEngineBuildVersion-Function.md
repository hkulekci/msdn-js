---
title: ScriptEngineBuildVersion Function (JavaScript)
---

### Introduction 

 Gets the build version number of the scripting engine in use.

### Syntax 

```
ScriptEngineBuildVersion()
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The return value corresponds directly to the version information contained in the dynamic-link library (DLL) for the scripting language in use.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>ScriptEngineBuildVersion</b> function:
</p>

```
document.write(ScriptEngineBuildVersion()); // Output: &lt;current build version&gt;
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
    <span sdata="link" xmlns:util="util"><a href="65674b2b-d2c2-4493-99b3-f0d20fda8249.htm">ScriptEngine Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="3e251bce-1e14-4cb5-b79f-53845d1920fd.htm">ScriptEngineMajorVersion Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="caa506a5-e61d-4b2a-8b83-83d56a2f26cd.htm">ScriptEngineMinorVersion Function (JavaScript)</a></span>
  </div>
</div>

