## [Array Object (JavaScript)](Array-Object.html)

### Introduction 

 Provides support for creation of arrays of any data type.

### Syntax 

```
arrayObj = new Array() arrayObj = new Array([size ]) arrayObj = new Array([element0 [, element1 [, ...[, elementN ]]]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arrayObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <b>Array</b> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">size</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The size of the array. As arrays are zero-based, created elements will have indexes from zero to <span class="parameter" sdata="paramReference">size</span> -1.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">element0,...,elementN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The elements to place in the array. This creates an array with <i>n</i> + 1 elements, and a <b>length</b> of <i>n</i> + 1. Using this syntax, you must supply more than one element.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    After an array is created, you can access the individual elements of the array by using [ ] notation. Note that arrays in JavaScript are zero-based.
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          JavaScript&nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 var my_array = new Array(); for (i = 0; i &lt; 10; i++) {     my_array[i] = i; } x = my_array[4]; document.write(x);  // Output: 4 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    You can pass an unsigned 32-bit integer to the <b>Array</b> constructor to specify the size of the array. If the value is negative or not an integer, a run-time error occurs. If you run the
    following code, you should see this error in the Console.
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          JavaScript&nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 var arr = new Array(10); document.write(arr.length  // Output: 10  // Don't do this var arr = new Array(-1); arr = new Array(1.50);  
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    If a single value is passed to the <b>Array</b> constructor, and it is not a number, the <b>length</b> property is set to 1, and the value of the only element becomes the single, passed-in
    argument.
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          &nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 var arr = new Array("one"); document.write(arr.length); document.write("&lt;br/&gt;"); document.write(arr[0]);  // Output: 1 one 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    JavaScript arrays are sparse arrays, which means that not all the elements in an array may contain data. In JavaScript, only the elements that actually contain data exist in the array. This
    reduces the amount of memory used by the array.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Array</b> object was introduced in
  </p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>. Some members in the following lists were introduced in later versions. For more information, see <span sdata="link">JavaScript Version Information</span> or the documentation for the
  individual members.
</div>

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the properties of the <b>Array</b> object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Property
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Description
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            constructor Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Specifies the function that creates an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            length Property (Array)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an integer value that is one higher than the highest element defined in an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            prototype Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a reference to the prototype for an array.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Functions 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table describes the functions of the <b>Array</b> object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Function
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Description
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Array.isArray Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether an object is an array.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Methods 

<div id="sectionSection3" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the methods of the <b>Array</b> object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Method
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Description
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            concat Method (Array)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a new array consisting of a combination of two arrays.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            every Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Checks whether a defined callback function returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> for all elements in an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            filter Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Calls a defined callback function on each element of an array, and returns an array of values for which the callback function returns <span sdata="langKeyword" value="true"><span class=
            "keyword">true</span></span>.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            forEach Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Calls a defined callback function for each element in an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            hasOwnProperty Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether an object has a property with the specified name.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            indexOf Method (Array)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the index of the first occurrence of a value in an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            isPrototypeOf Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether an object exists in another object's prototype chain.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            join Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object consisting of all the elements of an array concatenated together.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            lastIndexOf Method (Array)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the index of the last occurrence of a specified value in an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            map Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Calls a defined callback function on each element of an array, and returns an array that contains the results.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            pop Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Removes the last element from an array and returns it.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            propertyIsEnumerable Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether a specified property is part of an object and whether it is enumerable.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            push Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Appends new elements to an array, and returns the new length of the array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            reduce Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Accumulates a single result by calling a defined callback function for all elements in an array. The return value of the callback function is the accumulated result, and is provided as an
            argument in the next call to the callback function.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            reduceRight Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Accumulates a single result by calling a defined callback function for all elements in an array, in descending order. The return value of the callback function is the accumulated result,
            and is provided as an argument in the next call to the callback function.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            reverse Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an <b>Array</b> object with the elements reversed.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            shift Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Removes the first element from an array and returns it.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            slice Method (Array)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a section of an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            some Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Checks whether a defined callback function returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> for any element of an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            sort Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an <b>Array</b> object with the elements sorted.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            splice Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Removes elements from an array and, if necessary, inserts new elements in their place, returning the deleted elements.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toLocaleString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string using the current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string representation of an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            unshift Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Inserts new elements at the start of an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            valueOf Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets a reference to the array.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

