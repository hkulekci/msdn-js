---
title: JSON.stringify Function (JavaScript)
isChild: false
---

## JSON.stringify Function (JavaScript) {jsonstringify_function_javascript_title}

### Introduction 

 Converts a JavaScript value to a JavaScript Object Notation (JSON) string.

### Syntax 

```
JSON.stringify(value [ , replacer] [ , space] )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">value</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A JavaScript value, usually an object or array, to be converted.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">replacer</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A function or array that transforms the results.
      </p>
      <p xmlns:util="util">
        If <span class="parameter" sdata="paramReference">replacer</span> is a function, <span sdata="langKeyword" value="JSON.stringify"><span class="keyword">JSON.stringify</span></span> calls the
        function, passing in the key and value of each member. The return value is used instead of the original value. If the function returns <span sdata="langKeyword" value="undefined"><span class=
        "keyword">undefined</span></span>, the member is excluded. The key for the root object is an empty string: "".
      </p>
      <p xmlns:util="util">
        If <span class="parameter" sdata="paramReference">replacer</span> is an array, only members with key values in the array will be converted. The order in which the members are converted is the
        same as the order of the keys in the array. The <span class="parameter" sdata="paramReference">replacer</span> array is ignored when the <span class="parameter" sdata=
        "paramReference">value</span> argument is also an array.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">space</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Adds indentation, white space, and line break characters to the return-value JSON text to make it easier to read.
      </p>
      <p xmlns:util="util">
        If <span class="parameter" sdata="paramReference">space</span> is omitted, the return-value text is generated without any extra white space.
      </p>
      <p xmlns:util="util">
        If <span class="parameter" sdata="paramReference">space</span> is a number, the return-value text is indented with the specified number of white spaces at each level. If <span class=
        "parameter" sdata="paramReference">space</span> is greater than 10, text is indented 10 spaces.
      </p>
      <p xmlns:util="util">
        If <span class="parameter" sdata="paramReference">space</span> is a non-empty string, such as '\t', the return-value text is indented with the characters in the string at each level.
      </p>
      <p xmlns:util="util">
        If <span class="parameter" sdata="paramReference">space</span> is a string that is longer than 10 characters, the first 10 characters are used.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    A string that contains the JSON text.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Exception
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Condition
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link">Invalid replacer argument</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The <span class="parameter" sdata="paramReference">replacer</span> argument is not a function or an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span sdata="link">Circular reference in value argument not supported</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The <span class="parameter" sdata="paramReference">value</span> argument contains a circular reference.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">value</span> has a <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method, the <span sdata="langKeyword"
    value="JSON.stringify"><span class="keyword">JSON.stringify</span></span> function uses the return value of that method. If the return value of the <span sdata="langKeyword" value=
    "toJSON"><span class="keyword">toJSON</span></span> method is <span sdata="langKeyword" value="undefined"><span class="keyword">undefined</span></span>, the member is not converted. This enables
    an object to determine its own JSON representation.
  </p>
  <p xmlns:util="util">
    Values that do not have JSON representations, such as <span sdata="langKeyword" value="undefined"><span class="keyword">undefined</span></span>, will not be converted. In objects, they will be
    dropped. In arrays, they will be replaced with null.
  </p>
  <p xmlns:util="util">
    String values begin and end with a quotation mark. All Unicode characters may be enclosed in the quotation marks except for the characters that must be escaped by using a backslash. The following
    characters must be preceded by a backslash:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        Quotation mark (")
      </p>
    </li>
    <li>
      <p>
        Backslash (\)
      </p>
    </li>
    <li>
      <p>
        Backspace (b)
      </p>
    </li>
    <li>
      <p>
        Formfeed (f)
      </p>
    </li>
    <li>
      <p>
        Newline (n)
      </p>
    </li>
    <li>
      <p>
        Carriage return (r)
      </p>
    </li>
    <li>
      <p>
        Horizontal tab (t)
      </p>
    </li>
    <li>
      <p>
        Four-hexadecimal-digits (uhhhh)
      </p>
    </li>
  </ul>
  <h3 class="subHeading">
    Order of Execution
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      During the serialization process, if a <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method exists for the <span class="parameter" sdata=
      "paramReference">value</span> argument, <span sdata="langKeyword" value="JSON.stringify"><span class="keyword">JSON.stringify</span></span> first calls the <span sdata="langKeyword" value=
      "toJSON"><span class="keyword">toJSON</span></span> method. If it does not exist, the original value is used. Next, if a <span class="parameter" sdata="paramReference">replacer</span> argument
      is provided, the value (original value or <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> return-value) is replaced with the return-value of the <span class=
      "parameter" sdata="paramReference">replacer</span> argument. Finally, white spaces are added to the value based on the optional <span class="parameter" sdata="paramReference">space</span>
      argument to generate the final JSON text.
    </p>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  This example uses <span sdata="langKeyword" value="JSON.stringify"><span class="keyword">JSON.stringify</span></span> to convert the <span class="code">contact</span> object to JSON text. The
  <span class="code">memberfilter</span> array is defined so that only the <span class="code">surname</span> and <span class="code">phone</span> members are converted. The <span class=
  "code">firstname</span> member is omitted.
</p>

```
var contact = new Object(); contact.firstname = "Jesper"; contact.surname = "Aaberg"; contact.phone = ["555-0100", "555-0120"]; var memberfilter = new Array(); memberfilter[0] = "surname";
memberfilter[1] = "phone"; var jsonText = JSON.stringify(contact, memberfilter, "\t"); document.write(jsonText); // Output: // { "surname": "Aaberg", "phone": [ "555-0100", "555-0120" ] }
```

<p xmlns:util="util">
  This example uses <span sdata="langKeyword" value="JSON.stringify"><span class="keyword">JSON.stringify</span></span> with an array. The <span class="code">replaceToUpper</span> function converts
  every string in the array to uppercase.
</p>

```
var continents = new Array(); continents[0] = "Europe"; continents[1] = "Asia"; continents[2] = "Australia"; continents[3] = "Antarctica"; continents[4] = "North America"; continents[5] = "South
America"; continents[6] = "Africa"; var jsonText = JSON.stringify(continents, replaceToUpper); function replaceToUpper(key, value) { return value.toString().toUpperCase(); } //Output: //
"EUROPE,ASIA,AUSTRALIA,ANTARCTICA,NORTH AMERICA,SOUTH AMERICA,AFRICA"
```

<p xmlns:util="util">
  This example uses the <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method to convert string values to uppercase.
</p>

```
var contact = new Object(); contact.firstname = "Jesper"; contact.surname = "Aaberg"; contact.phone = ["555-0100", "555-0120"]; contact.toJSON = function(key) { var replacement = new Object(); for
(var val in this) { if (typeof (this[val]) === 'string') replacement[val] = this[val].toUpperCase(); else replacement[val] = this[val] } return replacement; }; var jsonText = JSON.stringify(contact);
document.write(jsonText); // Output: {"firstname":"JESPER","surname":"AABERG","phone":["555-0100","555-0120"]} '{"firstname":"JESPER","surname":"AABERG","phone":["555-0100","555-0120"]}' */
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10 standards. Also supported in Windows Store apps. See Version
    Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="20f00d31-5ab5-4c3c-ab49-2534fc39a9b4.htm">JSON.parse Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="f91df030-e9c9-425e-8e6d-b46bdda66cb6.htm">toJSON Method (Date) (JavaScript)</a></span>
  </div>
</div>

