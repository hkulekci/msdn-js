## [compile Method (Regular Expression) (JavaScript)](compile-Method__Regular-Expression.html)

### Introduction 

 Compiles a regular expression into an internal format for faster execution.

### Syntax 

```
rgExp .compile(pattern , [flags ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">rgExp</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An instance of a <b>Regular Expression</b> object. Can be a variable name or a literal.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">pattern</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A string expression containing a regular expression pattern to be compiled
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">flags</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Available flags, which may be combined, are:
      </p>
      <ul xmlns:util="util">
        <li>
          <p>
            g (global search for all occurrences of <i>pattern</i>)
          </p>
        </li>
        <li>
          <p>
            i (ignore case)
          </p>
        </li>
        <li>
          <p>
            m (multiline search)
          </p>
        </li>
      </ul>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>compile</b> method converts <i>pattern</i> into an internal format for faster execution. This allows for more efficient use of regular expressions in loops, for example. A compiled regular
    expression speeds things up when reusing the same expression repeatedly. No advantage is gained, however, if the regular expression changes.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>compile</b> method:
</p>

```
function CompileDemo(){ var rs; var s = "AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPp" // Create regular expression for uppercase only. var r = new RegExp("[A-Z]", "g"); var a1 = s.match(r) // Find matches. //
Compile the regular expression for lowercase only. r.compile( "[a-z]", "g") ; // Find matches. var a2 = s.match(r) return(a1 + "\n" + a2); }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="346aa83e-a045-47ea-acae-b42c7b121534.htm">Regular Expression Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
</div>

