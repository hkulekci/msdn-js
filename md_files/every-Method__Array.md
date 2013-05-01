## [every Method (Array) (JavaScript)](every-Method__Array.html)

### Introduction 

 Determines whether all the members of an array satisfy the specified test.

### Syntax 

```
array1 .every(callbackfn [, thisArg ])
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Parameter
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Definition
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">array1</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Required. An array object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">callbackfn</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Required. A function that accepts up to three arguments. The <b>every</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function for each element in
            <span class="parameter" sdata="paramReference">array1</span> until the <span class="parameter" sdata="paramReference">callbackfn</span> returns <span sdata="langKeyword" value=
            "false"><span class="keyword">false</span></span>, or until the end of the array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">thisArg</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Optional. An object to which the <span sdata="langKeyword" value="this"><span class="keyword">this</span></span> keyword can refer in the <span class="parameter" sdata=
            "paramReference">callbackfn</span> function. If <span class="parameter" sdata="paramReference">thisArg</span> is omitted, <span sdata="langKeyword" value="undefined"><span class=
            "keyword">undefined</span></span> is used as the <span sdata="langKeyword" value="this"><span class="keyword">this</span></span> value.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if the <span class="parameter" sdata="paramReference">callbackfn</span> function returns <span sdata="langKeyword"
    value="true"><span class="keyword">true</span></span> for all array elements; otherwise, <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>. If the array is has no
    elements, the <b>every</b> method returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the <span class="parameter" sdata="paramReference">callbackfn</span> argument is not a function object, a <b>TypeError</b> exception is thrown.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>every</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each array element, in ascending index order, until the <span class=
    "parameter" sdata="paramReference">callbackfn</span> function returns <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>. If an element that causes <span class=
    "parameter" sdata="paramReference">callbackfn</span> to return <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> is found, the <b>every</b> method immediately
    returns <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>. Otherwise, the <span sdata="langKeyword" value="every"><span class="keyword">every</span></span> method
    returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>.
  </p>
  <p xmlns:util="util">
    The callback function is not called for missing elements of the array.
  </p>
  <p xmlns:util="util">
    In addition to array objects, the <b>every</b> method can be used by any object that has a <span sdata="langKeyword" value="length"><span class="keyword">length</span></span> property and that
    has numerically indexed property names.
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
            You can use the <span sdata="link"><a href="7b6822f9-c406-4f4e-bfec-a93459745992.htm">some Method (Array) (JavaScript)</a></span> to check whether the callback function returns
            <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> for any element of an array.
          </p>
        </td>
      </tr>
    </table>
  </div>
  <h3 class="subHeading">
    Callback Function Syntax
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      The syntax of the callback function is as follows:
    </p>
    <p xmlns:util="util">
      <span class="code">function callbackfn(value, index, array1)</span>
    </p>
    <p xmlns:util="util">
      You can declare the callback function with up to three parameters.
    </p>
    <p xmlns:util="util">
      The following table lists the callback function parameters.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Callback parameter
            </p>
          </th>
          <th>
            <p xmlns:util="util">
              Definition
            </p>
          </th>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              <span class="parameter" sdata="paramReference">value</span>
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              The value of the array element.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              <span class="parameter" sdata="paramReference">index</span>
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              The numeric index of the array element.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              <span class="parameter" sdata="paramReference">array1</span>
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              The array object that contains the element.
            </p>
          </td>
        </tr>
      </table>
    </div>
  </div>
  <h3 class="subHeading">
    Modifying the Array Object
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      The array object can be modified by the callback function.
    </p>
    <p xmlns:util="util">
      The following table describes the results of modifying the array object after the <b>every</b> method starts.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Condition after the <b>every</b> method starts
            </p>
          </th>
          <th>
            <p xmlns:util="util">
              Element passed to callback function?
            </p>
          </th>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Element is added beyond the original length of the array.
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Element is added to fill in a missing element of the array.
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes, if that index has not yet been passed to the callback function.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Element is changed.
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes, if that element has not yet been passed to the callback function.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Element is deleted from the array.
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No, unless that element has already been passed to the callback function.
            </p>
          </td>
        </tr>
      </table>
    </div>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>every</b> method.
</p>

```
// Define the callback function. function CheckIfEven(value, index, ar) { document.write(value + " "); if (value % 2 == 0) return true; else return false; } // Create an array. var numbers = [2, 4,
5, 6, 8]; // Check whether the callback function returns true for all of the // array values. if (numbers.every(CheckIfEven)) document.write("All are even."); else document.write("Some are not
even."); // Output: // 2 4 5 Some are not even.
```

<p xmlns:util="util">
  The following example illustrates the use of the <span class="parameter" sdata="paramReference">thisArg</span> argument, which specifies an object to which the <span sdata="langKeyword" value=
  "this"><span class="keyword">this</span></span> keyword can refer.
</p>

```
// Create a function that returns true if the value is // numeric and within range. var checkNumericRange = function(value) { if (typeof value !== 'number') return false; else return value &gt;=
this.minimum &amp;&amp; value &lt;= this.maximum; } // Create an array of numbers. var numbers = [10, 15, 19]; // Check whether the callback function returns true for // all of the array values. //
The obj argument enables use of the this value // within the callback function. var obj = { minimum: 10, maximum: 20 } if (numbers.every(checkNumericRange, obj)) document.write ("All are within
range."); else document.write ("Some are not within range."); // Output: // All are within range.
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
    <span sdata="link" xmlns:util="util"><a href="7b6822f9-c406-4f4e-bfec-a93459745992.htm">some Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1d260370-9e6e-43fc-870f-2d35850db7ee.htm">filter Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Using Arrays (Windows Scripting - JScript)</span>
  </div>
</div>

