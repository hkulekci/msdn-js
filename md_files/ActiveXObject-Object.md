---
title: ActiveXObject Object (JavaScript)
isChild: false
---

## ActiveXObject Object (JavaScript) {activexobject_object_javascript_title}

### Introduction 

 Enables and returns a reference to an Automation object. This object is used only to instantiate Automation objects, and has no members. Caution This object is supported in Internet Explorer only,
not in Windows Store apps.

### Syntax 

```
newObj = new ActiveXObject(servername.typename [, location ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">newObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <b>ActiveXObject</b> is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">servername</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The name of the application providing the object.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">typename</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The type or class of the object to create.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">location</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The name of the network server where the object is to be created.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Automation servers provide at least one type of object. For example, a word-processing application may provide an application object, a document object, and a toolbar object.
  </p>
  <p xmlns:util="util">
    To create an Automation object, assign the new <b>ActiveXObject</b> to an object variable:
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
 var ExcelApp = new ActiveXObject("Excel.Application"); var ExcelSheet = new ActiveXObject("Excel.Sheet"); 
</pre>
        </td>
      </tr>
    </table>
  </div>
  <p xmlns:util="util">
    This code starts the application creating the object (in this case, a Microsoft Excel worksheet). Once an object is created, you refer to it in code using the object variable you defined. In the
    following example, you access properties and methods of the new object using the object variable <span class="code">ExcelSheet</span> and other Excel objects, including the Application object and
    the ActiveSheet.Cells collection.
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
 // Make Excel visible through the Application object. ExcelSheet.Application.Visible = true; // Place some text in the first cell of the sheet. ExcelSheet.ActiveSheet.Cells(1,1).Value = "This is column A, row 1"; // Save the sheet. ExcelSheet.SaveAs("C:\\TEST.XLS"); // Close Excel with the Quit method on the Application object. ExcelSheet.Application.Quit(); 
</pre>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Not supported in Windows Store apps. See <span sdata="link">Version Information</span>.
  </p>
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
            Creating an <b>ActiveXObject</b> on a remote server is not supported in Internet Explorer 9 standards mode, Internet Explorer 10 standards mode, and win8_appname_long apps or later.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="62efcdbc-8b86-491d-9000-ef38aa9942a9.htm">GetObject Function (JavaScript)</a></span>
  </div>
</div>

