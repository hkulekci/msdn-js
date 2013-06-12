---
title: slice Method (String) (JavaScript)
isChild: false
---

## slice Method (String) (JavaScript) {slice_method_string_javascript_title}

### Introduction 

 Returns a section of a string.

### Syntax 

```
stringObj .slice(start , [end ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">stringObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. A <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">start</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The index to the beginning of the specified portion of <span class="parameter" sdata="paramReference">stringObj</span>.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">end</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The index to the end of the specified portion of <span class="parameter" sdata="paramReference">stringObj</span>. The substring includes the characters up to, but not including, the
        character indicated by <span class="parameter" sdata="paramReference">end</span>. If this value is not specified, the substring continues to the end of <span class="parameter" sdata=
        "paramReference">stringObj</span>.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>slice</b> method returns a <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object containing the specified portion of <span class="parameter" sdata=
    "paramReference">stringObj</span>.
  </p>
  <p xmlns:util="util">
    The <b>slice</b> method copies up to, but not including, the character indicated by <span class="parameter" sdata="paramReference">end</span>.
  </p>
  <p xmlns:util="util">
    If <span class="parameter" sdata="paramReference">start</span> is negative, it is treated as <i>length</i> + <span class="parameter" sdata="paramReference">start</span> where <i>length</i> is the
    length of the string. If <span class="parameter" sdata="paramReference">end</span> is negative, it is treated as <i>length</i> + <span class="parameter" sdata="paramReference">end</span>. If
    <span class="parameter" sdata="paramReference">end</span> is omitted, copying continues to the end of <span class="parameter" sdata="paramReference">stringObj</span>. If <span class="parameter"
    sdata="paramReference">end</span> occurs before <span class="parameter" sdata="paramReference">start</span>, no characters are copied to the new string.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  In the first example, the <span sdata="langKeyword" value="slice"><span class="keyword">slice</span></span> method returns the entire string. In the second example, the <span sdata="langKeyword"
  value="slice"><span class="keyword">slice</span></span> method returns the entire string, except for the last character.
</p>

```
var str1 = "all good boys do fine"; var slice1 = str1.slice(0); var slice2 = str1.slice(0,-1); var slice3 = str1.slice(4); var slice4 = str1.slice(4, 8); document.write(slice1 + "&lt;br/&gt;");
document.write(slice2 + "&lt;br/&gt;"); document.write(slice3 + "&lt;br/&gt;"); document.write(slice4); // Output: // all good boys do fine // all good boys do fin // good boys do fine // good
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
    <span sdata="link" xmlns:util="util"><a href="3c122219-14de-4126-b091-809659c026d6.htm">slice Method (Array) (JavaScript)</a></span>
  </div>
</div>

