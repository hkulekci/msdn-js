## [for...in Statement (JavaScript)](for_in-Statement.html)

### Introduction 

 Executes one or more statements for each property of an object, or each element of an array.

### Syntax 

```
for (variable in [object | array ]) { 
	statements }
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">variable</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A variable that can be any property name of <span class="parameter" sdata="paramReference">object</span> or any element index of an <span class="parameter" sdata=
        "paramReference">array</span>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>, <span class="parameter" sdata="paramReference" xmlns:util="util">array</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. An object or array over which to iterate.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">statements</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. One or more statements to be executed for each property of <span class="parameter" sdata="paramReference">object</span> or each element of <span class="parameter" sdata=
        "paramReference">array</span>. Can be a compound statement.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    At the beginning of each iteration of a loop, the value of <span class="parameter" sdata="paramReference">variable</span> is the next property name of <span class="parameter" sdata=
    "paramReference">object</span> or the next element index of <span class="parameter" sdata="paramReference">array</span>. You can then use <span class="parameter" sdata=
    "paramReference">variable</span> in any of the statements inside the loop to reference the property of <span class="parameter" sdata="paramReference">object</span> or the element of <span class=
    "parameter" sdata="paramReference">array</span>.
  </p>
  <p xmlns:util="util">
    The properties of an object are not assigned in a determinate manner. You cannot specify a particular property by its index, only by the name of the property.
  </p>
  <p xmlns:util="util">
    Iterating through an array is performed in element order, that is, 0, 1, 2.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="for...in"><span class="keyword">for...in</span></span> statement with an object used as an associative array.
</p>

```
// Initialize object. a = {"a" : "Athens" , "b" : "Belgrade", "c" : "Cairo"} // Iterate over the properties. var s = "" for (var key in a) { s += key + ": " + a[key]; s += "&lt;br /&gt;"; }
document.write (s); // Output: // a: Athens // b: Belgrade // c: Cairo
```

<p xmlns:util="util">
  This example illustrates the use of the <span sdata="langKeyword" value="for ... in"><span class="keyword">for ... in</span></span> statement to iterate though an <b>Array</b> object that has
  expando properties.
</p>

```
// Initialize the array. var arr = new Array("zero","one","two"); // Add a few expando properties to the array. arr["orange"] = "fruit"; arr["carrot"] = "vegetable"; // Iterate over the properties
and elements. var s = ""; for (var key in arr) { s += key + ": " + arr[key]; s += "&lt;br /&gt;"; } document.write (s); // Output: // 0: zero // 1: one // 2: two // orange: fruit // carrot: vegetable
```

<p xmlns:util="util">
  Use the <b>Enumerator</b> object to iterate over the members of a collection.
</p>

```
<p xmlns:util="util">
  Use the <b>Enumerator</b> object to iterate over the members of a collection.
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
    <span sdata="link" xmlns:util="util"><a href="bae0ec40-152e-43f3-969b-3696489ec5c4.htm">for Statement (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="d63777cf-0e1a-4555-8d3a-334381001f48.htm">while Statement (JavaScript)</a></span>
  </div>
</div>

