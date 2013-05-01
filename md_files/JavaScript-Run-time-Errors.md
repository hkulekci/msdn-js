## [JavaScript Run-time Errors](JavaScript-Run-time-Errors.html)

### Introduction 

 JavaScript run-time errors are errors that occur when your script attempts to perform an action that the system cannot execute. You may see run-time errors when variable expressions are being
evaluated or memory is being allocated.

#### Windows Runtime Errors 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    If you are using Windows Runtime APIs in your Windows Store app, you may see JavaScript errors that have been converted from Windows Runtime HRESULTs. Windows Runtime HRESULTs in the range over
    0x80070000 are converted to JavaScript errors by taking the hexadecimal value of the low bits and converting it to a decimal. For example, the HRESULT 0x80070032 is converted to the decimal value
    50, and the JavaScript error is SCRIPT50. The HRESULT 0x80074005 is converted to the decimal value 16389, and the JavaScript error is SCRIPT16389.
  </p>
</div>

#### Errors 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Error Number
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
            1001
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Out of memory
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5029
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Array length must be a finite positive integer
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5030
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Array length must be assigned a finite positive number
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5028
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Array or arguments object expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5010
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Boolean expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5003
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Cannot assign to a function result
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5000
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Cannot assign to 'this'
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5034
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Circular reference in value argument not supported
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5006
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Date object expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5015
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Enumerator object expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5022
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Exception thrown and not caught
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5020
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Expected ')' in regular expression
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5019
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Expected ']' in regular expression
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5023
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Function does not have a valid prototype object
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5002
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Function expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5008
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Illegal assignment
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5021
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Invalid range in character set
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5035
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Invalid replacer argument
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5014
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            JavaScript object expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5001
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Number expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5007
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Object expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5012
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Object member expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5016
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Regular Expression object expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5005
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            String expected
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5017
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Syntax error in regular expression
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5026
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The number of fractional digits is out of range
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5027
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The precision is out of range
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5025
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The URI to be decoded is not a valid encoding
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5024
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            The URI to be encoded contains an invalid character
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5009
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Undefined identifier
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5018
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Unexpected quantifier
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            5013
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            VBArray expected
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
    <span sdata="link" xmlns:util="util"><a href="0343dc19-5f5e-4a4c-83da-630b4fbcb3b6.htm">JavaScript Syntax Errors</a></span>
  </div>
</div>

