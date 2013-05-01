## [return Statement (JavaScript)](return-Statement.html)

### Introduction 

 Exits from the current function and returns a value from that function.

### Syntax 

```
return[(][expression ][)];
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The optional <i>expression</i> argument is the value to be returned from the function. If omitted, the function does not return a value.
  </p>
  <p xmlns:util="util">
    You use the <span sdata="langKeyword" value="return"><span class="keyword">return</span></span> statement to stop execution of a function and return the value of <i>expression</i>. If
    <i>expression</i> is omitted, or no <span sdata="langKeyword" value="return"><span class="keyword">return</span></span> statement is executed from within the function, the expression that called
    the current function is assigned the value undefined.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="return"><span class="keyword">return</span></span> statement.
</p>

```
function myfunction(arg1, arg2){ var r; r = arg1 * arg2; return(r); }
```

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="return"><span class="keyword">return</span></span> statement to return a function.
</p>

```
function doWork() { return function calculate(y) { return y + 1; }; } var func = doWork(); var x = func(5); document.write(x); // Output: 6
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
</div>

