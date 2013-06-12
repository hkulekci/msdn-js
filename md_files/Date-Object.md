---
title: Date Object (JavaScript)
isChild: false
---

## Date Object (JavaScript) {date_object_javascript_title}

### Introduction 

 Enables basic storage and retrieval of dates and times.

### Syntax 

```
dateObj = new Date() dateObj = new Date(dateVal ) dateObj = new Date(year , month , date [, hours [, minutes [, seconds [,ms ]]]])
```

#### Parameters 

<div id="sectionSection0" class="section" name="collapseableSection" style="" expanded="true">
  <dl class="authored">
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">dateObj</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The variable name to which the <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object is assigned.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">dateVal</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. If a numeric value, <span class="parameter" sdata="paramReference">dateVal</span> represents the number of milliseconds in Universal Coordinated Time between the specified date and
        midnight January 1, 1970. If a string, <span class="parameter" sdata="paramReference">dateVal</span> is parsed according to the rules in <span sdata="link">Formatting Date and Time Strings
        (Windows Scripting - JScript)</span>. The <span class="parameter" sdata="paramReference">dateVal</span> argument can also be a VT_DATE value as returned from some ActiveX objects.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">year</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The full year, for example, 1976 (and not 76).
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">month</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The month as an integer between 0 and 11 (January to December).
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">date</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Required. The date as an integer between 1 and 31.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">hours</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Must be supplied if <span class="parameter" sdata="paramReference">minutes</span> is supplied. An integer from 0 to 23 (midnight to 11pm) that specifies the hour.
      </p>
    </dd>
    <dt>
      minutes
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Must be supplied if <span class="parameter" sdata="paramReference">seconds</span> is supplied. An integer from 0 to 59 that specifies the minutes.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">seconds</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. Must be supplied if <span class="parameter" sdata="paramReference">milliseconds</span> is supplied. An integer from 0 to 59 that specifies the seconds.
      </p>
    </dd>
    <dt>
      <span class="parameter" sdata="paramReference" xmlns:util="util">ms</span>
    </dt>
    <dd>
      <p xmlns:util="util">
        Optional. An integer from 0 to 999 that specifies the milliseconds.
      </p>
    </dd>
  </dl>
</div>

#### Remarks 

<div id="languageReferenceRemarksSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    A <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object contains a number representing a particular instant in time to within a millisecond. If the value of an
    argument is greater than its range or is a negative number, other stored values are modified accordingly. For example, if you specify 150 seconds, JavaScript redefines that number as two minutes
    and 30 seconds.
  </p>
  <p xmlns:util="util">
    If the number is <b>NaN</b>, the object does not represent a specific instant of time. If you pass no parameters to the <span sdata="langKeyword" value="Date"><span class=
    "keyword">Date</span></span> object, it is initialized to the current time (UTC). A value must be given to the object before you can use it.
  </p>
  <p xmlns:util="util">
    The range of dates that can be represented in a <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object is approximately 285,616 years on either side of January 1,
    1970.
  </p>
  <p xmlns:util="util">
    See <span sdata="link">Date and Time Calculations (Windows Scripting - JScript)</span> for more information about how to use the <span sdata="langKeyword" value="Date"><span class=
    "keyword">Date</span></span> object and related methods.
  </p>
</div>

#### Example 

<p xmlns:util="util">
  The following example illustrates the use of the <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
</p>

```
var dateString = "Today's date is: "; var newDate = new Date(); // Get the month, day, and year. dateString += (newDate.getMonth() + 1) + "/"; dateString += newDate.getDate() + "/"; dateString +=
newDate.getFullYear(); document.write(dateString); // Output: Today's date is: &lt;date&gt;
```

#### Requirements 

<div id="requirementsTitleSection" class="section" name="collapseableSection" style="">
  <p xmlns:util="util">
    The <b>Date object</b> was introduced in Internet Explorer before Internet Explorer 6. Some members in the following lists were introduced in later versions. For more information, see
    <span sdata="link">Version Information</span> or the documentation for the individual members.
  </p>
</div>

#### Properties 

<div id="sectionSection1" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists properties of the <b>Date Object</b>.
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
    The following table lists functions of the <b>Date Object</b>.
  </p>
  <div class="caption"></div>
  <div class="tableSection">
    <table width="50%" cellspacing="2" cellpadding="5" frame="lhs">
      <tr>
        <th>
          <p xmlns:util="util">
            Functions
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
            Date.now Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the number of milliseconds between January 1, 1970, and the current date and time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Date.parse Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Parses a string containing a date, and returns the number of milliseconds between that date and midnight, January 1, 1970.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            Date.UTC Function
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the number of milliseconds between midnight, January 1, 1970 Universal Coordinated Time (UTC) (or GMT) and the supplied date.
          </p>
        </td>
      </tr>
    </table>
  </div>
</div>

#### Methods 

<div id="sectionSection3" class="section" name="collapseableSection" style="" expanded="true">
  <p xmlns:util="util">
    The following table lists methods of the <b>Date Object</b>.
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
            getDate Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the day-of-the-month value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getDay Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the day-of-the-week value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getFullYear Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the year value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getHours Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the hours value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getMilliseconds Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the milliseconds value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getMinutes Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the minutes value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getMonth Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the month value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getSeconds Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns seconds value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getTime Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the time value in a <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> Object as the number of milliseconds since midnight January 1, 1970.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getTimezoneOffset Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the difference in minutes between the time on the host computer and Universal Coordinated Time (UTC).
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getUTCDate Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the day-of-the-month value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getUTCDay Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the day-of-the-week value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getUTCFullYear Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the year value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getUTCHours Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the hours value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getUTCMilliseconds Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the milliseconds value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getUTCMinutes Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the minutes value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getUTCMonth Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the month value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getUTCSeconds Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the seconds value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getVarDate Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the VT_DATE value in a <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            getYear Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns the year value .
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            hasOwnProperty Method
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
            isPrototypeOf Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a Boolean value that indicates whether an object exists in another object's prototype chain.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            propertyIsEnumerable Method
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
            setDate Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the numeric day of the month using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setFullYear Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the year value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setHours Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the hours value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setMilliseconds Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the milliseconds value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setMinutes Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the minutes value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setMonth Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the month value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setSeconds Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the seconds value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setTime Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the date and time value in the <span sdata="langKeyword" value="Date"><span class="keyword">Date</span></span> object.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setUTCDate Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the numeric day of the month using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setUTCFullYear Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the year value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setUTCHours Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the hours value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setUTCMilliseconds Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the milliseconds value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setUTCMinutes Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the minutes value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setUTCMonth Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the month value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setUTCSeconds Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the seconds value using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            setYear Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Sets the year value using local time.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toDateString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a date as a string value.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toGMTString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a date converted to a string using Greenwich Mean Time (GMT).
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toISOString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a date as a string value in ISO format.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toJSON Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Used to transform data of an object type before the JSON serialization.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toLocaleDateString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a date as a string value appropriate to the host environment's current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toLocaleString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns an object converted to a string using the current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toLocaleTimeString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a time as a string value appropriate to the host environment's current locale.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toString Method
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
            toTimeString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a time as a string value.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            toUTCString Method
          </p>
        </td>
        <td>
          <p xmlns:util="util">
            Returns a date converted to a string using UTC.
          </p>
        </td>
      </tr>
      <tr>
        <td>
          <p xmlns:util="util">
            valueOf Method
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
    <span sdata="link" xmlns:util="util">Date and Time Calculations (Windows Scripting - JScript)</span>
  </div>
  <div class="seeAlsoStyle">
    <span sdata="link" xmlns:util="util">Formatting Date and Time Strings (Windows Scripting - JScript)</span>
  </div>
</div>

