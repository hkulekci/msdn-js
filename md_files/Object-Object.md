## [Object Object (JavaScript)](Object-Object.html)

### Introduction 

 Provides functionality common to all JavaScript objects.

### Syntax 

```
obj = new Object([value ])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">obj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <span sdata="langKeyword" value="Object"><span class="keyword">Object</span></span> object is assigned.
      </p>
    </dd>
    <dt>
      <i xmlns:util="util">value</i>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Any one of the JavaScript primitive data types (Number, Boolean, or String). If value is an object, the object is returned unmodified. If <i>value</i> is <span sdata="langKeyword"
        value="null"><span class="keyword">null</span></span>, <b>undefined</b>, or not supplied, an object with no content is created.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <span sdata="langKeyword" value="Object"><span class="keyword">Object</span></span> object is contained in all other JavaScript objects; all of its methods and properties are available in all
    other objects. The methods can be redefined in user-defined objects, and are called by JavaScript at appropriate times. The <b>toString</b> method is an example of a frequently redefined
    <span sdata="langKeyword" value="Object"><span class="keyword">Object</span></span> method.
  </p>
  <p xmlns:util="util">
    In this language reference, the description of each <span sdata="langKeyword" value="Object"><span class="keyword">Object</span></span> method includes both default and object-specific
    implementation information for the intrinsic JavaScript objects.
  </p>
</div>

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Object Object</b> was introduced in Internet Explorer before Internet Explorer 6. Some members in the following lists were introduced in later versions.
  </p>
</div>

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists properties of the <b>Object Object</b>.
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

<div id="sectionSection2" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists functions of the <b>Object Object</b>.
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
            Object.create Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Creates an object that has a specified prototype, and that optionally contains specified properties.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.defineProperties Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Adds one or more properties to an object, and/or modifies attributes of existing properties.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.defineProperty Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Adds a property to an object, or modifies attributes of an existing property.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.freeze Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Prevents the modification of existing property attributes and values, and prevents the addition of new properties.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.getOwnPropertyDescriptor Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the definition of a data property or an accessor property.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.getOwnPropertyNames Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the names of the properties and methods of an object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.getPrototypeOf Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the prototype of an object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.isExtensible Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a value that indicates whether new properties can be added to an object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.isFrozen Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if existing property attributes and values cannot be modified in an object and new properties
            cannot be added to the object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.isSealed Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns <span sdata="langKeyword" value="true"><span class="keyword">true</span></span> if existing property attributes cannot be modified in an object and new properties cannot be added
            to the object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.keys Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the names of the enumerable properties and methods of an object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.preventExtensions Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Prevents the addition of new properties to an object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Object.seal Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Prevents the modification of attributes of existing properties, and prevents the addition of new properties.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Methods 

<div id="sectionSection3" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists methods of the <b>Object Object</b>.
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
            hasOwnProperty method
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
            isPrototypeOf method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether an object exists in another object's prototype hierarchy.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            propertyIsEnumerable method
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
            toLocaleString method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an object converted to a string based on the current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toString method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a string representation of an object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            valueOf method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the primitive value of the specified object.
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
    <span sdata="link" xmlns:util="util"><a href="4a29a831-41c9-4843-9385-c3879e385585.htm">JavaScript Objects</a></span>
  </div>
</div>

