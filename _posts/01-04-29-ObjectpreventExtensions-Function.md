---
title: Object.preventExtensions Function (JavaScript)
---

### Introduction 

 Prevents the addition of new properties to an object.

### Syntax 

```
Object.preventExtensions(object )
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The object to make non-extensible.
      </p>
    </dd>
  </dl>
</div>

#### Return Value 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The object that is passed to the function.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the <span class="parameter" sdata="paramReference">object</span> argument is not an object, a <span sdata="langKeyword" value="TypeError"><span class="keyword">TypeError</span></span>
    exception is thrown.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Object.preventExtensions</b> function makes an object non-extensible, so that new named properties cannot be added to it. After an object is made non-extensible, it cannot be made
    extensible.
  </p>
  <p xmlns:util="util">
    For information about how to set property attributes, see <span sdata="link"><a href="c5d05346-940a-40c2-b12a-e8b25abc8d46.htm">Object.defineProperty Function (JavaScript)</a></span>.
  </p>
  <p xmlns:util="util"></p>
  <h3 class="subHeading">
    Related Functions
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      The following related functions prevent the modification of object attributes.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Function
            </p>
          </th>
          <th>
            <p xmlns:util="util">
              Object is made non-extensible
            </p>
          </th>
          <th>
            <p xmlns:util="util">
              <span sdata="langKeyword" value="configurable"><span class="keyword">configurable</span></span> is set to <span sdata="langKeyword" value="false"><span class=
              "keyword">false</span></span> for each property
            </p>
          </th>
          <th>
            <p xmlns:util="util">
              <span sdata="langKeyword" value="writable"><span class="keyword">writable</span></span> is set to <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> for
              each property
            </p>
          </th>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              <b>Object.preventExtensions</b>
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Object.seal
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Object.freeze
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
        </tr>
      </table>
    </div>
    <p xmlns:util="util">
      The following functions return <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if all of the conditions marked in the following table are true.
    </p>
    <div class="caption"></div>
    <div class="tableSection">
      <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
        <tr>
          <th>
            <p xmlns:util="util">
              Function
            </p>
          </th>
          <th>
            <p xmlns:util="util">
              Object is extensible?
            </p>
          </th>
          <th>
            <p xmlns:util="util">
              <span sdata="langKeyword" value="configurable"><span class="keyword">configurable</span></span> is <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> for
              all properties?
            </p>
          </th>
          <th>
            <p xmlns:util="util">
              <span sdata="langKeyword" value="writable"><span class="keyword">writable</span></span> is <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> for all data
              properties?
            </p>
          </th>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Object.isExtensible
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Object.isSealed
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No
            </p>
          </td>
        </tr>
        <tr>
          <td>
            <p xmlns:util="util">
              Object.isFrozen
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              No
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
          <td>
            <p xmlns:util="util">
              Yes
            </p>
          </td>
        </tr>
      </table>
    </div>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>Object.preventExtensions</b> function.
</p>

```
// Create an object that has two properties. var obj = { pasta: "spaghetti", length: 10 }; // Make the object non-extensible. Object.preventExtensions(obj); document.write(Object.isExtensible(obj));
document.write("&lt;br/&gt;"); // Try to add a new property, and then verify that it is not added. obj.newProp = 50; document.write(obj.newProp); // Output: // false // undefined
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Internet Explorer 9 standards and Internet Explorer 10 standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="e72c804a-4dab-4ec9-b9df-9c9c908aa12d.htm">Object.seal Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="83ffe193-0a37-4e0c-9b66-44c422765fb3.htm">Object.freeze Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="a7d10beb-0d01-4e2d-8263-59ff07ac4352.htm">Object.isExtensible Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="af4f192e-cebe-44b9-8eef-90c096f5ae8f.htm">Object.isSealed Function (JavaScript)</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="6cf1bbc6-56e8-429b-8e2c-0024fa614acc.htm">Object.isFrozen Function (JavaScript)</a></span>
  </div>
</div>

