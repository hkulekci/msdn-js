---
title: toJSON Method (Date) (JavaScript)
isChild: false
---

## toJSON Method (Date) (JavaScript) {tojson_method_date_javascript_title}

### Introduction 

 Used by the JSON.stringify method to enable the transformation of an object's data for JavaScript Object Notation (JSON) serialization.

### Syntax 

```
objectname .toJSON()
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">objectname</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An object for which JSON serialization is wanted.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method is used by the <span sdata="langKeyword" value="JSON.stringify"><span class=
    "keyword">JSON.stringify</span></span> function. <span sdata="langKeyword" value="JSON.stringify"><span class="keyword">JSON.stringify</span></span> serializes a JavaScript value into JSON text.
    If a <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method is provided to <span sdata="langKeyword" value="JSON.stringify"><span class=
    "keyword">JSON.stringify</span></span>, the <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method is called when <span sdata="langKeyword" value=
    "JSON.stringify"><span class="keyword">JSON.stringify</span></span> is called.
  </p>
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method is a built-in member of the Date JavaScript object. It returns an ISO-formatted date string for the
    UTC time zone (denoted by the suffix Z).
  </p>
  <p xmlns:util="util">
    You can override the <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method for the <span sdata="langKeyword" value="Date"><span class=
    "keyword">Date</span></span> type, or define a <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method for other object types to achieve transformation of data
    for the specific object type before JSON serialization.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example uses the <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method to serialize string member values in uppercase. The <span sdata=
  "langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method is called when <span sdata="langKeyword" value="JSON.stringify"><span class="keyword">JSON.stringify</span></span> is
  called.
</p>

```
var contact = new Object(); contact.firstname = "Jesper"; contact.surname = "Aaberg"; contact.phone = ["555-0100", "555-0120"]; contact.toJSON = function(key) { var replacement = new Object(); for
(var val in this) { if (typeof (this[val]) === 'string') replacement[val] = this[val].toUpperCase(); else replacement[val] = this[val] } return replacement; }; var jsonText = JSON.stringify(contact);
/* The value of jsonText is: '{"firstname":"JESPER","surname":"AABERG","phone":["555-0100","555-0120"]}' */
```

<p xmlns:util="util">
  The following example illustrates how to use the <span sdata="langKeyword" value="toJSON"><span class="keyword">toJSON</span></span> method that is a built-in member of the Date object.
</p>

```
var dt = new Date('8/24/2009'); dt.setUTCHours(7, 30, 0); var jsonText = JSON.stringify(dt); /* The value of jsonText is: '"2009-08-24T07:30:00Z"' */
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
  </p><b>Applies To:</b> Date Object
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="0279a0e0-70bf-451a-a78e-0da4e2fdeb9a.htm">JSON Object (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="20f00d31-5ab5-4c3c-ab49-2534fc39a9b4.htm">JSON.parse Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="0fafaf3b-c29b-46dc-b65b-ca223064a1d0.htm">JSON.stringify Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="003747e2-7860-4c96-b129-5180ae0fe745.htm">JavaScript Methods</a></span>
  </div>
</div>

