## [Subtraction Operator (-) (JavaScript)](Subtraction-Operator.html)

### Introduction 

 Subtracts the value of one expression from another or provides unary negation of a single expression.

### Syntax 

```
result = number1 - number2 ;
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">result</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any numeric variable.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">number</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any numeric expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">number1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any numeric expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">number2</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any numeric expression.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    In Syntax 1, the <b>-</b> operator is the arithmetic subtraction operator used to find the difference between two numbers. In Syntax 2, the <b>-</b> operator is used as the unary negation
    operator to indicate the negative value of an expression.
  </p>
  <p xmlns:util="util">
    For Syntax 2, as for all unary operators, expressions are evaluated as follows:
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
    The operator is applied to the resulting number. In Syntax 2, if the resulting number is nonzero, <i>result</i> is equal to the resulting number with its sign reversed. If the resulting number is
    zero, <i>result</i> is zero.
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
    <span sdata="link" xmlns:util="util"><a href="a03adbd8-75fa-4633-80c5-f7215332a8ef.htm">Subtraction Assignment Operator (-=) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

