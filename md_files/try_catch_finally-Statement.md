---
title: try...catch...finally Statement (JavaScript)
isChild: false
---

## try...catch...finally Statement (JavaScript) {trycatchfinally_statement_javascript_title}

### Introduction 

 Sets up blocks of code in which errors that are thrown in one block are handled in another. Errors that are thrown inside the try block are caught in the catch block. JavaScript.

### Syntax 

```
try { 
	tryStatements } 
catch(exception ){ 
	catchStatements } 
finally { 
	finallyStatements }
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">tryStatements</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Statements where an error can occur.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">exception</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any variable name. The initial value of <span class="parameter" sdata="paramReference">exception</span> is the value of the thrown error.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">catchStatements</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Statements to handle errors occurring in the associated <span class="parameter" sdata="paramReference">tryStatements</span>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">finallyStatements</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Statements that are unconditionally executed after all other error processing has occurred.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="try...catch...finally"><span class="keyword">try...catch...finally</span></span> statement provides a way to handle some or all of the errors that may occur
    in a given block of code, while still running code. If errors occur that are not handled, JavaScript provides the normal error message.
  </p>
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="try"><span class="keyword">try</span></span> block contains code that may provoke an error, while the <span sdata="langKeyword" value="catch"><span class=
    "keyword">catch</span></span> block contains the code that handles some or all errors. If an error occurs in the <span sdata="langKeyword" value="try"><span class="keyword">try</span></span>
    block, program control is passed to the <span sdata="langKeyword" value="catch"><span class="keyword">catch</span></span> block. The value of <span class="parameter" sdata=
    "paramReference">exception</span> is the value of the error that occurred in the <span sdata="langKeyword" value="try"><span class="keyword">try</span></span> block. If no error occurs, the code
    in the <span sdata="langKeyword" value="catch"><span class="keyword">catch</span></span> block is never executed.
  </p>
  <p xmlns:util="util">
    You can pass the error up to the next level by using the <span sdata="langKeyword" value="throw"><span class="keyword">throw</span></span> statement to re-throw the error.
  </p>
  <p xmlns:util="util">
    After all the statements in the <span sdata="langKeyword" value="try"><span class="keyword">try</span></span> block have been executed and error handling has been done in the <span sdata=
    "langKeyword" value="catch"><span class="keyword">catch</span></span> block, the statements in the <span sdata="langKeyword" value="finally"><span class="keyword">finally</span></span> block are
    executed, whether or not an error was handled. The code in the <span sdata="langKeyword" value="finally"><span class="keyword">finally</span></span> block is guaranteed to run unless an unhandled
    error occurs (for example, a run-time error inside the <b>catch</b> block).
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example causes a <span sdata="langKeyword" value="ReferenceError"><span class="keyword">ReferenceError</span></span> exception to be thrown and displays the name of the error and its
  message.
</p>

```
try { addalert("bad call"); } catch(e) { document.write ("Error Message: " + e.message); document.write ("&lt;br /&gt;"); document.write ("Error Code: "); document.write (e.number &amp; 0xFFFF)
document.write ("&lt;br /&gt;"); document.write ("Error Name: " + e.name); } // Output: Error Message: 'addalert' is undefined Error Code: 5009 Error Name: ReferenceError
```

<p xmlns:util="util">
  The following example shows how to re-throw errors, as well as the execution of nested <span sdata="langKeyword" value="try&#8230;catch"><span class="keyword">try&#8230;catch</span></span> blocks.
  When the error is thrown from the nested <span sdata="langKeyword" value="try"><span class="keyword">try</span></span> block, it passes to the nested <span sdata="langKeyword" value=
  "catch"><span class="keyword">catch</span></span> block, which re-throws it. The nested <span sdata="langKeyword" value="finally"><span class="keyword">finally</span></span> block runs before the
  outer <span sdata="langKeyword" value="catch"><span class="keyword">catch</span></span> block handles the error, and at the end the outer <span sdata="langKeyword" value="finally"><span class=
  "keyword">finally</span></span> block runs.
</p>

```
try { document.write("Outer try running...&lt;br/&gt;"); try { document.write("Nested try running...&lt;br/&gt;"); throw new Error(301, "an error"); } catch (e) { document.write ("Nested catch caught
" + e.message + "&lt;br/&gt;"); throw e; } finally { document.write ("Nested finally is running...&lt;br/&gt;"); } } catch (e) { document.write ("Outer catch caught " + e.message + "&lt;br/&gt;"); }
finally { document.write ("Outer finally running"); } // Output: // Outer try running... // Nested try running... // Nested catch caught error from nested try // Nested finally is running... // Outer
catch caught error from nested try // Outer finally running
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
    <span sdata="link" xmlns:util="util"><a href="75cbade0-fb81-4ffe-b187-b71be380bb05.htm">throw Statement (JavaScript)</a></span>
  </div>
</div>

