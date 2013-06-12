---
title: JavaScript Properties
---

### Introduction 

 The following table lists JavaScript properties.

#### Properties 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
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
        <th>
          <p xmlns:util="util">
            JavaScript object
          </p>
        </th>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            0...n Properties
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the value of individual arguments from an <b>arguments</b> object.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>arguments</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            $1...$9 Properties
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the nine most-recently memorized portions found during pattern matching.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>RegExp</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            arguments Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an array containing each argument passed to the currently executing function.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Function</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            callee Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the <span sdata="langKeyword" value="Function"><span class="keyword">Function</span></span> object being executed.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>arguments</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            caller Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a reference to the function that invoked the current function.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Function</b>
          </p>
        </td>
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
        <td>
          <p xmlns:util="util">
            Multiple
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            description Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns or sets the descriptive string associated with a specific error.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Error</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            global Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value indicating the state of the global flag (<b>g</b>) used with a regular expression.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Regular Expression</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            ignoreCase Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value indicating the state of the ignoreCase flag (<b>i</b>) used with a regular expression.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Regular Expression</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            index Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the character position where the first successful match begins in a searched string.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>RegExp</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            input Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the string against which a search was performed.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>RegExp</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            lastIndex Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the character position where the last successful match begins in a searched string.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>RegExp</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            lastMatch Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the last matched characters from any regular expression search.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>RegExp</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            lastParen Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the last parenthesized submatch from any regular expression search, if any.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>RegExp</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            leftContext Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the characters from the beginning of a searched string up to the position before the beginning of the last match.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>RegExp</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            length Property (arguments)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the actual number of arguments passed to a function by the caller.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>arguments</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            length Property (Array)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an integer value one higher than the highest element defined in an array.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Array</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            length Property (Function)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the number of arguments defined for a function.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Function</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            length Property (String)
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the length of a <span sdata="langKeyword" value="String"><span class="keyword">String</span></span> object.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>String</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            message Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an error message string.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Error</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            multiline Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value indicating the state of the multiline flag (<b>m</b>) used with a regular expression.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Regular Expression</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            name Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the name of an error.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Error</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            number Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns or sets the numeric value associated with a specific error.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Error</b>
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
        <td>
          <p xmlns:util="util">
            Multiple
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            rightContext Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the characters from the position following the last match to the end of the searched string.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>RegExp</b>
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            source Property
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a copy of the text of the regular expression pattern.
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            <b>Regular Expression</b>
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
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="35b141cc-8116-47b1-bc0b-0f22e182f7e7.htm">JavaScript Constants</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="003747e2-7860-4c96-b129-5180ae0fe745.htm">JavaScript Methods</a></span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util"><a href="63cf9c47-9312-40c1-a4af-84547a7e5512.htm">JavaScript Functions</a></span>
  </div>
</div>

