---
title: Boolean Object (JavaScript)
---

### Introduction 

 Creates a new Boolean value.

### Syntax 

```
boolObj = new Boolean([boolValue ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">boolObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <b>Boolean</b> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">boolValue</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The initial Boolean value for the new object. If <span class="parameter" sdata="paramReference">boolvalue</span> is omitted, or is <span sdata="langKeyword" value=
        "false"><span class="keyword">false</span></span>, 0, <span sdata="langKeyword" value="null"><span class="keyword">null</span></span>, <span sdata="langKeyword" value="NaN"><span class=
        "keyword">NaN</span></span>, or an empty string, the initial value of the Boolean object is <span sdata="langKeyword" value="false"><span class="keyword">false</span></span>. Otherwise, the
        initial value is <span sdata="langKeyword" value="true"><span class="keyword">true</span></span>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Boolean</b> object is a wrapper for the Boolean data type. JavaScript implicitly uses the <b>Boolean</b> object whenever a Boolean data type is converted to a <b>Boolean</b> object.
  </p>
  <p xmlns:util="util">
    You rarely instantiate the <b>Boolean</b> object explicitly.
  </p>
</div>

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the properties of the <b>Boolean</b> object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Property
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Description
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            constructor Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Specifies the function that creates a Boolean.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            prototype Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a reference to the prototype for a Boolean.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Methods 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the methods of the <b>Boolean</b> object.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Method
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Description
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string representation of a Boolean.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            valueOf Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Gets a reference to the Boolean.
          </p>
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

