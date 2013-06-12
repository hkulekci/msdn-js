---
title: new Operator (JavaScript)
---

### Introduction 

 Creates a new object.

### Syntax 

```
new constructor ([arguments ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">constructor</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The constructor of the object. The parentheses can be omitted if the constructor takes no arguments.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">arguments</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Any arguments to be passed to the new object's constructor.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="new"><span class="keyword">new</span></span> operator performs the following tasks:
  </p>
  <ul xmlns:util="util">
    <li>
      <p>
        It creates an object with no members.
      </p>
    </li>
    <li>
      <p>
        It calls the constructor for that object, passing a pointer to the newly created object as the <span sdata="langKeyword" value="this"><span class="keyword">this</span></span> pointer.
      </p>
    </li>
    <li>
      <p>
        The constructor then initializes the object according to the arguments passed to the constructor.
      </p>
    </li>
  </ul>
  <p xmlns:util="util">
    These are examples of valid uses of the <b>new</b> operator.
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
 my_object = new Object; my_array = new Array(); my_date = new Date("Jan 5 1996"); 
</pre>
        </td>
      </tr>
    </table>
  </div>
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
    <span sdata="link" xmlns:util="util"><a href="cc9cfd43-1305-41c8-ad67-545d20f4fafe.htm">function Statement (JavaScript)</a></span>
  </div>
</div>

