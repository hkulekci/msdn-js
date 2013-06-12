---
title: Number Object (JavaScript)
---

### Introduction 

 An object that represents a number of any kind. All JavaScript numbers are 64-bit floating-point numbers.

### Syntax 

```
numObj = new Number(value )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">numObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <b>Number</b> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">value</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The numeric value.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    JavaScript creates <b>Number</b> objects when a variable is set to a number value, for example <span class="code">var num = 255.336;</span>. It is seldom necessary to create <b>Number</b> objects
    explicitly.
  </p>
  <p xmlns:util="util">
    The <b>Number</b> object has its own properties and methods, in addition to the properties and methods inherited from <b>Object</b>. Numbers are converted into strings under certain
    circumstances, for example when a number is added or concatenated with a string, as well as by means of the <b>toString</b> method. For more information, see <span sdata="link"><a href=
    "ec1237d3-e78b-4e77-bd7d-c0204cf03acd.htm">Addition Operator (+) (JavaScript)</a></span>.
  </p>
  <p xmlns:util="util">
    JavaScript has several number constants. For a complete list, see <span sdata="link"><a href="e0701b41-99ae-4916-9ec0-f79bb15386fb.htm">Number Constants (JavaScript)</a></span>.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the properties of the <b>Number</b> object.
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
            Specifies the function that creates an object.
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
            Returns a reference to the prototype for a class of objects.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Methods 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the methods of the <b>Number</b> object.
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
            isPrototypeOf Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether an object exists in another object's prototype hierarchy.
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
            toExponential method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string that contains a number represented in exponential notation.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toFixed method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string that represents a number in fixed-point notation.
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
            Returns an object converted to a string based on the current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toPrecision method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string that contains a number that is represented in either exponential or fixed-point notation and that has a specified number of digits.
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
            Returns a string representation of an object.
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
            Returns the primitive value of the specified object.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4a29a831-41c9-4843-9385-c3879e385585.htm">JavaScript Objects</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="607b94cb-921c-43cd-b514-fdbc13aeced6.htm">Math Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="5ea556ba-7ae6-426c-8430-9032eee5a0a5.htm">new Operator (JavaScript)</a></span>
  </div>
</div>

