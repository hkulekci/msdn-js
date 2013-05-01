## [Logical OR Operator (||) (JavaScript)](Logical-OR-Operator.html)

### Introduction 

 Performs a logical disjunction on two expressions.

### Syntax 

```
result = expression1 || expression2
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
      <i xmlns:util="util">expression1</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any expression.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">expression2</i>
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
    If either or both expressions evaluate to <b>True</b>, <i>result</i> is <b>True</b>. The following table illustrates how <i>result</i> is determined:
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            If <span class="code">expression1</span> is
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            And <span class="code">expression2</span> is
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            The <span class="code">result</span> is
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
            True
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            True
          </p>
        </td>
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
        <td>
          <p xmlns:util="util">
            True
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
        <td>
          <p xmlns:util="util">
            True
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
            False
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            False
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    JavaScript uses the following rules for converting non-Boolean values to Boolean values:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        All objects are considered true.
      </p>
    </li>
    <li>
      <p>
        Strings are considered false if and only if they are empty.
      </p>
    </li>
    <li>
      <p>
        <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> and undefined are considered false.
      </p>
    </li>
    <li>
      <p>
        Numbers are false if, and only if, they are 0.
      </p>
    </li>
  </ul>
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

