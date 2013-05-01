## [concat Method (String) (JavaScript)](concat-Method__String.html)

### Introduction 

 Returns a string that contains the concatenation of two or more strings.

### Syntax 

```
string1 . concat([string2 [, string3 [, . . . [, stringN ]]]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">string1</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal to which all other specified strings are concatenated.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">string2,. . ., stringN</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The strings to append to the end of <span class="parameter" sdata="paramReference">string1</span>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The result of the <b>concat</b> method is equivalent to: <span class="parameter" sdata="paramReference">result</span> = <span class="parameter" sdata="paramReference">string1</span> +
    <span class="parameter" sdata="paramReference">string2</span> + <span class="parameter" sdata="paramReference">string3</span> + <span class="parameter" sdata="paramReference">stringN</span>. A
    change of value in either a source or result string does not affect the value in the other string. If any of the arguments are not strings, they are first converted to strings before being
    concatenated to <span class="parameter" sdata="paramReference">string1</span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>concat</b> method when used with a string:
</p>

```
var str1 = "ABCD" var str2 = "EFGH"; var str3 = "1234"; var str4 = "5678"; document.write(str1.concat(str2, str3, str4)); // Output: "ABCDEFGH12345678"
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
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
    <span sdata="link" xmlns:util="util"><a href="ec1237d3-e78b-4e77-bd7d-c0204cf03acd.htm">Addition Operator (+) (JavaScript)</a></span>
  </div>
</div>

