---
title: lastIndex Property (RegExp) (JavaScript)
isChild: false
---

## lastIndex Property (RegExp) (JavaScript) {lastindex_property_regexp_javascript_title}

### Introduction 

 Returns the character position where the next match begins in a searched string.

### Syntax 

```
RegExp.lastIndex
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The object associated with this property is always the global <b>RegExp</b> object.
  </p>
  <p xmlns:util="util">
    The <b>lastIndex</b> property is zero-based, that is, the index of the first character is zero. Its initial value is &#8211;1. Its value is modified whenever a successful match is made.
  </p>
  <p xmlns:util="util">
    The <b>lastIndex</b> property is modified by the <b>exec</b> and <b>test</b> methods of the <b>RegExp</b> object, and the <b>match</b>, <b>replace</b>, and <b>split</b> methods of the
    <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object.
  </p>
  <p xmlns:util="util">
    The following rules apply to values of <b>lastIndex</b>:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        If there is no match, <b>lastIndex</b> is set to -1.
      </p>
    </li>
    <li>
      <p>
        If <b>lastIndex</b> is greater than the length of the string, <b>test</b> and <b>exec</b> fail and <b>lastIndex</b> is set to -1.
      </p>
    </li>
    <li>
      <p>
        If <b>lastIndex</b> is equal to the length of the string, the regular expression matches if the pattern matches the empty string. Otherwise, the match fails and <b>lastIndex</b> is reset to
        -1.
      </p>
    </li>
    <li>
      <p>
        Otherwise, <b>lastIndex</b> is set to the next position following the most recent match.
      </p>
    </li>
  </ul>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>lastIndex</b> property. This function iterates a search string and prints out the <b>index</b> and <b>lastIndex</b> values for each word in the
  string.
</p>

```
function RegExpTest() { var ver = Number(ScriptEngineMajorVersion() + "." + ScriptEngineMinorVersion()) if (ver &lt; 5.5) { document.write("You need a newer version of JavaScript for this to work");
return; } var src = "The quick brown fox jumps over the lazy dog."; // Create regular expression pattern with a global flag. var re = /\w+/g; // Get the next word, starting at the position of
lastindex. var arr; while ((arr = re.exec(src)) != null) { // New line: document.write ("&lt;br /&gt;"); document.write (arr.index + "-" + re.lastIndex + " "); document.write (arr); } }
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

