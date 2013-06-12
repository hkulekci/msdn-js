---
title: Logical AND Operator (&amp;&amp;) (JavaScript)
isChild: false
---

## Logical AND Operator (&amp;&amp;) (JavaScript) {logical_and_operator_ampamp_javascript_title}

### Introduction 

 Performs a logical conjunction on two expressions.

### Syntax 

```
result = expression1 &amp;&amp; 
expression2
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
      <span class="parameter" sdata="paramReference" xmlns:util="util">expression1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Any expression.
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
    If both expressions evaluate to <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>, <span class="parameter" sdata="paramReference">result</span> is <span sdata=
    "langKeyword" value="true"><span class="keyword">true</span></span>. If either expression evaluates to <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>,
    <span class="parameter" sdata="paramReference">result</span> is <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>.
  </p>
  <p xmlns:util="util">
    JavaScript uses the following rules for converting non-Boolean values to Boolean values:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        All objects are considered to be <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>.
      </p>
    </li>
    <li>
      <p>
        Strings are considered to be <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> if they are empty.
      </p>
    </li>
    <li>
      <p>
        <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> and <span sdata="langKeyword" value="undefined"><span class="keyword">undefined</span></span> are considered to
        be <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>.
      </p>
    </li>
    <li>
      <p>
        A Number is <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> if it is zero.
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

