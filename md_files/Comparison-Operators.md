## [Comparison Operators (JavaScript)](Comparison-Operators.html)

### Introduction 

 Returns a Boolean value indicating the result of the comparison.

### Syntax 

```
expression1 comparisonoperator expression2
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">comparisonoperator</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any comparison operator.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression2</span>
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
    When comparing strings, JavaScript uses the Unicode character value of the string expression.
  </p>
  <p xmlns:util="util">
    The following describes how the different groups of operators behave depending on the types and values of <span class="parameter" sdata="paramReference">expression1</span> and <span class=
    "parameter" sdata="paramReference">expression2</span>:
  </p>
  <p xmlns:util="util">
    Relational operators: <b>&lt;</b>, <b>&gt;</b>, <b>&lt;=</b>, <b>&gt;=</b>
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        Attempt to convert both <span class="parameter" sdata="paramReference">expression1</span> and <span class="parameter" sdata="paramReference">expression2</span> into numbers.
      </p>
    </li>
    <li>
      <p>
        If both expressions are strings, do a string comparison.
      </p>
    </li>
    <li>
      <p>
        If either expression is <b>NaN</b>, return <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>.
      </p>
    </li>
    <li>
      <p>
        Negative zero equals Positive zero.
      </p>
    </li>
    <li>
      <p>
        Negative Infinity is less than everything including itself.
      </p>
    </li>
    <li>
      <p>
        Positive Infinity is greater than everything including itself.
      </p>
    </li>
  </ul>
  <p xmlns:util="util">
    Equality operators: <b>==</b>, <b>!=</b>
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        If the types of the two expressions are different, attempt to convert them to a String, Number, or Boolean.
      </p>
    </li>
    <li>
      <p>
        <b>NaN</b> is not equal to anything including itself.
      </p>
    </li>
    <li>
      <p>
        Negative zero equals positive zero.
      </p>
    </li>
    <li>
      <p>
        <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> equals both <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> and <span sdata=
        "langKeyword" value="undefined"><span class="keyword">undefined</span></span>.
      </p>
    </li>
    <li>
      <p>
        Values are considered equal if they are identical strings, numerically equivalent numbers, the same object, identical Boolean values, or (if different types) they can be coerced into one of
        these situations.
      </p>
    </li>
    <li>
      <p>
        Every other comparison is considered unequal.
      </p>
    </li>
  </ul>
  <p xmlns:util="util">
    Identity operators: <b>===</b>, <b>!==</b>
  </p>
  <p xmlns:util="util">
    These operators behave the same as the equality operators, except that no type conversion is done. If the types of both expressions are not the same, these expressions always return <span sdata=
    "langKeyword" value="false"><span class="keyword">false</span></span>.
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
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

