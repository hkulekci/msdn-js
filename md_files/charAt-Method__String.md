## [charAt Method (String) (JavaScript)](charAt-Method__String.html)

### Introduction 

 Returns the character at the specified index.

### Syntax 

```
strObj . charAt(index )
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">strObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object or string literal.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">index</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The zero-based index of the desired character.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>charAt</b> method returns a character value equal to the character at the specified <span class="parameter" sdata="paramReference">index</span>. The first character in a string is at index
    0, the second is at index 1, and so forth. Values of <span class="parameter" sdata="paramReference">index</span> that are out of range return an empty string.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <b>charAt</b> method:
</p>

```
var str = "ABCDEFGHIJKLMNOPQRSTUVWXYZ"; document.write(str.charAt(str.length - 1)); // Output: Z
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
    <span sdata="link" xmlns:util="util"><a href="8063ecd5-5778-4e87-b985-b21420171914.htm">String Object (JavaScript)</a></span>
  </div>
</div>

