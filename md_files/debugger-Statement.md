## [debugger Statement (JavaScript)](debugger-Statement.html)

### Introduction 

 Suspends execution.

### Syntax 

```
debugger
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You can place <span sdata="langKeyword" value="debugger"><span class="keyword">debugger</span></span> statements anywhere in procedures to suspend execution. Using the <span sdata="langKeyword"
    value="debugger"><span class="keyword">debugger</span></span> statement is similar to setting a breakpoint in the code.
  </p>
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="debugger"><span class="keyword">debugger</span></span> statement suspends execution, but it does not close any files or clear any variables.
  </p>
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
            The <span sdata="langKeyword" value="debugger"><span class="keyword">debugger</span></span> statement has no effect unless the script is being debugged.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  This example uses the <span sdata="langKeyword" value="debugger"><span class="keyword">debugger</span></span> statement to suspend execution for each iteration through the <span sdata="langKeyword"
  value="for"><span class="keyword">for</span></span> loop.
</p>

```
for(i = 1; i&lt;5; i++) { // Print i to the Output window. Debug.write("loop index is " + i); // Wait for user to resume. debugger }
```

<p xmlns:util="util">
  To run this example, you must have a script debugger installed and the script must run in debug mode.
</p>

```
<p xmlns:util="util">
  To run this example, you must have a script debugger installed and the script must run in debug mode.
</p>
```

<p xmlns:util="util">
  Internet Explorer 8 includes the JavaScript debugger. If you are using an earlier version of Internet Explorer, see <a href="http://go.microsoft.com/fwlink/?LinkId=133801">How to: Enable and Start
  Script Debugging from Internet Explorer</a>.
</p>

```
<p xmlns:util="util">
  Internet Explorer 8 includes the JavaScript debugger. If you are using an earlier version of Internet Explorer, see <a href="http://go.microsoft.com/fwlink/?LinkId=133801">How to: Enable and Start
  Script Debugging from Internet Explorer</a>.
</p>
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
    <span sdata="link" xmlns:util="util"><a href="c0abc33e-5ebf-4e83-8a08-a1db9070e3b4.htm">JavaScript Statements</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Conditional Compilation</span>
  </div>
</div>

