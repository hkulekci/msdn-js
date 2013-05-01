## [index Property (RegExp) (JavaScript)](index-Property__RegExp.html)

### Introduction 

 Returns the character position where the first successful match begins in a searched string. Read-only.

### Syntax 

```
RegExp.index
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The object associated with this property is always the global <b>RegExp</b> object.
  </p>
  <p xmlns:util="util">
    The <b>index</b> property is zero-based. The initial value of the <b>index</b> property is &#8211;1. Its value changes whenever a successful match is made.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>index</b> property. This function iterates a search string and prints out the <b>index</b> and <b>lastIndex</b> values for each word in the
  string.
</p>

```
function RegExpTest() { var ver = Number(ScriptEngineMajorVersion() + "." + ScriptEngineMinorVersion()) if (ver &lt; 5.5) { document.write("You need a newer version of JavaScript for this to work");
return; } var src = "The quick brown fox jumps over the lazy dog."; // Create regular expression pattern with a global flag. var re = /\w+/g; // Get the next word, starting at the position of
lastindex. var arr; while ((arr = re.exec(src)) != null) { // New line: document.write ("&lt;br /&gt;"); document.write (arr.index + "-" + arr.lastIndex + " "); document.write (arr); } }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="7f6b1073-8cbb-49ed-94b6-56833ba663c5.htm">RegExp Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
</div>

