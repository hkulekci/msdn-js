---
title: replace Method (String) (JavaScript)
isChild: false
---

## replace Method (String) (JavaScript) {replace_method_string_javascript_title}

### Introduction 

 Replaces text in a string, using a regular expression or search string.

### Syntax 

```
stringObj . replace(rgExp , replaceText )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal on which to perform the replacement. This string is not modified by
        the <b>replace</b> method. Rather, the return value of this method is the string produced by the replacement.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">rgExp</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An instance of a <b>Regular Expression</b> object containing the regular expression pattern and applicable flags. Can also be a <span sdata="langKeyword" value="String"><span class=
        "keyword">String</span></span> object or string literal that represents the regular expression. If <span class="parameter" sdata="paramReference">rgExp</span> is not an instance of a
        <b>Regular Expression</b> object, it is converted to a string, and an exact search is made for the results; no attempt is made to convert the string into a regular expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">replaceText</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal containing the text to replace for every successful match of
        <span class="parameter" sdata="paramReference">rgExp</span> in <span class="parameter" sdata="paramReference">stringObj</span>. In Internet Explorer 5.5 or later, the <span class="parameter"
        sdata="paramReference">replaceText</span> argument can also be a function that returns the replacement text.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The result of the <b>replace</b> method is a copy of <span class="parameter" sdata="paramReference">stringObj</span> after the specified replacements have been made.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Any of the following match variables can be used to identify the most recent match and the string from which it came. The match variables can be used in text replacement where the replacement
    string has to be determined dynamically.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Characters
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Meaning
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <b>$$</b>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <span sdata="langKeyword" value="$"><span class="keyword">$</span></span> (Internet Explorer 5.5 or later)
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <b>$&amp;</b>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Specifies that portion of <span class="parameter" sdata="paramReference">stringObj</span> that the entire pattern matched. (Internet Explorer 5.5 or later)
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <b>$`</b>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Specifies that portion of <span class="parameter" sdata="paramReference">stringObj</span> that precedes the match described by <b>$&amp;</b>. (Internet Explorer 5.5 or later)
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <b>$'</b>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Specifies that portion of <span class="parameter" sdata="paramReference">stringObj</span> that follows the match described by <b>$&amp;</b>. (Internet Explorer 5.5 or later)
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="langKeyword" value="$"><span class="keyword">$</span></span><b><i>n</i></b>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The <i>n</i>th captured submatch, where <i>n</i> is a single decimal digit from 1 through 9. (Internet Explorer 5.5 or later)
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="langKeyword" value="$"><span class="keyword">$</span></span><b><i>nn</i></b>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The <i>nn</i>th captured submatch, where <i>nn</i> is a two-digit decimal number from 01 through 99. (Internet Explorer 5.5 or later)
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">replaceText</span> is a function, for each matched substring the function is called with the following <i>m</i> + 3 arguments where <i>m</i> is
    the number of left capturing parentheses in the <span class="parameter" sdata="paramReference">rgExp</span>. The first argument is the substring that matched. The next <i>m</i> arguments are all
    of the captures that resulted from the search. Argument <i>m</i> + 2 is the offset within <span class="parameter" sdata="paramReference">stringObj</span> where the match occurred, and argument
    <i>m</i> + 3 is <span class="parameter" sdata="paramReference">stringObj</span>. The result is the string value that results from replacing each matched substring with the corresponding return
    value of the function call.
  </p>
  <p xmlns:util="util">
    The <b>replace</b> method updates the properties of the global <b>RegExp</b> object.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>replace</b> method to replace all instances of "the" with "a."
</p>

```
var s = "the batter hit the ball with the bat"; // Replace "the" with "a". var re = /the/g; var result = s.replace(re, "a"); document.write(result); // Output: a batter hit a ball with a bat
```

<p xmlns:util="util">
  In addition, the <b>replace</b> method can also replace subexpressions in the pattern. The following example exchanges each pair of words in the string.
</p>

```
var s = "The quick brown fox jumped over the lazy dog."; var re = /(\S+)(\s+)(\S+)/g; // Exchange each pair of words. var result = s.replace(re, "$3$2$1"); document.write(result); // Output: quick
The fox brown over jumps lazy the dog.
```

<p xmlns:util="util">
  The following example, which works in JavaScript 5.5 and later, shows how to use a function that returns the replacement text. It replaces any instance of a number followed by "F" with a Celsius
  conversion.
</p>

```
function f2c(s1) { // Initialize pattern. var test = /(\d+(\.\d*)?)F\b/g; // Use a function for the replacement. var s2 = s1.replace(test, function($0,$1,$2) { return((($1-32) * 5/9) + "C"); } )
return s2; } document.write(f2c("Water freezes at 32F and boils at 212F.")); // Output: Water freezes at 0C and boils at 100C.
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="83092452-60cc-4218-b4ae-af9e3cb96c34.htm">exec Method (Regular Expression) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="eda9ad27-4f9b-4cb1-8345-a0ae85979ca0.htm">match Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="7f6b1073-8cbb-49ed-94b6-56833ba663c5.htm">RegExp Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="1cae0fbc-3319-4327-ba4e-d5fa2c4a9ba0.htm">search Method (String) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4f4b6e39-cb1a-4be9-a66f-7b846075580d.htm">test Method (Regular Expression) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Regular Expression Programming (Scripting)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Alternation and Subexpressions (Scripting)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Backreferences (Scripting)</span>
  </div>
</div>

