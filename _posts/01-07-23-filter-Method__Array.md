---
title: filter Method (Array) (JavaScript)
---

### Introduction 

 Returns the elements of an array that meet the condition specified in a callback function.

### Syntax 

```
array1 .filter(callbackfn [, thisArg ])
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
            Required. A function that accepts up to three arguments. The <b>filter</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each
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
    A new array that contains all the values for which the callback function returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>. If the callback function returns
    <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> for all elements of <span class="parameter" sdata="paramReference">array1</span>, the length of the new array is
    0.
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
    The <b>filter</b> method calls the <span class="parameter" sdata="paramReference">callbackfn</span> function one time for each element in the array, in ascending index order. The callback
    function is not called for missing elements of the array.
  </p>
  <p xmlns:util="util">
    In addition to array objects, the <b>filter</b> method can be used by any object that has a <span sdata="langKeyword" value="length"><span class="keyword">length</span></span> property and that
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
      The <b>filter</b> method does not directly modify the original array, but the callback function might modify it. The following table describes the results of modifying the array object after
      the <b>filter</b> method starts.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Condition after the <b>filter</b> method starts
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
  The following example shows how to use the <b>filter</b> method.
</p>

```
// Define a callback function. function CheckIfPrime(value, index, ar) { high = Math.floor(Math.sqrt(value)) + 1; for (var div = 2; div &lt;= high; div++) { if (value % div == 0) { return false; } }
return true; } // Create the original array. var numbers = [31, 33, 35, 37, 39, 41, 43, 45, 47, 49, 51, 53]; // Get the prime numbers that are in the original array. var primes =
numbers.filter(CheckIfPrime); document.write(primes); // Output: 31,37,41,43,47,53
```

<p xmlns:util="util">
  In the following example, the <span class="parameter" sdata="paramReference">callbackfn</span> argument includes the code of the callback function.
</p>

```
// Create the original array. var arr = [5, "element", 10, "the", true]; // Create an array that contains the string // values that are in the original array. var result = arr.filter( function
(value) { return (typeof value === 'string'); } ); document.write(result); // Output: element, the
```

<p xmlns:util="util">
  The following example displays the names of properties that start with the letter "css" in the <span class="code">window</span> DOM object.
</p>

```
var filteredNames = Object.getOwnPropertyNames(window).filter(IsC); for (i in filteredNames) document.write(filteredNames[i] + "&lt;br/&gt;"); // Check whether the string starts with "css". function
IsC(value) { var firstChar = value.substr(0, 3); if (firstChar.toLowerCase() == "css") return true; else return false; } // Output: // CSSRule // CSSFontFaceRule // CSSImportRule // CSSMediaRule //
CSSNamespaceRule // CSSPageRule // CSSRuleList // CSSStyleDeclaration // CSSStyleRule // CSSStyleSheet
```

<p xmlns:util="util"></p>

```
var checkNumericRange = function(value) { if (typeof value !== 'number') return false; else return value &gt;= this.minimum &amp;&amp; value &lt;= this.maximum; } var numbers = [6, 12, "15", 16,
"the", -12]; // The obj argument enables use of the this value // within the callback function. var obj = { minimum: 10, maximum: 20 } var result = numbers.filter(checkNumericRange, obj);
document.write(result); // Output: 12,16
```

<p xmlns:util="util">
  The following example illustrates the use of the <span class="parameter" sdata="paramReference">thisArg</span> argument, which specifies an object to which the <span sdata="langKeyword" value=
  "this"><span class="keyword">this</span></span> keyword can refer.
</p>

```
// Define a callback function that returns true // if the current array element follows a space // or is the first character. function CheckValue(value, index, ar) { if (index == 0) return true; else
return ar[index - 1] === " "; } // Create a string. var sentence = "The quick brown fox jumps over the lazy dog."; // Create an array that contains all characters that follow a space. var subset =
[].filter.call(sentence, CheckValue); // You can use this alternative syntax. //var subset = Array.prototype.filter.call(sentence, CheckValue); document.write(subset); // Output: T,q,b,f,j,o,t,l,d
```

<p xmlns:util="util">
  The <b>filter</b> method can be applied to a string instead of an array. The following example shows how to do this.
</p>

```
<p xmlns:util="util">
  The <b>filter</b> method can be applied to a string instead of an array. The following example shows how to do this.
</p>
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
    <span sdata="link" xmlns:util="util"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Using Arrays (Windows Scripting - JScript)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="500dc4f8-d73d-4a28-a5b8-c9bd5674ea36.htm">map Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="bd188034-a62b-4cbd-99c8-46d70dd6823d.htm">forEach Method (Array) (JavaScript)</a></span>
  </div>
</div>

