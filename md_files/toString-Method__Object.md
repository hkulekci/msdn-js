## [toString Method (Object) (JavaScript)](toString-Method__Object.html)

### Introduction 

 Returns a string representation of an object.

### Syntax 

```
objectname .toString([radix ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">objectname</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. An object for which a string representation is sought.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">radix</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Specifies a radix for converting numeric values to strings. This value is only used for numbers.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>toString</b> method is a member of all built-in JavaScript objects. How it behaves depends on the object type:
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Object
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Behavior
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Array
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Elements of an <b>Array</b> are converted to strings. The resulting strings are concatenated, separated by commas.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Boolean
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            If the Boolean value is <b>true</b>, returns "<span class="code">true</span>". Otherwise, returns "<span class="code">false</span>".
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Date
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the textual representation of the date.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Error
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string containing the associated error message.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string of the following form, where <i>functionname</i> is the name of the function whose <b>toString</b> method was called:
          </p>
          <div class="code">
            <table width="100%" cellspacing="0" cellpadding="0">
              <tr>
                <th>
                  &nbsp;
                </th>
                <th>
                  <span class="copyCode" onclick="CopyCode(this)" onkeypress="CopyCode_CheckKey(this, event)" onmouseover="ChangeCopyCodeIcon(this)" onmouseout="ChangeCopyCodeIcon(this)" tabindex=
                  "0"><img class="copyCodeImage" name="ccImage" align="absmiddle" alt="Copy image" title="Copy image" src="../icons/copycode.gif" />Copy Code</span>
                </th>
              </tr>
              <tr>
                <td colspan="2">
                  <pre>
 function functionname( ) { [native code] } 
</pre>
                </td>
              </tr>
            </table>
          </div>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Number
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the textual representation of the number.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            String
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the value of the <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Default
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns <span class="code">"[object objectname]"</span>, where <span class="code">objectname</span> is the name of the object type.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>toString</b> method with a radix argument. The return value of function shown below is a Radix conversion table.
</p>

```
function CreateRadixTable (){ var s = ""; // Create table heading. s += "Hex Dec Bin \n"; for (x = 0; x &lt; 16; x++) { s += " "; // Convert to hexidecimal. s += x.toString(16); s += " "; if (x &lt;
10) s += " "; // Convert to decimal. s += x.toString(10); s += " "; // Convert to binary. s += x.toString(2); s += "\n"; } return(s); }
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="08e5f552-0797-4b48-8164-609582fc18c9.htm">Array Object (JavaScript)</a></span>| <span sdata="link"><a href=
    "d67748f2-7bf5-4889-8269-e777616cc5f0.htm">Boolean Object (JavaScript)</a></span>| <span sdata="link"><a href="ce2202bb-7ec9-4f5a-bf48-3a04feff283e.htm">Date Object (JavaScript)</a></span>|
    <span sdata="link"><a href="0b27d6ec-3997-4e91-a6c0-5afbaf494db7.htm">Error Object (JavaScript)</a></span>| <span sdata="link"><a href="d3834767-203c-475e-848c-95c423ba15b6.htm">Function Object
    (JavaScript)</a></span>| <span sdata="link"><a href="76e87c37-cf6c-46cc-bafa-04be1fe3d78d.htm">Number Object (JavaScript)</a></span>| <span sdata="link"><a href=
    "d24ef8fc-217b-4828-94e1-19f72780bae0.htm">Object Object (JavaScript)</a></span>| <span sdata="link"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
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

