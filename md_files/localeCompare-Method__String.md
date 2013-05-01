## [localeCompare Method (String) (JavaScript)](localeCompare-Method__String.html)

### Introduction 

 Determines whether two strings are equivalent in the current locale.

### Syntax 

```
stringVar .localeCompare(stringExp )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringVar</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringExp</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. String to compare to <span class="parameter" sdata="paramReference">stringVar</span>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>localeCompare</b> performs a locale-sensitive string comparison of the <span class="parameter" sdata="paramReference">stringVar</span> and the <span class="parameter" sdata=
    "paramReference">stringExp</span> and returns -1, 0, or +1, depending on the sort order of the system default locale.
  </p>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">stringVar</span> sorts before <span class="parameter" sdata="paramReference">stringExp</span>, <b>localeCompare</b> returns &#8211;1; if
    <span class="parameter" sdata="paramReference">stringVar</span> sorts after <span class="parameter" sdata="paramReference">stringExp</span>, +1 is returned. A return value of zero means that the
    two strings are equivalent.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following code shows how to use <b>localeCompare</b>.
</p>

```
var str1 = "def"; var str2 = "abc" document.write(str1.localeCompare(str2) + "&lt;br/&gt;"); // Output: 1 var str3 = "ghi"; document.write(str1.localeCompare(str3)+ "&lt;br/&gt;"); // Output: -1 var
str4 = "def"; document.write(str1.localeCompare(str4)); // Output: 0
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
    <span sdata="link" xmlns:util="util"><a href="0901afcb-126b-4ed7-bd6a-2301d50e2326.htm">toLocaleString Method (Object) (JavaScript)</a></span>
  </div>
</div>

