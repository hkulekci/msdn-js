---
title: Addition Assignment Operator (+=) (JavaScript)
isChild: false
---

## Addition Assignment Operator (+=) (JavaScript) {addition_assignment_operator_plusequal_javascript_title}

### Introduction 

 Adds the value of an expression to the value of a variable and assigns the result to the variable.

### Syntax 

```
result += expression
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">result</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any variable.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any expression.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Using this operator is exactly the same as specifying: <span class="code">result = result + expression</span>.
  </p>
  <p xmlns:util="util">
    The types of the two expressions determine the behavior of the <span sdata="langKeyword" value="+="><span class="keyword">+=</span></span> operator.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            If
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Then
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Both expressions are numeric or Boolean
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Add
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Both expressions are strings
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Concatenate
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            One expression is numeric and the other is a string
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Concatenate
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ec1237d3-e78b-4e77-bd7d-c0204cf03acd.htm">Addition Operator (+) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

