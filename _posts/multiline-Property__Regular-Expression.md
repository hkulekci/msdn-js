---
title: multiline Property (Regular Expression) (JavaScript)
isChild: false
---

## multiline Property (Regular Expression) (JavaScript) {multiline_property_regular_expression_javascript_title}

### Introduction 

 Returns a Boolean value indicating the state of the multiline flag (m) used with a regular expression. Default is false. Read-only.

### Syntax 

```
rgExp .multiline
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">rgExp</span> argument is an instance of the <b>RegExp</b> object
  </p>
  <p xmlns:util="util">
    The <b>multiline</b> property returns <b>true</b> if the multiline flag is set for a regular expression, and returns <b>false</b> if it is not. The <b>multiline</b> property is <b>true</b> if the
    regular expression object was created with the <b>m</b> flag.
  </p>
  <p xmlns:util="util">
    If <b>multiline</b> is <b>false</b>, "^" matches the position at the beginning of a string, and "$" matches the position at the end of a string. If <b>multiline</b> is <b>true</b>, "^" matches
    the position at the beginning of a string as well as the position following a "\n" or "\r", and "$" matches the position at the end of a string and the position preceding "\n" or "\r".
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the behavior of the <b>multiline</b> property. If you pass "m" in to the function shown below, the word "while" is replaced with the word "and". This is because
  with the multiline flag is set and the word "while" occurs at the beginning of the line after a newline character. The multiline flag allows the search to be performed on multiline strings.
</p>

```
function RegExpMultilineDemo(flag){ // The flag parameter is a string that contains // g, i, or m. The flags can be combined. // Check flags for validity. if (flag.match(/[^gim]/)) { return ("Flag
specified is not valid"); } // Create the string on which to perform the replacement. var ss = "The man hit the ball with the bat "; ss += "\nwhile the fielder caught the ball with the glove."; //
Replace "while" with "and". var re = new RegExp("^while", flag); var r = ss.replace(re, "and"); // Output the multiline flag and the resulting string. var s = ""; s += "Result for multiline = " +
re.multiline.toString(); s += ": " + r; return(s); } sa = RegExpMultilineDemo("m"); sb = RegExpMultilineDemo(""); document.write (sa + "&lt;br /&gt;" + sb);
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
    <span sdata="link" xmlns:util="util"><a href="816f0df5-5a82-44a5-a4ab-dbc91fa76e61.htm">ignoreCase Property (Regular Expression) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
</div>

