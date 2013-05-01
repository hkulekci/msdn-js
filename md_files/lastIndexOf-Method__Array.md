## [lastIndexOf Method (Array) (JavaScript)](lastIndexOf-Method__Array.html)

### Introduction 

 Returns the index of the last occurrence of a specified value in an array.

### Syntax 

```
array1 .lastIndexOf(searchElement [, fromIndex ])
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
            Required. The array object to search.
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
            Optional. The array index at which to begin the search. If <span class="parameter" sdata="paramReference">fromIndex</span> is omitted, the search starts at the last index in the array.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The index of the last occurrence of <span class="parameter" sdata="paramReference">searchElement</span> in the array, or -1 if <span class="parameter" sdata="paramReference">searchElement</span>
    is not found.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>lastIndexOf</b> method searches an array for a specified value. The method returns the index of the first occurrence, or -1 if the specified value is not found.
  </p>
  <p xmlns:util="util">
    The search occurs in descending index order (last member first). To search in ascending order, use the <span sdata="link"><a href="5bee31ae-aaf1-4466-8cfd-ed287e3cdf17.htm">indexOf Method (Array)
    (JavaScript)</a></span>.
  </p>
  <p xmlns:util="util">
    The array elements are compared to the <span class="parameter" sdata="paramReference">searchElement</span> value by strict equality, similar to the comparison made by the <span sdata=
    "langKeyword" value="==="><span class="keyword">===</span></span> operator. For more information, see <span sdata="link"><a href="084f90f0-d010-47cf-96dd-13d637fc9b68.htm">Comparison Operators
    (JavaScript)</a></span>.
  </p>
  <p xmlns:util="util">
    The optional <span class="parameter" sdata="paramReference">fromIndex</span> argument specifies the array index at which to begin the search. If <span class="parameter" sdata=
    "paramReference">fromIndex</span> is greater than or equal to the array length, the whole array is searched. If <span class="parameter" sdata="paramReference">fromIndex</span> is negative, the
    search starts at the array length plus <span class="parameter" sdata="paramReference">fromIndex</span>. If the computed index is less than 0, -1 is returned.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following examples illustrate the use of the <b>lastIndexOf</b> method.
</p>

```
// Create an array. var ar = ["ab", "cd", "ef", "ab", "cd"]; // Determine the first location, in descending order, of "cd". document.write(ar.lastIndexOf("cd") + "&lt;br/&gt;"); // Output: 4 // Find
"cd" in descending order, starting at index 2. document.write(ar.lastIndexOf("cd", 2) + "&lt;br/&gt;"); // Output: 1 // Search for "gh" (which is not found). document.write(ar.lastIndexOf("gh")+
"&lt;br/&gt;"); // Output: -1 // Find "ab" with a fromIndex argument of -3. // The search in descending order starts at index 3, // which is the array length minus 2.
document.write(ar.lastIndexOf("ab", -3) + "&lt;br/&gt;"); // Output: 0
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
    <span sdata="link" xmlns:util="util"><a href="5bee31ae-aaf1-4466-8cfd-ed287e3cdf17.htm">indexOf Method (Array) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Using Arrays (Windows Scripting - JScript)</span>
  </div>
</div>

