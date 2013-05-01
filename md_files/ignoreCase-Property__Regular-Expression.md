## [ignoreCase Property (Regular Expression) (JavaScript)](ignoreCase-Property__Regular-Expression.html)

### Introduction 

 Returns a Boolean value indicating the state of the ignoreCase flag (i) used with a regular expression. Default is false. Read-only.

### Syntax 

```
rgExp .ignoreCase
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">rgExp</span> reference is an instance of the <b>RegExp</b> object.
  </p>
  <p xmlns:util="util">
    The <b>ignoreCase</b> property returns <b>true</b> if the ignoreCase flag is set for a regular expression, and returns <b>false</b> if it is not.
  </p>
  <p xmlns:util="util">
    The ignoreCase flag, when used, indicates that a search should ignore case sensitivity when matching the pattern within the searched string.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>ignoreCase</b> property. If you pass "gi" in to the function shown below, all instances of the word "the" are replaced with the word "a",
  including the initial "The". This is because with the ignoreCase flag set, the search ignores any case sensitivity. So "T" is the same as "t" for the purposes of matching.
</p>

```
function RegExpPropDemo(flag){ // The flag parameter is a string that contains // g, i, or m. The flags can be combined. // Check flags for validity. if (flag.match(/[^gim]/)) { return ("Flag
specified is not valid"); } // Create the string on which to perform the replacement. var orig = "The batter hit the ball with the bat "; orig += "and the fielder caught the ball with the glove."; //
Replace "the" with "a". var re = new RegExp("the", flag); var r = orig.replace(re, "a"); // Output the resulting string and the values of the flags. var s = ""; s += "global: " +
re.global.toString(); s += "&lt;br /&gt;"; s += "ignoreCase: " + re.ignoreCase.toString(); s += "&lt;br /&gt;"; s += "multiline: " + re.multiline.toString(); s += "&lt;br /&gt;"; s += "Resulting
String: " + r; s += "&lt;br /&gt;"; s += "&lt;br /&gt;"; return (s); } document.write(RegExpPropDemo("gi")); document.write(RegExpPropDemo("g"));
```

<p xmlns:util="util">
  This function returns the Boolean values that indicate the state of the allowable regular expression flags, which are <b>g</b>, <b>i</b>, and <b>m</b>. The function also returns the string with all
  replacements made.
</p>

```
global: true ignoreCase: true multiline: false Resulting String: a batter hit a ball with a bat and a fielder caught a ball with a glove. global: true ignoreCase: false multiline: false Resulting
String: The batter hit a ball with a bat and a fielder caught a ball with a glove.
```

<p xmlns:util="util">
  Following is the resulting output.
</p>

```
<p xmlns:util="util">
  Following is the resulting output.
</p>
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="346aa83e-a045-47ea-acae-b42c7b121534.htm">Regular Expression Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="76a0f115-0d89-4aca-86d5-932895c6d649.htm">global Property (Regular Expression) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ca7b276a-1fe2-4189-ac27-f089ab3e9974.htm">multiline Property (Regular Expression) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
</div>

