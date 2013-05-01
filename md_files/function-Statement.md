## [function Statement (JavaScript)](function-Statement.html)

### Introduction 

 Declares a new function.

### Syntax 

```
function functionname ([arg1 [, arg2 [,...[, argN ]]]]) { 
	statements }
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">functionname</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The name of the function.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arg1...argN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. An optional, comma-separated list of arguments the function understands.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statements</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. One or moreJavaScript statements.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Use the <span sdata="langKeyword" value="function"><span class="keyword">function</span></span> statement to declare a function for later use. The code that is contained in <span class=
    "parameter" sdata="paramReference">statements</span> is not executed until the function is called from elsewhere in the script.
  </p>
  <p xmlns:util="util">
    The return statement is used to return a value from the function. You do not have to use a <span sdata="langKeyword" value="return"><span class="keyword">return</span></span> statement; the
    program will return when it reaches the end of the function. If no <span sdata="langKeyword" value="return"><span class="keyword">return</span></span> statement is executed in the function, or if
    the <span sdata="langKeyword" value="return"><span class="keyword">return</span></span> statement has no expression, the function returns the value <span sdata="langKeyword" value=
    "undefined"><span class="keyword">undefined</span></span>.
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
            When you call a function, be sure to include the parentheses and any required arguments. Calling a function without parentheses returns a reference to the function, not the results of the
            function.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="function"><span class="keyword">function</span></span> statement.
</p>

```
function myfunction (arg1, arg2) { var r = arg1 * arg2; return(r); }
```

<p xmlns:util="util">
  A function can be assigned to a variable. This is illustrated in the following example.
</p>

```
function AddFive(x) { return x + 5; } function AddTen(x) { return x + 10; } var condition = false; var MyFunc; if (condition) { MyFunc = AddFive; } else { MyFunc = AddTen; } var result = MyFunc(123);
// Output: 133
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
    <span sdata="link" xmlns:util="util"><a href="5ea556ba-7ae6-426c-8430-9032eee5a0a5.htm">new Operator (JavaScript)</a></span>
  </div>
</div>

