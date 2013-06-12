---
title: switch Statement (JavaScript)
isChild: false
---

## switch Statement (JavaScript) {switch_statement_javascript_title}

### Introduction 

 Enables the execution of one or more statements when a specified expression's value matches a label.

### Syntax 

```
switch (expression ) { 
	case label : statementlist case label : default : statementlist }
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The expression to be evaluated.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">label</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        An identifier to be matched against <span class="parameter" sdata="paramReference">expression</span>. If <span class="parameter" sdata="paramReference">label</span> is an <span class=
        "parameter" sdata="paramReference">expression</span>, execution starts with the <span class="parameter" sdata="paramReference">statementlist</span> immediately after the colon, and continues
        until it encounters either a <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement, which is optional, or the end of the <span sdata="langKeyword" value=
        "switch"><span class="keyword">switch</span></span> statement.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statementlist</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        One or more statements to be executed.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Use the <span sdata="langKeyword" value="default"><span class="keyword">default</span></span> clause to provide a statement to be executed if none of the label values matches <span class=
    "parameter" sdata="paramReference">expression</span>. It can appear anywhere within the <span sdata="langKeyword" value="switch"><span class="keyword">switch</span></span> code block.
  </p>
  <p xmlns:util="util">
    Zero or more <span class="parameter" sdata="paramReference">label</span> blocks may be specified. If no <span class="parameter" sdata="paramReference">label</span> matches the value of
    <span class="parameter" sdata="paramReference">expression</span>, and a <span sdata="langKeyword" value="default"><span class="keyword">default</span></span> case is not supplied, no statements
    are executed.
  </p>
  <p xmlns:util="util">
    Execution flows through a <span sdata="langKeyword" value="switch"><span class="keyword">switch</span></span> statement as follows:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        Evaluate <span class="parameter" sdata="paramReference">expression</span> and look at <span class="parameter" sdata="paramReference">label</span> in order until a match is found.
      </p>
    </li>
    <li>
      <p>
        If a <span class="parameter" sdata="paramReference">label</span> value equals <span class="parameter" sdata="paramReference">expression</span>, execute its accompanying <span class=
        "parameter" sdata="paramReference">statementlist</span>.
      </p>
      <p>
        Continue execution until a <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement is encountered, or the <span sdata="langKeyword" value=
        "switch"><span class="keyword">switch</span></span> statement ends. This means that multiple <span class="parameter" sdata="paramReference">label</span> blocks are executed if a <span sdata=
        "langKeyword" value="break"><span class="keyword">break</span></span> statement is not used.
      </p>
    </li>
    <li>
      <p>
        If no <span class="parameter" sdata="paramReference">label</span> equals <span class="parameter" sdata="paramReference">expression</span>, go to the <span sdata="langKeyword" value=
        "default"><span class="keyword">default</span></span> case. If there is no <span sdata="langKeyword" value="default"><span class="keyword">default</span></span> case, go to last step.
      </p>
    </li>
    <li>
      <p>
        Continue execution at the statement following the end of the <span sdata="langKeyword" value="switch"><span class="keyword">switch</span></span> code block.
      </p>
    </li>
  </ul>
</div>

#### Example 

<p xmlns:util="util">
  The following example tests an object for its type.
</p>

```
function MyObjectType(obj) { switch (obj.constructor) { case Date: document.write("Object is a Date."); break; case Number: document.write("Object is a Number."); break; case String:
document.write("Object is a String."); break; default: document.write("Object is unknown."); } } // Output when obj is a Date: // Object is a Date. // Output when obj is a Number: // Object is a
Number. // Output when obj is a String: // Object is a String. // Output when obj is something other than a Date, Number, or String: // Object is unknown.
```

<p xmlns:util="util">
  The following code shows what happens if you do not use a <span sdata="langKeyword" value="break"><span class="keyword">break</span></span> statement.
</p>

```
function MyObjectType(obj) { switch (obj.constructor) { case Date: document.write("Object is a Date."); case Number: document.write("Object is a Number."); case String: document.write("Object is a
String."); default: document.write("Object is unknown."); } } // Output when obj is a Date: // Object is a Date.Object is a Number.Object is a String.Object is unknown. // Output when obj is a
Number: // Object is a Number.Object is a String.Object is unknown. // Output when obj is a String: // Object is a String.Object is unknown. // Output when obj is something other than a Date, Number,
or String: // Object is unknown.
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
    <span sdata="link" xmlns:util="util"><a href="5be0f2a8-5fe7-4a6c-89af-ca20a925ce87.htm">break Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="dfbe86e8-9c1e-4ef5-bb9c-7d1db7ce2506.htm">if...else Statement (JavaScript)</a></span>
  </div>
</div>

