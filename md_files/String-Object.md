## [String Object (JavaScript)](String-Object.html)

### Introduction 

 Allows manipulation and formatting of text strings and determination and location of substrings within strings.

### Syntax 

```
newString = new String(["stringLiteral "])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">newString</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringLiteral</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Any group of Unicode characters.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    JavaScript provides escape sequences that you can include in strings to create characters that you cannot type directly. For example, <span class="code">\t</span> specifies a tab character. For
    more information, see <span sdata="link">Special Characters (JScript)</span>.
  </p>
  <h3 class="subHeading">
    String Literals
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      A <span class="term">string literal</span> is zero or more characters enclosed in single or double quotation marks. A string literal has a primary (primitive) data type of <span sdata=
      "langKeyword" value="string"><span class="keyword">string</span></span>. A <span class="term">String object</span> is created by using the new Operator, and has a data type of <b>Object</b>.
    </p>
    <p xmlns:util="util">
      The following example shows that the data type of a string literal is not the same as that of a <b>String</b> object.
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
 var strLit = "This is a string literal."; var strObj = new String("This is a string object.");  document.write(typeof strLit); document.write("&lt;br/&gt;"); document.write(typeof strObj); // Output: // string // object 
</pre>
          </td>
        </tr>
      </table>
    </div>
  </div>
  <h3 class="subHeading">
    Methods for String Literals
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      When you call a method on a string literal, it is temporarily converted to a string wrapper object. The string literal is treated as though the <b>new</b> operator were used to create it.
    </p>
    <p xmlns:util="util">
      The following example applies the <b>toUpperCase</b> method to a string literal.
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
 var strLit = "This is a string literal.";  var result1 = strLit.toUpperCase();  var result2 = (new String(strLit)).toUpperCase();  document.write(result1); document.write("&lt;br/&gt;"); document.write(result2); // Output:  // THIS IS A STRING LITERAL. // THIS IS A STRING LITERAL. 
</pre>
          </td>
        </tr>
      </table>
    </div>
  </div>
  <h3 class="subHeading">
    Accessing an Individual Character
  </h3>
  <div class="subsection">
    <p xmlns:util="util">
      You can access an individual character of a string as a read-only array-indexed property. This feature was introduced in Internet Explorer 9 standards mode, Internet Explorer 10 standards mode,
      and win8_appname_long apps. The following example accesses individual string characters.
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
 var str = "abcd"; var result = str[2]; document.write (result); // Output: c  var result = "the"[0]; document.write(result); // Output: t 
</pre>
          </td>
        </tr>
      </table>
    </div>
  </div>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>String Object</b> was introduced in Internet Explorer before Internet Explorer 6. Some members in the following lists were introduced in later versions.
  </p>
</div>

#### Properties 

<div id="sectionSection4" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the properties of the <b>String</b> object.
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
            Specifies the function that creates an object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            length Property (String)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the length of a <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object.
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
            Returns a reference to the prototype for a class of objects.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Functions 

<div id="sectionSection5" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the functions of the <b>String</b> object.
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
            Description
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            String.fromCharCode Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string from a number of Unicode character values.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Methods 

<div id="sectionSection6" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists the methods of the <b>String</b> object.
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
            anchor Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places an HTML anchor that has a NAME attribute around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            big Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;BIG&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            blink Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;BLINK&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            bold Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;B&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            charAt Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the character at the specified index.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            charCodeAt Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the Unicode encoding of the specified character.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            concat Method (String)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string that contains the concatenation of two supplied strings.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            fixed Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;TT&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            fontcolor Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;FONT&gt; tags with a COLOR attribute around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            fontsize Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;FONT&gt; tags with a SIZE attribute around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            hasOwnProperty Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether an object has a property with the specified name.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            indexOf Method (String)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the character position where the first occurrence of a substring occurs within a string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            isPrototypeOf Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether an object exists in another object's prototype chain.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            italics Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;I&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            lastIndexOf Method (String)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the last occurrence of a substring within a string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            link Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places an HTML anchor that has an HREF attribute around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            localeCompare Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a value that indicates whether two strings are equivalent in the current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            match Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Searches a string by using a supplied <b>Regular Expression</b> object and returns the results as an array.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            propertyIsEnumerable Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether a specified property is part of an object and whether it is enumerable.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            replace Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Uses a regular expression to replace text in a string and returns the result.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            search Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the position of the first substring match in a regular expression search.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            slice Method (String)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a section of a string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            small Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;SMALL&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            split Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the array of strings that results when a string is separated into substrings.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            strike Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;STRIKE&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            sub Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;SUB&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            substr Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a substring beginning at a specified location and having a specified length.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            substring Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the substring at a specified location within a <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            sup Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Places HTML &lt;SUP&gt; tags around text.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toLocaleLowerCase Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string in which all alphabetic characters are converted to lowercase, taking into account the host environment's current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toLocaleString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an object converted to a string, using the current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toLocaleUpperCase Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string in which all alphabetic characters are converted to uppercase, taking into account the host environment's current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toLowerCase Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string in which all alphabetic characters are converted to lowercase.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the string.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toUpperCase Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string in which all alphabetic characters are converted to uppercase.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            trim Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string with leading and trailing white space and line terminator characters removed.
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
            Returns the string.
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
    <span sdata="link" xmlns:util="util"><a href="5ea556ba-7ae6-426c-8430-9032eee5a0a5.htm">new Operator (JavaScript)</a></span>
  </div>
</div>

