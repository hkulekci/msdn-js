---
title: map Method (Array) (JavaScript)
isChild: false
---

## map Method (Array) (JavaScript) {map_method_array_javascript_title}

### Introduction 

 Calls a defined callback function on each element of an array, and returns an array that contains the results.

### Syntax 

```
array1 .map(callbackfn [, thisArg ])
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
            Required. A function that accepts up to three arguments. The <b>map</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each
            element in the array.
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
    A new array in which each element is the callback function return value for the associated original array element.
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
    The <b>map</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each element in the array, in ascending index order. The callback function
    is not called for missing elements of the array.
  </p>
  <p xmlns:util="util">
    In addition to array objects, the <b>map</b> method can be used by any object that has a <span sdata="langKeyword" value="length"><span class="keyword">length</span></span> property and that has
    numerically indexed property names.
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
      The following table describes the results of modifying the array object after the <b>map</b> method starts.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Condition after the <b>map</b> method starts
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
  The following example illustrates the use of the <b>map</b> method.
</p>

```
// Define the callback function. function AreaOfCircle(radius) { var area = Math.PI * (radius * radius); return area.toFixed(0); } // Create an array. var radii = [10, 20, 30]; // Get the areas from
the radii. var areas = radii.map(AreaOfCircle); document.write(areas); // Output: // 314,1257,2827
```

<p xmlns:util="util">
  The following example illustrates the use of the <span class="parameter" sdata="paramReference">thisArg</span> argument, which specifies an object to which the <span sdata="langKeyword" value=
  "this"><span class="keyword">this</span></span> keyword can refer.
</p>

```
// Define an object that contains a divisor property and // a remainder function. var obj = { divisor: 10, remainder: function (value) { return value % this.divisor; } } // Create an array. var
numbers = [6, 12, 25, 30]; // Get the remainders. // The obj argument specifies the this value in the callback function. var result = numbers.map(obj.remainder, obj); document.write(result); //
Output: // 6,2,5,0
```

<p xmlns:util="util">
  In the following example, a built-inJavaScript method is used as the callback function.
</p>

```
// Apply Math.sqrt(value) to each element in an array. var numbers = [9, 16]; var result = numbers.map(Math.sqrt); document.write(result); // Output: 3,4
```

<p xmlns:util="util">
  The <b>map</b> method can be applied to a string. The following example illustrates this.
</p>

```
// Define the callback function. function threeChars(value, index, str) { // Create a string that contains the previous, current, // and next character. return str.substring(index - 1, index + 2); }
// Create a string. var word = "Thursday"; // Apply the map method to the string. // Each array element in the result contains a string that // has the previous, current, and next character. // The
commented out statement shows an alternative syntax. var result = [].map.call(word, threeChars); // var result = Array.prototype.map.call(word, threeChars); document.write(result); // Output: //
Th,Thu,hur,urs,rsd,sda,day,ay
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
    <span sdata="link" xmlns:util="util"><a href="003747e2-7860-4c96-b129-5180ae0fe745.htm">JavaScript Methods</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Using Arrays (Windows Scripting - JScript)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1d260370-9e6e-43fc-870f-2d35850db7ee.htm">filter Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="bd188034-a62b-4cbd-99c8-46d70dd6823d.htm">forEach Method (Array) (JavaScript)</a></span>
  </div>
</div>

