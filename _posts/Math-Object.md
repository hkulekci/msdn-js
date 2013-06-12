---
title: Math Object (JavaScript)
isChild: false
---

## Math Object (JavaScript) {math_object_javascript_title}

### Introduction 

 An intrinsic object that provides basic mathematics functionality and constants.

### Syntax 

```
Math.[{property | method }]
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">property</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Name of one of the properties of the <b>Math</b>. object.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">method</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Name of one of the methods of the <b>Math</b>. object.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Math</b> object cannot be created using the <b>new</b> operator, and gives an error if you attempt to do so. The scripting engine creates it when the engine is loaded. All of its methods
    and properties are available to your script at all times.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Math</b> object was introduced in Internet Explorer before Internet Explorer 6.
  </p>
</div>

#### Constants 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the constants of the <b>Math</b> object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Constant
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
            Math.E Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The mathematical constant e. This is Euler's number, the base of natural logarithms.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.LN2 Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The natural logarithm of 2.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.LN10 Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The natural logarithm of 10.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.LOG2E Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The base-2 logarithm of e.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.LOG10E Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The base-10 logarithm of e.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.PI Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Pi. This is the ratio of the circumference of a circle to its diameter.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.SQRT1_2 Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The square root of 0.5, or, equivalently, one divided by the square root of 2.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.SQRT2 Constant
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The square root of 2.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Functions 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the functions of the <b>Math</b> object.
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
            Math.abs Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the absolute value of a number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.acos Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the arccosine of a number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.asin Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the arcsine of a number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.atan Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the arctangent of a number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.atan2 Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the angle (in radians) from the X axis to a point represented by the supplied y and x coordinates.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.ceil Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the smallest integer that is greater than or equal to the supplied numeric expression.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.cos Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the cosine of a number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.exp Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns <i>e</i> (the base of natural logarithms) raised to a power.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.floor Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the greatest integer that is less than or equal to the supplied numeric expression.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.log Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the natural logarithm of a number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.max Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the greater of two supplied numeric expressions.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.min Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the lesser of two supplied numbers.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.pow Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the value of a base expression raised to a specified power.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.random Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a pseudorandom number between 0 and 1.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.round Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a specified numeric expression rounded to the nearest integer.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.sin Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the sine of a number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.sqrt Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the square root of a number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Math.tan Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the tangent of a number.
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
    <span sdata="link" xmlns:util="util"><a href="76e87c37-cf6c-46cc-bafa-04be1fe3d78d.htm">Number Object (JavaScript)</a></span>
  </div>
</div>

