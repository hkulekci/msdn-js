---
title: substring Method (String) (JavaScript)
---

### Introduction 

 Returns the substring at the specified location within a String object.

### Syntax 

```
strVariable . substring(start [, end ]) "String Literal".substring(start [, end ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">start</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The zero-based index integer indicating the beginning of the substring.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">end</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. The zero-based index integer indicating the end of the substring. The substring includes the characters up to, but not including, the character indicated by <span class="parameter"
        sdata="paramReference">end</span>.
      </p>
      <p xmlns:util="util">
        If <span class="parameter" sdata="paramReference">end</span> is omitted, the characters from <span class="parameter" sdata="paramReference">start</span> through the end of the original string
        are returned.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="substring"><span class="keyword">substring</span></span> method returns a string containing the substring from <span class="parameter" sdata=
    "paramReference">start</span> up to, but not including, <span class="parameter" sdata="paramReference">end</span>.
  </p>
  <p xmlns:util="util">
    The <b>substring</b> method uses the lower value of <span class="parameter" sdata="paramReference">start</span> and <span class="parameter" sdata="paramReference">end</span> as the beginning
    point of the substring. For example, strvar.substring(0, 3<b>)</b> and strvar.substring(3, 0) return the same substring.
  </p>
  <p xmlns:util="util">
    If either <span class="parameter" sdata="paramReference">start</span> or <span class="parameter" sdata="paramReference">end</span> is <b>NaN</b> or negative, it is replaced with zero.
  </p>
  <p xmlns:util="util">
    The length of the substring is equal to the absolute value of the difference between <span class="parameter" sdata="paramReference">start</span> and <span class="parameter" sdata=
    "paramReference">end</span>. For example, the length of the substring returned in strvar.substring(0, 3) and strvar.substring(3, 0) is three.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>substring</b> method.
</p>

```
var s = "The quick brown fox jumps over the lazy dog."; var ss = s.substring(10, 15); document.write(ss); // Output: // brown
```

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
    <span sdata="link" xmlns:util="util"><a href="f12541c1-2623-482e-941d-2e22bc3c4a4a.htm">substr Method (String) (JavaScript)</a></span>
  </div>
</div>

