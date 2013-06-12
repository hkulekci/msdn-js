---
title: name Property (Error) (JavaScript)
isChild: false
---

## name Property (Error) (JavaScript) {name_property_error_javascript_title}

### Introduction 

 Returns the name of an error.

### Syntax 

```
errorObj. name
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">errorObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Instance of <span sdata="langKeyword" value="Error"><span class="keyword">Error</span></span> object.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>name</b> property returns the name or exception type of an error. When a runtime error occurs, the name property is set to one of the following native exception types:
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Exception Type
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
            ConversionError
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            This error occurs whenever there is an attempt to convert an object into something to which it cannot be converted.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            RangeError
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            This error occurs when a function is supplied with an argument that has exceeded its allowable range. For example, this error occurs if you attempt to construct an <b>Array</b> object
            with a length that is not a valid positive integer.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            ReferenceError
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            This error occurs when an invalid reference has been detected. This error will occur, for example, if an expected reference is <span sdata="langKeyword" value="null"><span class=
            "keyword">null</span></span>.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            RegExpError
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            This error occurs when a compilation error occurs with a regular expression. Once the regular expression is compiled, however, this error cannot occur. This example will occur, for
            example, when a regular expression is declared with a pattern that has an invalid syntax, or flags other than <b>i</b>, <b>g</b>, or <b>m</b>, or if it contains the same flag more than
            once.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            SyntaxError
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            This error occurs when source text is parsed and that source text does not follow correct syntax. This error will occur, for example, if the <b>eval</b> function is called with an
            argument that is not valid program text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            TypeError
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            This error occurs whenever the actual type of an operand does not match the expected type. An example of when this error occurs is a function call made on something that is not an object
            or does not support the call.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            URIError
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            This error occurs when an illegal Uniform Resource Indicator (URI) is detected. For example, this is error occurs when an illegal character is found in a string being encoded or decoded.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example causes a TypeError exception to be thrown and displays the name of the error and its message.
</p>

```
try { var x = y; } catch(e) { document.write ("Error Message: " + e.message); document.write ("&lt;br /&gt;"); document.write ("Error Code: "); document.write (e.number &amp; 0xFFFF) document.write
("&lt;br /&gt;"); document.write ("Error Name: " + e.name); }
```

<p xmlns:util="util">
  The output of this code is as follows.
</p>

```
Error Message: 'y' is undefined Error Code: 5009 Error Name: TypeError
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="0b27d6ec-3997-4e91-a6c0-5afbaf494db7.htm">Error Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="ea727f1e-2041-4400-965c-67e6d47a1ff0.htm">description Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8cab0392-e0db-4714-827c-47ab04e8b4f2.htm">message Property (Error) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8697e20b-a2b0-4e26-85c0-ab07ddfe8281.htm">number Property (Error) (JavaScript)</a></span>
  </div>
</div>

