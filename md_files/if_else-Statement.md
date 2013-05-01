## [if...else Statement (JavaScript)](if_else-Statement.html)

### Introduction 

 Conditionally executes a group of statements, depending on the value of an expression.

### Syntax 

```
if (condition1 ) { 
	statement1 } 
[else if (condition2 ) { 
	statement2 }] [else { 
	statement3 ] }]
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">condition1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A Boolean expression. If <span class="parameter" sdata="paramReference">condition1</span> is <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> or
        <span sdata="langKeyword" value="undefined"><span class="keyword">undefined</span></span>, <span class="parameter" sdata="paramReference">condition1</span> is treated as <span sdata=
        "langKeyword" value="false"><span class="keyword">false</span></span>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statement1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The statement to be executed if <span class="parameter" sdata="paramReference">condition1</span> is <b>true</b>. Can be a compound statement.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">condition2</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        The condition to be evaluated.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statement2</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The statement to be executed if <span class="parameter" sdata="paramReference">condition2</span> is <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>.
        Can be a compound statement.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statement3</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        If both <span class="parameter" sdata="paramReference">condition1</span> and <span class="parameter" sdata="paramReference">condition2</span> are <span sdata="langKeyword" value=
        "false"><span class="keyword">false</span></span>, this statement is executed.
      </p>
    </dd>
  </dl>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use <span sdata="langKeyword" value="if"><span class="keyword">if</span></span>, <span sdata="langKeyword" value="if else"><span class="keyword">if
  else</span></span>, and <span sdata="langKeyword" value="else"><span class="keyword">else</span></span>.
</p>

```
var z = 3; if (x == 5) { z = 10; } else if (x == 10) { z = 15; } else { z = 20; }
```

<p xmlns:util="util">
  It is good practice to enclose <span class="parameter" sdata="paramReference">statement1</span> and <span class="parameter" sdata="paramReference">statement2</span> in braces ({}) for clarity and
  to avoid inadvertent errors.
</p>

```
<p xmlns:util="util">
  It is good practice to enclose <span class="parameter" sdata="paramReference">statement1</span> and <span class="parameter" sdata="paramReference">statement2</span> in braces ({}) for clarity and
  to avoid inadvertent errors.
</p>
```

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
    <span sdata="link" xmlns:util="util"><a href="7399ac32-9324-4a9a-ae76-be9c0f9df81c.htm">Conditional (Ternary) Operator (?:) (JavaScript)</a></span>
  </div>
</div>

