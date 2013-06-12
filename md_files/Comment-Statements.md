---
title: Comment Statements (JavaScript)
isChild: false
---

## Comment Statements (JavaScript) {comment_statements_javascript_title}

### Introduction 

 Causes comments to be ignored by the JavaScript parser.

### Syntax 

```
Single-line Comment: // comment
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">comment</span> argument is the text of any comment you want to include in your script. The <span class="parameter" sdata=
    "paramReference">condStatement</span> argument is to be used if conditional compilation is activated. If single-line comments are used, there can be no space between the "//" and "@" characters.
  </p>
  <p xmlns:util="util">
    Use comments to keep parts of a script from being read by the JavaScript parser. You can use comments to include explanatory remarks in a program.
  </p>
  <p xmlns:util="util">
    If single-line comments are used, the parser ignores any text between the comment marker and the end of the line. If multi-line comments are used, the parser ignores any text between the
    beginning and end markers.
  </p>
  <p xmlns:util="util">
    Comments are used to support conditional compilation while retaining compatibility with browsers that do not support that feature. These browsers treat those forms of comments as single-line or
    multi-line comments respectively.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the most common uses of comments.
</p>

```
/* This is a multiline comment that can span as many lines as necessary. */ function myfunction(arg1, arg2){ var r; // This is a single line comment. r = arg1 + arg2 return(r); }
```

<p xmlns:util="util">
  The following example shows how to use conditional compilation. This example uses special comment delimiters that are used only if conditional compilation is activated by the <span sdata=
  "langKeyword" value="@cc_on"><span class="keyword">@cc_on</span></span> statement. Scripting engines that do not support conditional compilation see only the message that says conditional
  compilation is not supported.
</p>

```
/*@cc_on @*/ /*@if (@_jscript_version &gt;= 4) alert("JavaScript version 4 or better"); @else @*/ alert("Conditional compilation not supported by this scripting engine."); /*@end @*/
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

