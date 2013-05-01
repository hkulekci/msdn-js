## [reduceRight Method (Array) (JavaScript)](reduceRight-Method__Array.html)

### Introduction 

 Calls the specified callback function for all the elements in an array, in descending order. The return value of the callback function is the accumulated result, and is provided as an argument in the
next call to the callback function.

### Syntax 

```
array1 .reduceRight(callbackfn [, initialValue ])
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
            Required. A function that accepts up to four arguments. The <b>reduceRight</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each
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
    An object that contains the accumulated result from the last call to the callback function.
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
    If an <span class="parameter" sdata="paramReference">initialValue</span> is provided, the <b>reduceRight</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span>
    function one time for each element in the array, in descending index order. If no <span class="parameter" sdata="paramReference">initialValue</span> is provided, the <b>reduceRight</b> method
    calls the <span class="parameter" sdata="paramReference">callbackfn</span> function on each element, starting with the second-to-last element, in descending index order.
  </p>
  <p xmlns:util="util">
    The return value of the callback function is provided as the <span class="parameter" sdata="paramReference">previousValue</span> argument on the next call to the callback function. The return
    value of the last call to the callback function is the return value of the <b>reduceRight</b> method.
  </p>
  <p xmlns:util="util">
    The callback function is not called for missing elements of the array.
  </p>
  <p xmlns:util="util">
    To accumulate a result in ascending index order, use the <span sdata="link"><a href="48d069e0-e083-494f-86d5-d459d2377dc5.htm">reduce Method (Array) (JavaScript)</a></span>.
  </p>
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
              The value from the previous call to the callback function. If an <span class="parameter" sdata="paramReference">initialValue</span> is provided to the <b>reduceRight</b> method, the
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
      The first time the callback function is called, the values provided as arguments depend on whether the <b>reduceRight</b> method has an <span class="parameter" sdata=
      "paramReference">initialValue</span> argument.
    </p>
    <p xmlns:util="util">
      If an <span class="parameter" sdata="paramReference">initialValue</span> is provided to the <b>reduceRight</b> method:
    </p>
    <ul xmlns:util="util">
      <li>
        <p>
          The <span class="parameter" sdata="paramReference">previousValue</span> argument is <span class="parameter" sdata="paramReference">initialValue</span>.
        </p>
      </li>
      <li>
        <p>
          The <span class="parameter" sdata="paramReference">currentValue</span> argument is the value of the last element present in the array.
        </p>
      </li>
    </ul>
    <p xmlns:util="util">
      If an <span class="parameter" sdata="paramReference">initialValue</span> is not provided:
    </p>
    <ul xmlns:util="util">
      <li>
        <p>
          The <span class="parameter" sdata="paramReference">previousValue</span> argument is the value of the last element present in the array.
        </p>
      </li>
      <li>
        <p>
          The <span class="parameter" sdata="paramReference">currentValue</span> argument is the value of the second-to-last element present in the array.
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
      The following table describes the results of modifying the array object after the <b>reduceRight</b> method starts.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Condition after the <b>reduceRight</b> method starts
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
  The following example concatenates array values into a string, separating the values with "::". Because no initial value is provided to the <b>reduceRight</b> method, the first call to the callback
  function has 456 as the <span class="parameter" sdata="paramReference">previousValue</span> argument and 123 as the <span class="parameter" sdata="paramReference">currentValue</span> argument.
</p>

```
// Define the callback function. function appendCurrent (previousValue, currentValue) { return previousValue + "::" + currentValue; } // Create an array. var elements = ["abc", "def", 123, 456]; //
Call the reduceRight method, which calls the callback function // for each array element, in descending index order. var result = elements.reduceRight(appendCurrent); document.write(result); //
Output: // 456::123::def::abc
```

<p xmlns:util="util">
  The following example finds the sum of the squares of the array elements. The <b>reduceRight</b> method is called with an initial value of 0.
</p>

```
// Define the callback function. function Process(previousValue, currentValue, index, array) { // Add the previous value to the current value squared. var nextValue = previousValue + (currentValue *
currentValue); // If this is not the last call by the reduceRight method, // the return value is previousValue on the next call. // If this is the last call by the reduceRight method, the // return
value is the return value of the reduceRight method. return nextValue; } // Create an array. var numbers = [3, 4, 5]; // Call the reduceRight method with an initial value of 0. var sumOfSquares =
numbers.reduceRight(Process, 0); document.write("sum of squares=" + sumOfSquares); // Output: // sum of squares=50
```

<p xmlns:util="util">
  The following example gets those elements of an array whose values are between 1 and 10. The initial value provided to the <b>reduceRight</b> method is an empty array.
</p>

```
function Process2(previousArray, currentValue) { // If currentValue is between 1 and 10, // append currentValue to the array. var nextArray; if (currentValue &gt;= 1 &amp;&amp; currentValue &lt;= 10)
nextArray = previousArray.concat(currentValue); else nextArray = previousArray; // If this is not the last call by the reduceRight method, // the returned array is previousArray on the next call. //
If this is the last call by the reduceRight method, the // returned array is the return value of the reduceRight method. return nextArray; } // Create an array. var numbers = [20, 1, -5, 6, 50, 3];
// Call the reduceRight method, starting with an empty array. var emptyArray = new Array(); var resultArray = numbers.reduceRight(Process2, emptyArray); document.write("result array=" + resultArray);
// Output: // result array=3,6,1
```

<p xmlns:util="util">
  The <b>reduceRight</b> method can be applied to a string. The following example shows how to use this method to reverse the characters in a string.
</p>

```
// Define the callback function. function AppendToArray(previousValue, currentValue) { return previousValue + currentValue; } var word = "retupmoc"; // Create a string that reverses the characters of
another string. // The commented-out statement shows an alternative syntax. var result = [].reduceRight.call(word, AppendToArray, "the "); // var result = Array.prototype.reduceRight.call(word,
AppendToArray, "the "); document.write(result); // Output: // the computer
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
    <span sdata="link" xmlns:util="util"><a href="48d069e0-e083-494f-86d5-d459d2377dc5.htm">reduce Method (Array) (JavaScript)</a></span>
  </div>
</div>

