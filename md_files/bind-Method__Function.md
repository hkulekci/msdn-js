## [bind Method (Function) (JavaScript)](bind-Method__Function.html)

### Introduction 

 For a given function, creates a bound function that has the same body as the original function. In the bound function, the this object resolves to the passed in object. The bound function has the
specified initial parameters.

### Syntax 

```
function .bind(thisArg [,arg1 [,arg2 [,argN ]]])
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">function</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A function object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">thisArg</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An object to which the <span sdata="langKeyword" value="this"><span class="keyword">this</span></span> keyword can refer inside the new function.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arg1</span>[,<span class="parameter" sdata="paramReference" xmlns:util="util">arg2</span>[,<span class="parameter" sdata=
      "paramReference" xmlns:util="util">argN</span>]]]
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A list of arguments to be passed to the new function.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    A new function that is the same as the <span class="parameter" sdata="paramReference">function</span> function, except for the <span class="parameter" sdata="paramReference">thisArg</span> object
    and the initial arguments.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the specified <span class="parameter" sdata="paramReference">function</span> is not a function, a <b>TypeError</b> exception is thrown.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use the <b>bind</b> method.
</p>

```
// Define the original function. var checkNumericRange = function (value) { if (typeof value !== 'number') return false; else return value &gt;= this.minimum &amp;&amp; value &lt;= this.maximum; } //
The range object will become the this value in the callback function. var range = { minimum: 10, maximum: 20 }; // Bind the checkNumericRange function. var boundCheckNumericRange =
checkNumericRange.bind(range); // Use the new function to check whether 12 is in the numeric range. var result = boundCheckNumericRange (12); document.write(result); // Output: true
```

<p xmlns:util="util">
  In the following example, the <span class="parameter" sdata="paramReference">thisArg</span> object is different from the object that contains the original method.
</p>

```
// Create an object that contains the original function. var originalObject = { minimum: 50, maximum: 100, checkNumericRange: function (value) { if (typeof value !== 'number') return false; else
return value &gt;= this.minimum &amp;&amp; value &lt;= this.maximum; } } // Check whether 10 is in the numeric range. var result = originalObject.checkNumericRange(10); document.write(result + " ");
// Output: false // The range object supplies the range for the bound function. var range = { minimum: 10, maximum: 20 }; // Create a new version of the checkNumericRange function that uses range.
var boundObjectWithRange = originalObject.checkNumericRange.bind(range); // Check whether 10 is in the numeric range. var result = boundObjectWithRange(10); document.write(result); // Output: true
```

<p xmlns:util="util">
  The following code shows how to use the <span class="parameter" sdata="paramReference">arg1[,arg2[,argN]]]</span> arguments. The bound function uses the parameters specified in the <b>bind</b>
  method as the first and second parameters. Any parameters specified when the bound function is called are used as the third, fourth (and so on) parameters.
</p>

```
// Define the original function with four parameters. var displayArgs = function (val1, val2, val3, val4) { document.write(val1 + " " + val2 + " " + val3 + " " + val4); } var emptyObject = {}; //
Create a new function that uses the 12 and "a" parameters // as the first and second parameters. var displayArgs2 = displayArgs.bind(emptyObject, 12, "a"); // Call the new function. The "b" and "c"
parameters are used // as the third and fourth parameters. displayArgs2("b", "c"); // Output: 12 a b c
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Internet Explorer 9 standards and Internet Explorer 10 standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d3834767-203c-475e-848c-95c423ba15b6.htm">Function Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1d260370-9e6e-43fc-870f-2d35850db7ee.htm">filter Method (Array) (JavaScript)</a></span>
  </div>
</div>

