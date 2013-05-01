## [Object.getOwnPropertyNames Function (JavaScript)](Object.getOwnPropertyNames-Function.html)

### Introduction 

 Returns the names of the own properties of an object. The own properties of an object are those that are defined directly on that object, and are not inherited from the object's prototype. The
properties of an object include both fields (objects) and functions.

### Syntax 

```
Object.getOwnPropertyNames(object )
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
            Required. The object that contains the own properties.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Return Value 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    An array that contains the names of the own properties of the object.
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
    The <b>getOwnPropertyNames</b> method returns the names of both enumerable and non-enumerable properties and methods. To return only the names of enumerable properties and methods, you can use
    the <span sdata="link"><a href="cf4a7daf-cf28-4467-bc6b-f7f106ec3876.htm">Object.keys Function (JavaScript)</a></span>.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example creates an object that has three properties and a method. It then uses the <b>getOwnPropertyNames</b> method to obtain the own properties (including the method) of the object.
</p>

```
function Pasta(grain, width, shape) { // Define properties. this.grain = grain; this.width = width; this.shape = shape; this.toString = function () { return (this.grain + ", " + this.width + ", " +
this.shape); } } // Create an object. var spaghetti = new Pasta("wheat", 0.2, "circle"); // Get the own property names. var arr = Object.getOwnPropertyNames(spaghetti); document.write (arr); //
Output: // grain,width,shape,toString
```

<p xmlns:util="util">
  The following example displays the names of properties that start with the letter 's' in a <span class="input">spaghetti</span> object constructed with the <span class="input">Pasta</span>
  constructor.
</p>

```
function Pasta(grain, size, shape) { this.grain = grain; this.size = size; this.shape = shape; } var spaghetti = new Pasta("wheat", 2, "circle"); var names =
Object.getOwnPropertyNames(spaghetti).filter(CheckKey); document.write(names); // Check whether the first character of a string is 's'. function CheckKey(value) { var firstChar = value.substr(0, 1);
if (firstChar.toLowerCase() == 's') return true; else return false; } // Output: // size,shape
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
    <span sdata="link" xmlns:util="util"><a href="cf4a7daf-cf28-4467-bc6b-f7f106ec3876.htm">Object.keys Function (JavaScript)</a></span>
  </div>
</div>

