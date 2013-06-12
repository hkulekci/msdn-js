---
title: forEach Method (Array) (JavaScript)
---

### Introduction 

 Performs the specified action for each element in an array.

### Syntax 

```
array1 .forEach(callbackfn [, thisArg ])
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
            Required. A function that accepts up to three arguments. <b>forEach</b> calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each element in
            the array.
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

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the <span class="parameter" sdata="paramReference">callbackfn</span> argument is not a function object, a <b>TypeError</b> exception is thrown.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>forEach</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each element present in the array, in ascending index order. The
    callback function is not called for missing elements of the array.
  </p>
  <p xmlns:util="util">
    In addition to array objects, the <b>forEach</b> method can be used by any object that has a <span sdata="langKeyword" value="length"><span class="keyword">length</span></span> property and that
    has numerically indexed property names.
  </p>
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
      You can declare the callback function by using up to three parameters.
    </p>
    <p xmlns:util="util">
      The callback function parameters are as follows.
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
      The <b>forEach</b> method does not directly modify the original array, but the callback function might modify it. The following table describes the results of modifying the array object after
      the <b>forEach</b> method starts.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Condition after <b>forEach</b> method starts
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
  The following example illustrates use of the <b>forEach</b> method.
</p>

```
// Define the callback function. function ShowResults(value, index, ar) { document.write("value: " + value); document.write(" index: " + index); document.write("&lt;br /&gt;"); } // Create an array.
var letters = ['ab', 'cd', 'ef']; // Call the ShowResults callback function for each // array element. letters.forEach(ShowResults); // Output: // value: ab index: 0 // value: cd index: 1 // value:
ef index: 2
```

<p xmlns:util="util">
  In the following example, the <span class="parameter" sdata="paramReference">callbackfn</span> argument includes the code of the callback function.
</p>

```
// Create an array. var numbers = [10, 11, 12]; // Call the addNumber callback function for each array element. var sum = 0; numbers.forEach( function addNumber(value) { sum += value; } );
document.write(sum); // Output: 33
```

<p xmlns:util="util">
  The following example illustrates the use of the <span class="parameter" sdata="paramReference">thisArg</span> argument, which specifies an object that can be referred to with the <span sdata=
  "langKeyword" value="this"><span class="keyword">this</span></span> keyword.
</p>

```
// Define the object that contains the callback function. var obj = { showResults: function(value, index) { // Call calcSquare by using the this value. var squared = this.calcSquare(value);
document.write("value: " + value); document.write(" index: " + index); document.write(" squared: " + squared); document.write("&lt;br /&gt;"); }, calcSquare: function(x) { return x * x } }; // Define
an array. var numbers = [5, 6]; // Call the showResults callback function for each array element. // The obj is the this value within the // callback function. numbers.forEach(obj.showResults, obj);
// Embed the callback function in the forEach statement. // The obj argument is the this value within the obj object. // The output is the same as for the previous statement.
numbers.forEach(function(value, index) { this.showResults(value, index) }, obj); // Output: // value: 5 index: 0 squared: 25 // value: 6 index: 1 squared: 36 // value: 5 index: 0 squared: 25 //
value: 6 index: 1 squared: 36
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
    <span sdata="link" xmlns:util="util"><a href="1d260370-9e6e-43fc-870f-2d35850db7ee.htm">filter Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="500dc4f8-d73d-4a28-a5b8-c9bd5674ea36.htm">map Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7b6822f9-c406-4f4e-bfec-a93459745992.htm">some Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Using Arrays (Windows Scripting - JScript)</span>
  </div>
</div>

