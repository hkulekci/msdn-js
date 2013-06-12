---
title: var Statement (JavaScript)
---

### Introduction 

 Declares a variable.

### Syntax 

```
var variable1 = value1
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">variable1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The name of the variable being declared.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">value1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The initial value assigned to the variable.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Use the <span sdata="langKeyword" value="var"><span class="keyword">var</span></span> statement to declare variables. You can assign values to the variables when you declare them or later in your
    script.
  </p>
  <p xmlns:util="util">
    A variable is declared the first time it appears in your script.
  </p>
  <p xmlns:util="util">
    You can declare a variable without using the <span sdata="langKeyword" value="var"><span class="keyword">var</span></span> keyword and assign a value to it. This is known as an <span class=
    "term">implicit declaration</span>, and it is not recommended. An implicit declaration gives the variable global scope. When you declare a variable at the procedure level, though, you typically
    do not want it to have global scope. To avoid giving the variable global scope, you must use the <span sdata="langKeyword" value="var"><span class="keyword">var</span></span> keyword in your
    variable declaration.
  </p>
  <p xmlns:util="util">
    If you do not initialize your variable in the <span sdata="langKeyword" value="var"><span class="keyword">var</span></span> statement, it is automatically assigned the JavaScript value
    <span sdata="langKeyword" value="undefined"><span class="keyword">undefined</span></span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following examples illustrate the use of the <span sdata="langKeyword" value="var"><span class="keyword">var</span></span> statement.
</p>

```
var index; var name = "Thomas Jefferson"; var answer = 42, counter, numpages = 10; var myarray = new Array();
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
    <span sdata="link" xmlns:util="util"><a href="cc9cfd43-1305-41c8-ad67-545d20f4fafe.htm">function Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="5ea556ba-7ae6-426c-8430-9032eee5a0a5.htm">new Operator (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">JScript Variables (Windows Scripting - JScript)</span>
  </div>
</div>

