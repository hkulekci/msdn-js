---
title: HTML Tag Methods (JavaScript)
isChild: false
---

## HTML Tag Methods (JavaScript) {html_tag_methods_javascript_title}

### Introduction 

 You can use HTML tag methods to place HTML elements around text in a String object.

#### Syntax 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the syntax for and a description of each HTML tag method.
  </p>
  <p xmlns:util="util">
    In the Syntax column, <span class="parameter" sdata="paramReference">string1</span> is a <b>String</b> object or literal.
  </p>
  <p xmlns:util="util">
    The Standard column indicates <a href="http://go.microsoft.com/fwlink/?LinkId=199553">World Wide Web Consortium (W3C)</a> recommendations for HTML 4. "Discouraged" indicates that the HTML element
    is discouraged in favor of style sheets.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Syntax
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Method description
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Parameter description
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Standard
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.anchor(<span class="parameter" sdata="paramReference">name</span>)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places an HTML anchor that has a NAME attribute around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The <span class="parameter" sdata="paramReference">name</span> parameter is text to put in the NAME attribute of the HTML anchor.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.big()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;BIG&gt; tags around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util">
            Discouraged
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.blink()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;BLINK&gt; tags around the text. The &lt;BLINK&gt; tag is not supported in Internet Explorer.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util">
            Not in standard
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.bold()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;B&gt; tags around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util">
            Discouraged
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.fixed()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;TT&gt; tags around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util">
            Discouraged
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.fontcolor(<span class="parameter" sdata="paramReference">color</span>)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;FONT&gt; tags with a COLOR attribute around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The <span class="parameter" sdata="paramReference">color</span> parameter is a string value that contains the hexadecimal value or predefined name for a color. Valid predefined color
            names depend on the JavaScript host browser and its version.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Deprecated
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.fontsize(<span class="parameter" sdata="paramReference">size</span>)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;FONT&gt; tags with a SIZE attribute around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The <span class="parameter" sdata="paramReference">size</span> parameter is an integer value that specifies the size of the text. Valid integer values depend on the JavaScript host
            browser and its version.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Deprecated
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.italics()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;I&gt; tags around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util">
            Discouraged
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.link(<span class="parameter" sdata="paramReference">href</span>)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places an HTML anchor that has an HREF attribute around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The <span class="parameter" sdata="paramReference">href</span> parameter is text to put in the HREF attribute of the HTML anchor.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.small()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;SMALL&gt; tags around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util">
            Discouraged
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.strike()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;STRIKE&gt; tags around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util">
            Deprecated
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.sub()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;SUB&gt; tags around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">string1</span>.sup()
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;SUP&gt; tags around the text.
          </p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
        <td>
          <p xmlns:util="util"></p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Remarks 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    No checking is performed to determine whether the HTML tags have already been applied to the string.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following examples show how to use the HTML tag methods.
</p>

```
// anchor method. var strVariable = "This is an anchor."; document.write(strVariable.anchor("Anchor1")); // Output: &lt;A NAME="Anchor1"&gt;This is an anchor.&lt;/A&gt; // big method. var strVariable
= "This is a string."; document.write(strVariable.big()); // Output: &lt;BIG&gt;This is a string.&lt;/BIG&gt; // blink method. var strVariable = "This is a string.";
document.write(strVariable.blink()); // Output: &lt;BLINK&gt;This is a string.&lt;/BLINK&gt; // bold method. var strVariable = "This is a string."; document.write(strVariable.bold()); // Output:
&lt;B&gt;This is a string.&lt;/B&gt; // fixed method. var strVariable = "This is a string."; document.write(strVariable.fixed()); // Output: &lt;TT&gt;This is a string.&lt;/TT&gt; // fontcolor
method. var strVariable = "This is a string."; document.write(strVariable.fontcolor("red")); // Output: &lt;FONT COLOR="red"&gt;This is a string.&lt;/FONT&gt; // fontsize method. var strVariable =
"This is a string."; document.write(strVariable.fontsize(-1)); // Output: &lt;FONT SIZE="-1"&gt;This is a string.&lt;/FONT&gt; // italics method var strVariable = "This is a string.";
document.write(strVariable.italics()); // Output: &lt;I&gt;This is a string.&lt;/I&gt; // link method. var strVariable = "This is a hyperlink.";
document.write(strVariable.link("http://www.microsoft.com")); // Output: &lt;A HREF="http://www.microsoft.com"&gt;This is a hyperlink.&lt;/A&gt; // small method. var strVariable = "This is a
string."; document.write(strVariable.small()); // Output: &lt;SMALL&gt;This is a string.&lt;/SMALL&gt; // strike method. var strVariable = "This is a string."; document.write(strVariable.strike());
// Output: &lt;STRIKE&gt;This is a string.&lt;/STRIKE&gt; // sub method. var strVariable = "This is a string."; document.write(strVariable.sub()); // Output: &lt;SUB&gt;This is a string.&lt;/SUB&gt;
// sup method. var strVariable = "This is a string."; document.write(strVariable.sup()); // Output: &lt;SUP&gt;This is a string.&lt;/SUP&gt;
```

#### Requirements 

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards, Internet Explorer 9 standards, Internet Explorer 10
    standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p xmlns:util="util">
    <b>Applies To</b>: <span sdata="link"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

