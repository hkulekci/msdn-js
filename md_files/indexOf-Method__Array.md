## [indexOf Method (Array) (JavaScript)](indexOf-Method__Array.html)

### Introduction 

 Returns the index of the first occurrence of a value in an array.

### Syntax 

```
array1 .indexOf(searchElement [, fromIndex ])
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
            <span class="parameter" sdata="paramReference">searchElement</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Required. The value to locate in <span class="parameter" sdata="paramReference">array1</span>.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">fromIndex</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Optional. The array index at which to begin the search. If <span class="parameter" sdata="paramReference">fromIndex</span> is omitted, the search starts at index 0.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The index of the first occurrence of <span class="parameter" sdata="paramReference">searchElement</span> in the array, or -1 if <span class="parameter" sdata="paramReference">searchElement</span>
    is not found.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>indexOf</b> method searches an array for a specified value. The method returns the index of the first occurrence, or -1 if the specified value is not found.
  </p>
  <p xmlns:util="util">
    The search occurs in ascending index order.
  </p>
  <p xmlns:util="util">
    The array elements are compared to the <span class="parameter" sdata="paramReference">searchElement</span> value by strict equality, similar to the <span sdata="langKeyword" value=
    "==="><span class="keyword">===</span></span> operator. For more information, see <span sdata="link"><a href="084f90f0-d010-47cf-96dd-13d637fc9b68.htm">Comparison Operators
    (JavaScript)</a></span>.
  </p>
  <p xmlns:util="util">
    The optional <span class="parameter" sdata="paramReference">fromIndex</span> argument specifies the array index at which to begin the search. If <span class="parameter" sdata=
    "paramReference">fromIndex</span> is greater than or equal to the array length, -1 is returned. If <span class="parameter" sdata="paramReference">fromIndex</span> is negative, the search starts
    at the array length plus <span class="parameter" sdata="paramReference">fromIndex</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following examples illustrate the use of the <b>indexOf</b> method.
</p>

```
// Create an array. (The elements start at index 0.) var ar = ["ab", "cd", "ef", "ab", "cd"]; // Determine the first location of "cd". document.write(ar.indexOf("cd") + "&lt;br/&gt;"); // Output: 1
// Find "cd" starting at index 2. document.write(ar.indexOf("cd", 2) + "&lt;br/&gt;"); // Output: 4 // Find "gh" (which is not found). document.write (ar.indexOf("gh")+ "&lt;br/&gt;"); // Output: -1
// Find "ab" with a fromIndex argument of -2. // The search starts at index 3, which is the array length plus -2. document.write (ar.indexOf("ab", -2) + "&lt;br/&gt;"); // Output: 3
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
</div>

