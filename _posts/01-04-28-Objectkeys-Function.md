---
title: Object.keys Function (JavaScript)
---

### Introduction 

 Returns the names of the enumerable properties and methods of an object.

### Syntax 

```
Object.keys(object )
```

#### Parameters 

<div id="parametersSection" class="section" name="collapseableSection" style="">
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Parameter
          </p>
        </th>
        <th>
          <p xmlns:util="util">
            Definition
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            <span class="parameter" sdata="paramReference">object</span>
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Required. The object that contains the properties and methods. This can be an object that you created or an existing Document Object Model (DOM) object.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Return Value 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    An array that contains the names of the enumerable properties and methods of the object.
  </p>
</div>

#### Exceptions 

<div id="ddueExceptionsSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    If the value supplied for the <span class="parameter" sdata="paramReference">object</span> argument is not the name of an object, a <span sdata="langKeyword" value="TypeError"><span class=
    "keyword">TypeError</span></span> exception is thrown.
  </p>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>keys</b> method returns only the names of enumerable properties and methods. To return the names of both enumerable and non-enumerable properties and methods, you can use <span sdata=
    "link"><a href="59f4b6b1-02be-44b3-a06c-a5ca8f70c3d8.htm">Object.getOwnPropertyNames Function (JavaScript)</a></span>.
  </p>
  <p xmlns:util="util">
    For information about the <span sdata="langKeyword" value="enumerable"><span class="keyword">enumerable</span></span> attribute of a property, see <span sdata="link"><a href=
    "c5d05346-940a-40c2-b12a-e8b25abc8d46.htm">Object.defineProperty Function (JavaScript)</a></span> and <span sdata="link"><a href=
    "8f0e1c90-c4f9-44c4-bf76-726bacecbc14.htm">Object.getOwnPropertyDescriptor Function (JavaScript)</a></span>.
  </p>
  <p xmlns:util="util"></p>
</div>

#### Example 

<p xmlns:util="util">
  The following example creates an object that has three properties and a method. It then uses the <b>keys</b> method to get the properties and methods of the object.
</p>

```
// Create a constructor function. function Pasta(grain, width, shape) { this.grain = grain; this.width = width; this.shape = shape; // Define a method. this.toString = function () { return
(this.grain + ", " + this.width + ", " + this.shape); } } // Create an object. var spaghetti = new Pasta("wheat", 0.2, "circle"); // Put the enumerable properties and methods of the object in an
array. var arr = Object.keys(spaghetti); document.write (arr); // Output: // grain,width,shape,toString
```

<p xmlns:util="util">
  The following example displays the names of all enumerable properties that start with the letter "g" in the Pasta object.
</p>

```
// Create a constructor function. function Pasta(grain, width, shape) { this.grain = grain; this.width = width; this.shape = shape; } var polenta = new Pasta("corn", 1, "mush"); var keys =
Object.keys(polenta).filter(CheckKey); document.write(keys); // Check whether the first character of a string is "g". function CheckKey(value) { var firstChar = value.substr(0, 1); if
(firstChar.toLowerCase() == "g") return true; else return false; } // Output: // grain
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util"></p>
  <p>
    Supported in the following document modes: Internet Explorer 9 standards and Internet Explorer 10 standards. Also supported in Windows Store apps. See Version Information.
  </p>
  <p>
    Not supported in the following document modes: Quirks, Internet Explorer 6 standards, Internet Explorer 7 standards, Internet Explorer 8 standards.
  </p>
</div>

#### See Also 

<div id="seeAlsoSection" class="section" name="collapseableSection" style="">
  <h4 class="subHeading">
    Other Resources
  </h4>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="59f4b6b1-02be-44b3-a06c-a5ca8f70c3d8.htm">Object.getOwnPropertyNames Function (JavaScript)</a></span>
  </div>
</div>

