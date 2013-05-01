## [Regular Expression Object (JavaScript)](Regular-Expression-Object.html)

### Introduction 

 An object that contains a regular expression pattern along with flags that identify how to apply the pattern.

### Syntax 

```
re = /pattern /[flags ]
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <i xmlns:util="util">re</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the regular expression pattern is assigned.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">pattern</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The regular expression pattern to use. If you use Syntax 1, delimit the pattern by "/" characters. If you use Syntax 2, enclose the pattern in quotation marks.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">flags</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Enclose flag in quotation marks if you use Syntax 2. Available flags, which may be combined, are:
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
    The <b>Regular Expression</b> object should not be confused with the global <b>RegExp</b> object. Even though they sound the same, they are separate and distinct. The properties of the <b>Regular
    Expression</b> object contain only information about one particular <b>Regular Expression</b> instance, while the properties of the global <b>RegExp</b> object contain continually updated
    information about each match as it occurs.
  </p>
  <p xmlns:util="util">
    <b>Regular Expression</b> objects store patterns used when searching strings for character combinations. After the <b>Regular Expression</b> object is created, it is either passed to a string
    method, or a string is passed to one of the regular expression methods. Information about the most recent search performed is stored in the global <b>RegExp</b> object.
  </p>
  <p xmlns:util="util">
    Use Syntax 1 when you know the search string ahead of time. Use Syntax 2 when the search string is changing frequently, or is unknown, such as strings taken from user input.
  </p>
  <p xmlns:util="util">
    The <i>pattern</i> argument is compiled into an internal format before use. For Syntax 1, <i>pattern</i> is compiled as the script is loaded. For Syntax 2, <i>pattern</i> is compiled just before
    use, or when the <b>compile</b> method is called.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>Regular Expression</b> object by creating an object (re) containing a regular expression pattern with its associated flags. In this case, the
  resulting <b>Regular Expression</b> object is then used by the <b>match</b> method:
</p>

```
function MatchDemo(){ var s = "through the pages of the book"; // Create regular expression pattern. var re = new RegExp("the", "i"); // Attempt match on search string. var r = s.match(re); // Return
first occurrence of "the". return(r); }
```

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    global Property | ignoreCase Property | multiline Property | source Property
  </p>
</div>

#### Methods 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    compile Method | exec Method | test Method
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
    <span sdata="link" xmlns:util="util"><a href="7f6b1073-8cbb-49ed-94b6-56833ba663c5.htm">RegExp Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

