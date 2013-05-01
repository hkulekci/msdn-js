## [Logical NOT Operator (!) (JavaScript)](Logical-NOT-Operator.html)

### Introduction 

 Performs logical negation on an expression.

### Syntax 

```
result = !expression
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">result</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any variable.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">expression</i>
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
    The following table illustrates how <i>result</i> is determined.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            If <span class="code">expression</span> is
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Then <span class="code">result</span> is
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            True
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            False
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            False
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            True
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    All unary operators, such as the <b>!</b> operator, evaluate expressions as follows:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        If applied to undefined or <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> expressions, a run-time error is raised.
      </p>
    </li>
    <li>
      <p>
        Objects are converted to strings.
      </p>
    </li>
    <li>
      <p>
        Strings are converted to numbers if possible. If not, a run-time error is raised.
      </p>
    </li>
    <li>
      <p>
        Boolean values are treated as numbers (0 if false, 1 if true).
      </p>
    </li>
  </ul>
  <p xmlns:util="util">
    The operator is applied to the resulting number.
  </p>
  <p xmlns:util="util">
    For the <b>!</b> operator, if <i>expression</i> is nonzero, <i>result</i> is zero. If <i>expression</i> is zero, <i>result</i> is 1.
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

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="39f92474-fe05-4a8b-9ad8-caca93f82bca.htm">Bitwise NOT Operator (~) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

