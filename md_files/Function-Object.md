---
title: Function Object (JavaScript)
isChild: false
---

## Function Object (JavaScript) {function_object_javascript_title}

### Introduction 

 Creates a new function.

### Syntax 

```
function functionName ([argname1 [, ...[, argnameN ]]]) { 
	body }
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">functionName</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The name of the newly created function
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">argname1...argnameN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A list of arguments the function accepts.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">body</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A string that contains the block of JavaScript code to be executed when the function is called.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The function is a basic data type in JavaScript. Syntax 1 creates a function value that JavaScript converts into a <span sdata="langKeyword" value="Function"><span class=
    "keyword">Function</span></span> object when necessary. JavaScript converts <span sdata="langKeyword" value="Function"><span class="keyword">Function</span></span> objects created by Syntax 2
    into function values at the time the function is called.
  </p>
  <p xmlns:util="util">
    Syntax 1 is the standard way to create new functions in JavaScript. Syntax 2 is an alternative form used to create function objects explicitly.
  </p>
  <p xmlns:util="util">
    For example, to declare a function that adds the two arguments passed to it, you can do it in one of two ways:
  </p>
</div>

#### Example 1 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          JavaScript&nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 function add(x, y) {    return(x + y); } 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 2 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          &nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 var add = function(x, y) {      return(x+y); } 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    In either case, you call the function with a line of code similar to the following:
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          JavaScript&nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 add(2, 3); 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <div class="alert">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th align="left">
          <img class="note" alt="Note" title="Note" src="../icons/alert_note.gif" /><b>Note</b>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            When you call a function, make sure that you always include the parentheses and any required arguments. Calling a function without parentheses causes the function itself to be returned,
            instead of the return value of the function.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Properties 

<div id="sectionSection3" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    0...n Properties |arguments Property | callee Property | caller Property | constructor Property | length Property (Function) | prototype Property
  </p>
</div>

#### Methods 

<div id="sectionSection4" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    apply Method | bind Method | call Method | toString Method | valueOf Method
  </p>
</div>

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
    <span sdata="link" xmlns:util="util"><a href="cc9cfd43-1305-41c8-ad67-545d20f4fafe.htm">function Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="5ea556ba-7ae6-426c-8430-9032eee5a0a5.htm">new Operator (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="56f900af-a5c4-4667-9664-5956d30f0aae.htm">var Statement (JavaScript)</a></span>
  </div>
</div>

