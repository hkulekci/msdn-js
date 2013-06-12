---
title: JSON Object (JavaScript)
isChild: false
---

## JSON Object (JavaScript) {json_object_javascript_title}

### Introduction 

 An intrinsic object that provides functions to convert JavaScript values to and from the JavaScript Object Notation (JSON) format. The JSON.stringify function serializes a JavaScript value to JSON
text. The JSON.parse function deserializes JSON text to produce a JavaScript value.

### Syntax 

```
JSON.[method]
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">Method</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Name of one of the methods of the <span sdata="langKeyword" value="JSON"><span class="keyword">JSON</span></span> object.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    You cannot create a <span sdata="langKeyword" value="JSON"><span class="keyword">JSON</span></span> object by using the <span sdata="langKeyword" value="new"><span class=
    "keyword">new</span></span> operator. An error occurs if you try to do this. However, you can override or modify the <span sdata="langKeyword" value="JSON"><span class=
    "keyword">JSON</span></span> object.
  </p>
  <p xmlns:util="util">
    The scripting engine creates the <span sdata="langKeyword" value="JSON"><span class="keyword">JSON</span></span> object when the engine is loaded. Its methods are available to your script at all
    times.
  </p>
  <p xmlns:util="util">
    To use the intrinsic <span sdata="langKeyword" value="JSON"><span class="keyword">JSON</span></span> object, make sure that you do not override it with another <span sdata="langKeyword" value=
    "JSON"><span class="keyword">JSON</span></span> object that is defined in your script. You may need to modify existing script statements that detect the presence of a <span sdata="langKeyword"
    value="JSON"><span class="keyword">JSON</span></span> object because those statements will evaluate differently. This is demonstrated in the following example.
  </p>
  <div class="code">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th>
          JavaScript&nbsp;
        </th>
        <th>
          <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
          "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
        </th>
      </tr>
      <tr>
        <td colspan="2">
          <pre>
 if (!this.JSON) {     // JSON object does not exist.     } 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    In the previous example, <span class="code">!this.JSON</span> evaluates to false in Internet Explorer 8 standards mode, Internet Explorer 9 standards mode, Internet Explorer 10 standards mode,
    and win8_appname_long apps. Therefore, the code inside the <span sdata="langKeyword" value="if"><span class="keyword">if</span></span> statement does not execute.
  </p>
</div>

#### Functions 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    <span sdata="link"><a href="20f00d31-5ab5-4c3c-ab49-2534fc39a9b4.htm">JSON.parse Function (JavaScript)</a></span>
  </p>
  <p xmlns:util="util">
    <span sdata="link"><a href="0fafaf3b-c29b-46dc-b65b-ca223064a1d0.htm">JSON.stringify Function (JavaScript)</a></span>
  </p>
</div>

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
    <span sdata="link" xmlns:util="util"><a href="f91df030-e9c9-425e-8e6d-b46bdda66cb6.htm">toJSON Method (Date) (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="4a29a831-41c9-4843-9385-c3879e385585.htm">JavaScript Objects</a></span>
  </div>
</div>

