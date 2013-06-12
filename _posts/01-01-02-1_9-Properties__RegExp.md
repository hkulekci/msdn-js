---
title: $1...$9 Properties (RegExp) (JavaScript)
---

### Introduction 

 Return the nine most-recently memorized portions found during pattern matching. Read-only.

### Syntax 

```
RegExp.$n
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <b xmlns:util="util">RegExp</b>
    </dt>
    <dd>
      <p xmlns:util="util">
        Always the global <b>RegExp</b> object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">n</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any integer from 1 through 9.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The values of the <b>$1...$9</b> properties are modified whenever a successful parenthesized match is made. Any number of parenthesized substrings may be specified in a regular expression
    pattern, but only the nine most recent can be stored.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example performs a regular expression search. It displays matches and submatches from the global <b>RegExp</b> object. The submatches are successful parenthesized matches that are
  contained in the <b>$1&hellip;$9</b> properties. The example also displays matches and submatches from the array that is returned by the <b>exec</b> method.
</p>

```
var newLine = "&lt;br /&gt;"; var re = /(\w+)@(\w+)\.(\w+)/g var src = "Please send mail to george@contoso.com and someone@example.com. Thanks!" var result; var s = ""; // Get the first match. result
= re.exec(src); while (result != null) { // Show the entire match. s += newLine; // Show the match and submatches from the RegExp global object. s += "RegExp.lastMatch: " + RegExp.lastMatch +
newLine; s += "RegExp.$1: " + RegExp.$1 + newLine; s += "RegExp.$2: " + RegExp.$2 + newLine; s += "RegExp.$3: " + RegExp.$3 + newLine; // Show the match and submatches from the array that is returned
// by the exec method. for (var index = 0; index &lt; result.length; index++) { s += index + ": "; s += result[index]; s += newLine; } // Get the next match. result = re.exec(src); }
document.write(s); // Output: // RegExp.lastMatch: george@contoso.com // RegExp.$1: george // RegExp.$2: contoso // RegExp.$3: com // 0: george@contoso.com // 1: george // 2: contoso // 3: com //
RegExp.lastMatch: someone@example.com // RegExp.$1: someone // RegExp.$2: example // RegExp.$3: com // 0: someone@example.com // 1: someone // 2: example // 3: com
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

