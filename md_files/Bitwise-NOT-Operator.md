## [Bitwise NOT Operator (~) (JavaScript)](Bitwise-NOT-Operator.html)

### Introduction 

 Performs a bitwise NOT (negation) on an expression.

### Syntax 

```
result = ~ expression
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
    All unary operators, such as the <span sdata="langKeyword" value="~"><span class="keyword">~</span></span> operator, evaluate expressions as follows:
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
    The <span sdata="langKeyword" value="~"><span class="keyword">~</span></span> operator looks at the binary representation of the values of the expression and does a bitwise negation operation on
    it.
  </p>
  <p xmlns:util="util">
    Any digit that is a 1 in the expression becomes a 0 in the result. Any digit that is a 0 in the expression becomes a 1 in the result.
  </p>
  <p xmlns:util="util">
    The following example illustrates use of the bitwise NOT (~) operator.
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
 var temp = ~5; 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    The resulting value is -6, as shown in the following table.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Expression
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Binary value (two's complement)
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Decimal value
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            00000000 00000000 00000000 00000101
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            5
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            ~5
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            11111111 11111111 11111111 11111010
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            -6
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
    <span sdata="link" xmlns:util="util"><a href="68c3dc71-ae95-4293-9155-67405846d71d.htm">Logical NOT Operator (!) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

