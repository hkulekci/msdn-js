---
title: JSON.parse Function (JavaScript)
---

### Introduction 

 Converts a JavaScript Object Notation (JSON) string into an object.

### Syntax 

```
JSON.parse(text [ , reviver] )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">text</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A valid JSON string.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">reviver</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. A function that transforms the results. This function is called for each member of the object. If a member contains nested objects, the nested objects are transformed before the
        parent object is. For each member, the following occurs:
      </p>
      <ul xmlns:util="util">
        <li>
          <p>
            If <span class="parameter" sdata="paramReference">reviver</span> returns a valid value, the member value is replaced with the transformed value.
          </p>
        </li>
        <li>
          <p>
            If <span class="parameter" sdata="paramReference">reviver</span> returns the same value it received, the member value is not modified.
          </p>
        </li>
        <li>
          <p>
            If <span class="parameter" sdata="paramReference">reviver</span> returns <span sdata="langKeyword" value="null"><span class="keyword">null</span></span> or <span sdata="langKeyword"
            value="undefined"><span class="keyword">undefined</span></span>, the member is deleted.
          </p>
        </li>
      </ul>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="returnValueSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    An object or array.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If this function provokes a JavaScript parser error (such as "SCRIPT1014: Invalid character", the input text does not comply with JSON syntax. To correct the error, do one of the following:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        Modify the <span class="parameter" sdata="paramReference">text</span> argument to comply with JSON syntax. For more information, see the <a href=
        "http://go.microsoft.com/fwlink/?LinkId=125203">BNF syntax notation</a> of JSON objects.
      </p>
    </li>
    <li>
      <p>
        Make sure that the text argument was serialized by a JSON-compliant implementation, such as <b>JSON.stringify</b>.
      </p>
    </li>
  </ul>
</div>

#### Example 

<p xmlns:util="util">
  The following example uses <b>JSON.parse</b> to convert a JSON string to an object.
</p>

```
var jsontext = '{"firstname":"Jesper","surname":"Aaberg","phone":["555-0100","555-0120"]}'; var contact = JSON.parse(jsontext); document.write(contact.surname + ", " + contact.firstname); // Output:
Aaberg, Jesper
```

<p xmlns:util="util">
  The following example shows how to convert an array to a JSON string by using <b>JSON.stringify</b>, and then convert the string back to an array by using <b>JSON.parse</b>.
</p>

```
var arr = ["a", "b", "c"]; var str = JSON.stringify(arr); document.write(str); document.write ("&lt;br/&gt;"); var newArr = JSON.parse(str); while (newArr.length &gt; 0) { document.write(newArr.pop()
+ "&lt;br/&gt;"); } // Output: var arr = ["a", "b", "c"]; var str = JSON.stringify(arr); document.write(str); document.write ("&lt;br/&gt;"); var newArr = JSON.parse(str); while (newArr.length &gt;
0) { document.write(newArr.pop + "&lt;br/&gt;"); } // Output: ["a","b","c"] c b a
```

<p xmlns:util="util">
  The <span class="parameter" sdata="paramReference">reviver</span> function is often used to transform JSON representation of International Organization for Standardization (ISO) date strings into
  Coordinated Universal Time (UTC) format <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> objects.
</p>

```
var jsontext = '{ "hiredate": "2008-01-01T12:00:00Z", "birthdate": "2008-12-25T12:00:00Z" }'; var dates = JSON.parse(jsontext, dateReviver); document.write(dates.birthdate.toUTCString()); function
dateReviver(key, value) { var a; if (typeof value === 'string') { a = /^(\d{4})-(\d{2})-(\d{2})T(\d{2}):(\d{2}):(\d{2}(?:\.\d*)?)Z$/.exec(value); if (a) { return new Date(Date.UTC(+a[1], +a[2] - 1,
+a[3], +a[4], +a[5], +a[6])); } } return value; }; // Output: // Thu, 25 Dec 2008 12:00:00 UTC
```

<p xmlns:util="util">
  This example uses <span sdata="langKeyword" value="JSON.parse"><span class="keyword">JSON.parse</span></span> to deserialize an ISO-formatted date string. The <span class="code">dateReviver</span>
  function returns <span class="code">Date</span> objects for members that are formatted like ISO date strings.
</p>

```
<p xmlns:util="util">
  This example uses <span sdata="langKeyword" value="JSON.parse"><span class="keyword">JSON.parse</span></span> to deserialize an ISO-formatted date string. The <span class="code">dateReviver</span>
  function returns <span class="code">Date</span> objects for members that are formatted like ISO date strings.
</p>
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
    <span sdata="link" xmlns:util="util"><a href="0fafaf3b-c29b-46dc-b65b-ca223064a1d0.htm">JSON.stringify Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="f91df030-e9c9-425e-8e6d-b46bdda66cb6.htm">toJSON Method (Date) (JavaScript)</a></span>
  </div>
</div>

