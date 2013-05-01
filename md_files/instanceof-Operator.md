## [instanceof Operator (JavaScript)](instanceof-Operator.html)

### Introduction 

 Returns a Boolean value that indicates whether or not an object is an instance of a particular class.

### Syntax 

```
result = object instanceof class
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">result</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any variable.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">object</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any object expression.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">class</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. Any defined object class.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>instanceof</b> operator returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if <span class="parameter" sdata="paramReference">object</span> is an
    instance of <span class="parameter" sdata="paramReference">class</span>. It returns <span sdata="langKeyword" value="false"><span class="keyword">false</span></span> if <span class="parameter"
    sdata="paramReference">object</span> is not an instance of <span class="parameter" sdata="paramReference">class</span>, or if <span class="parameter" sdata="paramReference">object</span> is
    <span sdata="langKeyword" value="null"><span class="keyword">null</span></span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example shows how to use the <b>instanceof</b> operator.
</p>

```
function objTest(obj){ var i, t, s = ""; t = new Array(); t["Date"] = Date; t["Object"] = Object; t["Array"] = Array; for (i in t){ if (obj instanceof t[i]) { s += "obj is an instance of " + i +
"&lt;br/&gt;"; } else { s += "obj is not an instance of " + i + "&lt;br/&gt;"; } } return(s); } var obj = new Date(); document.write(objTest(obj)); // Output: // obj is an instance of Date // obj is
an instance of Object // obj is not an instance of Array
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
    <span sdata="link" xmlns:util="util">Operator Precedence</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Operator Summary</span>
  </div>
</div>

