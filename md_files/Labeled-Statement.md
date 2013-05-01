## [Labeled Statement (JavaScript)](Labeled-Statement.html)

### Introduction 

 Provides an identifier for a statement.

### Syntax 

```
label : statements
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">label</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A unique identifier used when referring to the labeled statement.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statements</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. One or more statements associated with <i>label</i>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Labels are used by the <b>break</b> and <b>continue</b> statements to specify the statement to which the <b>break</b> and <b>continue</b> apply.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  In the following code, the <b>continue</b> statement refers to the <b>for</b> loop that is preceded by the <span class="code">Inner:</span> statement. When <span class="code">j</span> is 24, the
  <b>continue</b> statement causes that <b>for</b> loop to go to the next iteration. The numbers 21 through 23 and 25 through 30 print on each line.
</p>

```
Outer: for (i = 1; i &lt;= 10; i++) { document.write ("&lt;br /&gt;"); document.write ("i: " + i); document.write (" j: "); Inner: for (j = 21; j &lt;= 30; j++) { if (j == 24) { continue Inner; }
document.write (j + " "); } }
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
    <span sdata="link" xmlns:util="util"><a href="5be0f2a8-5fe7-4a6c-89af-ca20a925ce87.htm">break Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="f8a30d9f-e2de-4e1f-8668-4e4cf95f7df9.htm">continue Statement (JavaScript)</a></span>
  </div>
</div>

