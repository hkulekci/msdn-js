## [this Statement (JavaScript)](this-Statement.html)

### Introduction 

 Refers to the current object.

### Syntax 

```
this.property
```

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The required <span class="parameter" sdata="paramReference">property</span> argument is one of the current object's properties
  </p>
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="this"><span class="keyword">this</span></span> keyword can be used in object constructors to refer to the current object.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  In the following example, <b>this</b> refers to the newly created Car object, and assigns values to three properties:
</p>

```
function Car(color, make, model){ this.color = color; this.make = make; this.model = model; }
```

<p xmlns:util="util">
  The <b>this</b> keyword generally refers to the <b>window</b> object if used outside of the scope of any other object. However, inside event handlers <span sdata="langKeyword" value=
  "this"><span class="keyword">this</span></span> refers to the DOM element that raised the event.
</p>

```
document.getElementById("clicker").addEventListener("click", eventHandler, false); function eventHandler(ev) { document.write(this.toString()); } // Output (when you click the button): [object
HTMLButtonElement]
```

<p xmlns:util="util">
  In the following code (for Internet Explorer 9 and later), the event handler prints the string version of a button that has an ID of "clicker".
</p>

```
<p xmlns:util="util">
  In the following code (for Internet Explorer 9 and later), the event handler prints the string version of a button that has an ID of "clicker".
</p>
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
    <span sdata="link" xmlns:util="util"><a href="5ea556ba-7ae6-426c-8430-9032eee5a0a5.htm">new Operator (JavaScript)</a></span>
  </div>
</div>

