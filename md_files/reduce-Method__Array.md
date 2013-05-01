## [reduce Method (Array) (JavaScript)](reduce-Method__Array.html)

### Introduction 

 Calls the specified callback function for all the elements in an array. The return value of the callback function is the accumulated result, and is provided as an argument in the next call to the
callback function.

### Syntax 

```
array1 .reduce(callbackfn [, initialValue ])
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
            Required. A function that accepts up to four arguments. The <b>reduce</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each
            element in the array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">initialValue</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Optional. If <span class="parameter" sdata="paramReference">initialValue</span> is specified, it is used as the initial value to start the accumulation. The first call to the <span class=
            "parameter" sdata="paramReference">callbackfn</span> function provides this value as an argument instead of an array value.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The accumulated result from the last call to the callback function.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    A <b>TypeError</b> exception is thrown when either of the following conditions is true:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        The <span class="parameter" sdata="paramReference">callbackfn</span> argument is not a function object.
      </p>
    </li>
    <li>
      <p>
        The array contains no elements and <span class="parameter" sdata="paramReference">initialValue</span> is not provided.
      </p>
    </li>
  </ul>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If an <span class="parameter" sdata="paramReference">initialValue</span> is provided, the <b>reduce</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function
    one time for each element present in the array, in ascending index order. If an <span class="parameter" sdata="paramReference">initialValue</span> is not provided, the <b>reduce</b> method calls
    the <span class="parameter" sdata="paramReference">callbackfn</span> function on each element, starting with the second element.
  </p>
  <p xmlns:util="util">
    The return value of the callback function is provided as the <span class="parameter" sdata="paramReference">previousValue</span> argument on the next call to the callback function. The return
    value of the last call to the callback function is the return value of the <b>reduce</b> method.
  </p>
  <p xmlns:util="util">
    The callback function is not called for missing elements of the array.
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
            The <span sdata="link"><a href="85963761-da11-407c-8bce-278c930e61bd.htm">reduceRight Method (Array) (JavaScript)</a></span> processes the elements in descending index order.
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
      <span class="code">function callbackfn(previousValue, currentValue, currentIndex, array1)</span>
    </p>
    <p xmlns:util="util">
      You can declare the callback function by using up to four parameters.
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
              Callback argument
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
              <span class="parameter" sdata="paramReference">previousValue</span>
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              The value from the previous call to the callback function. If an <span class="parameter" sdata="paramReference">initialValue</span> is provided to the <b>reduce</b> method, the
              <span class="parameter" sdata="paramReference">previousValue</span> is <span class="parameter" sdata="paramReference">initialValue</span> the first time the function is called.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              <span class="parameter" sdata="paramReference">currentValue</span>
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              The value of the current array element.
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              <span class="parameter" sdata="paramReference">currentIndex</span>
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              The numeric index of the current array element.
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
    First Call to the Callback Function
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      The first time the callback function is called, the values provided as arguments depend on whether the <b>reduce</b> method has an <span class="parameter" sdata=
      "paramReference">initialValue</span> argument.
    </p>
    <p xmlns:util="util">
      If an <span class="parameter" sdata="paramReference">initialValue</span> is provided to the reduce method:
    </p>
    <ul xmlns:util="util">
      <li>
        <p>
          The <span class="parameter" sdata="paramReference">previousValue</span> argument is <span class="parameter" sdata="paramReference">initialValue</span>.
        </p>
      </li>
      <li>
        <p>
          The <span class="parameter" sdata="paramReference">currentValue</span> argument is the value of the first element present in the array.
        </p>
      </li>
    </ul>
    <p xmlns:util="util">
      If an <span class="parameter" sdata="paramReference">initialValue</span> is not provided:
    </p>
    <ul xmlns:util="util">
      <li>
        <p>
          The <span class="parameter" sdata="paramReference">previousValue</span> argument is the value of the first element present in the array.
        </p>
      </li>
      <li>
        <p>
          The <span class="parameter" sdata="paramReference">currentValue</span> argument is the value of the second element present in the array.
        </p>
      </li>
    </ul>
  </div>
  <h3 class="subHeading">
    Modifying the Array Object
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      The array object can be modified by the callback function.
    </p>
    <p xmlns:util="util">
      The following table describes the results of modifying the array object after the <b>reduce</b> method starts.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Condition after the <b>reduce</b> method starts
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
  The following example concatenates array values into a string, separating the values with "::". Because no initial value is provided to the <b>reduce</b> method, the first call to the callback
  function has "abc" as the <span class="parameter" sdata="paramReference">previousValue</span> argument and "def" as the <span class="parameter" sdata="paramReference">currentValue</span> argument.
</p>

```
// Define the callback function. function appendCurrent (previousValue, currentValue) { return previousValue + "::" + currentValue; } // Create an array. var elements = ["abc", "def", 123, 456]; //
Call the reduce method, which calls the callback function // for each array element. var result = elements.reduce(appendCurrent); document.write(result); // Output: // abc::def::123::456
```

<p xmlns:util="util">
  The following example adds the values of an array after they have been rounded. The <b>reduce</b> method is called with an initial value of 0.
</p>

```
// Define the callback function. function addRounded (previousValue, currentValue) { return previousValue + Math.round(currentValue); } // Create an array. var numbers = [10.9, 15.4, 0.5]; // Call
the reduce method, starting with an initial value of 0. var result = numbers.reduce(addRounded, 0); document.write (result); // Output: 27
```

<p xmlns:util="util">
  The following example adds the values in an array. The <span class="parameter" sdata="paramReference">currentIndex</span> and <span class="parameter" sdata="paramReference">array1</span> parameters
  are used in the callback function.
</p>

```
function addDigitValue(previousValue, currentDigit, currentIndex, array) { var exponent = (array.length - 1) - currentIndex; var digitValue = currentDigit * Math.pow(10, exponent); return
previousValue + digitValue; } var digits = [4, 1, 2, 5]; // Determine an integer that is computed from values in the array. var result = digits.reduce(addDigitValue, 0); document.write (result); //
Output: 4125
```

<p xmlns:util="util">
  The following example gets an array that contains only those values that are between 1 and 10 in another array. The initial value provided to the <b>reduce</b> method is an empty array.
</p>

```
function Process(previousArray, currentValue) { // If currentValue is between 1 and 10, // append currentValue to the array. var nextArray; if (currentValue &gt;= 1 &amp;&amp; currentValue &lt;= 10)
nextArray = previousArray.concat(currentValue); else nextArray = previousArray; // If this is not the last call by the reduce method, // the returned array is previousArray on the next call. // If
this is the last call by the reduce method, the // returned array is the return value of the reduce method. return nextArray; } // Create an array. var numbers = [20, 1, -5, 6, 50, 3]; // Call the
reduce method, starting with an initial empty array. var emptyArray = new Array(); var resultArray = numbers.reduce(Process, emptyArray); document.write("result array=" + resultArray); // Output: //
result array=1,6,3
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
    <span sdata="link" xmlns:util="util"><a href="85963761-da11-407c-8bce-278c930e61bd.htm">reduceRight Method (Array) (JavaScript)</a></span>
  </div>
</div>

