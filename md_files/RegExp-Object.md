## [RegExp Object (JavaScript)](RegExp-Object.html)

### Introduction 

 An intrinsic global object that stores information about the results of regular expression pattern matches.

### Syntax 

```
RegExp.property
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <i>property</i> argument can be any one of the <b>RegExp</b> object properties.
  </p>
  <p xmlns:util="util">
    The <b>RegExp</b> object cannot be created directly, but is always available for use. Until a successful regular expression search has been completed, the initial values of the various properties
    of the <b>RegExp</b> object are as follows:
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Property
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Shorthand
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Initial Value
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            index
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            &nbsp;
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            -1
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            input
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            $_
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Empty string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            lastIndex
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            &nbsp;
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            -1
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            lastMatch
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            $&amp;
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Empty string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            lastParen
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            $+
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Empty string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            leftContext
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            $`
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Empty string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            rightContext
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            $'
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Empty string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            $1 - $9
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            $1 - $9
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Empty string.
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    Its properties have undefined as their value until a successful regular expression search has been completed.
  </p>
  <p xmlns:util="util">
    The global <b>RegExp</b> object should not be confused with the <b>Regular Expression</b> object. Even though they sound like the same thing, they are separate and distinct. The properties of the
    global <b>RegExp</b> object contain continually updated information about each match as it occurs, while the properties of the <b>Regular Expression</b> object contain only information about the
    matches that occur with that instance of the <b>Regular Expression</b>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example performs a regular expression search. It displays matches and submatches from the global <b>RegExp</b> object, and from the array that is returned by the <b>exec</b> method.
</p>

```
var newLine = "&lt;br /&gt;"; var re = /(\w+)@(\w+)\.(\w+)/g var src = "Please send mail to george@contoso.com and someone@example.com. Thanks!" var result; var s = ""; // Get the first match. result
= re.exec(src); while (result != null) { // Show the entire match. s += newLine; // Show the match and submatches from the RegExp global object. s += "RegExp.lastMatch: " + RegExp.lastMatch +
newLine; s += "RegExp.$1: " + RegExp.$1 + newLine; s += "RegExp.$2: " + RegExp.$2 + newLine; s += "RegExp.$3: " + RegExp.$3 + newLine; // Show the match and submatches from the array that is returned
// by the exec method. for (var index = 0; index &lt; result.length; index++) { s += index + ": "; s += result[index]; s += newLine; } // Get the next match. result = re.exec(src); }
document.write(s); // Output: // RegExp.lastMatch: george@contoso.com // RegExp.$1: george // RegExp.$2: contoso // RegExp.$3: com // 0: george@contoso.com // 1: george // 2: contoso // 3: com //
RegExp.lastMatch: someone@example.com // RegExp.$1: someone // RegExp.$2: example // RegExp.$3: com // 0: someone@example.com // 1: someone // 2: example // 3: com
```

#### Properties 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    $1...$9 Properties | index Property | input Property | lastIndex Property | lastMatch Property | lastParen Property | leftContext Property | rightContext Property
  </p>
</div>

#### Methods 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The <b>RegExp</b> object has no methods.
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
    <span sdata="link" xmlns:util="util"><a href="346aa83e-a045-47ea-acae-b42c7b121534.htm">Regular Expression Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Syntax</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

