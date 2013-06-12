---
title: GetObject Function (JavaScript)
isChild: false
---

## GetObject Function (JavaScript) {getobject_function_javascript_title}

### Introduction 

 Returns a reference to an Automation object from a file. Note This function is not supported in Internet Explorer 9 (standards mode) or later.

### Syntax 

```
GetObject([pathname ] [, class ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">pathname</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Full path and name of the file containing the object to retrieve. If <span class="parameter" sdata="paramReference">pathname</span> is omitted, <span class="parameter" sdata=
        "paramReference">class</span> is required.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">class</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Class of the object.
      </p>
    </dd>
  </dl>
  <p xmlns:util="util">
    The <span class="parameter" sdata="paramReference">class</span> argument uses the syntax <span class="parameter" sdata="paramReference">appname.objectype</span> and has these parts:
  </p>
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">appname</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Name of the application providing the object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">objectype</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Type or class of object to create.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>GetObject</b> function is not supported in Internet Explorer 9 standards mode, Internet Explorer 10 standards mode, and win8_appname_long apps or later.
  </p>
  <p xmlns:util="util">
    Use the <b>GetObject</b> function to access an Automation object from a file. Assign the object returned by <b>GetObject</b> to the object variable. For example:
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
 var CADObject; CADObject = GetObject("C:\\CAD\\SCHEMA.CAD"); 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    When this code is executed, the application associated with the specified <span class="parameter" sdata="paramReference">pathname</span> is started, and the object in the specified file is
    activated. If <span class="parameter" sdata="paramReference">pathname</span> is a zero-length string (""), <b>GetObject</b> returns a new object instance of the specified type. If the
    <span class="parameter" sdata="paramReference">pathname</span> argument is omitted, <b>GetObject</b> returns a currently active object of the specified type. If no object of the specified type
    exists, an error occurs.
  </p>
  <p xmlns:util="util">
    Some applications allow you to activate part of a file. To do so, add an exclamation point (!) to the end of the file name and follow it with a string that identifies the part of the file you
    want to activate. For information on how to create this string, see the documentation for the application that created the object.
  </p>
  <p xmlns:util="util">
    For example, in a drawing application you might have multiple layers to a drawing stored in a file. You could use the following code to activate a layer within a drawing called <span class=
    "code">SCHEMA.CAD</span>:
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
 var LayerObject = GetObject("C:\\CAD\\SCHEMA.CAD!Layer3"); 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    If you do not specify the object's class, Automation determines which application to start and which object to activate, based on the file name you provide. Some files, however, may support more
    than one class of object. For example, a drawing might support three different types of objects: an Application object, a Drawing object, and a Toolbar object, all of which are part of the same
    file. To specify which object in a file you want to activate, use the optional <span class="parameter" sdata="paramReference">class</span> argument. For example:
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
 var MyObject; MyObject = <span class="label">GetObject(</span>"C:\\DRAWINGS\\SAMPLE.DRW", "FIGMENT.DRAWING"<span class="label">)</span>; 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    In the preceding example, <span class="code">FIGMENT</span> is the name of a drawing application and <span class="code">DRAWING</span> is one of the object types it supports. Once an object is
    activated, you reference it in code using the object variable you defined. In the preceding example, you access properties and methods of the new object using the object variable <span class=
    "code">MyObject</span>. For example:
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
 MyObject.Line(9, 90); MyObject.InsertText(9, 100, "Hello, world."); MyObject.SaveAs("C:\\DRAWINGS\\SAMPLE.DRW"); 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <div class="alert">
    <table width="100%" cellspacing="0" cellpadding="0">
      <tr>
        <th align="left">
          <img class="note" alt="Note" title="Note" src="../icons/alert_note.gif" /><b>Note</b>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Use the <b>GetObject</b> function when there is a current instance of the object, or if you want to create the object with a file already loaded. If there is no current instance, and you
            don't want the object started with a file loaded, use the <b>ActiveXObject</b> object.
          </p>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    If an object has registered itself as a single-instance object, only one instance of the object is created, no matter how many times <b>ActiveXObject</b> is executed. With a single-instance
    object, <b>GetObject</b> always returns the same instance when called with the zero-length string ("") syntax, and it causes an error if the <span class="parameter" sdata=
    "paramReference">pathname</span> argument is omitted.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, and Internet Explorer 8 standards. See <span sdata="link">Version
    Information</span>.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="9c7bed07-853f-48aa-92db-3131324746ec.htm">ActiveXObject Object (JavaScript)</a></span>
  </div>
</div>

