# Strings
Strings are a type of data in javascript where textual data wrapped in quotes.  
#### Example: `"Javascript"`  
  

## 🛠️ String methods
Strings have different built-in methods where we can manipulate text in one way or another.  
Suppose str = "Javascript" is a string variable, to access string methods, you need to add " . " as a suffix to the variable. `str.method(args)`  

<table>
  <tr>
    <td><b>returnType method(parameterType)<b/></td>
    <td><b>Description<b/></td>
    <td><b>Example<b/></td>
    <td><b>Extra<b/></td>
  </tr>
  <tr>
    <td>char charAt(int)</td>
    <td>returns the character at index specified</td>
    <td>str.charAt(0) = "J"</td>
    <td>str.charAt(100) = `undefined` </td>
  </tr>
    <tr>
    <td>int indexOf(char)</td>
    <td>returns the first index of specified character in the string</td>
    <td>str.indexOf("a") = 1</td>
    <td>str.indexOf("H") =  `undefined`, str.indexOf("va") = str.indexOf("v") </td>
  </tr>
    <tr>
    <td>int lastIndexOf(char)</td>
    <td>returns the last index of specified character in the string</td>
    <td>str.lastIndexOf("a") = 3</td>
    <td>str.lastIndexOf("H") =  `undefined`, str.indexOf("va") = str.lastIndexOf("v") </td>
    <tr>
    <td>string trim(string)</td>
    <td>trims all the spaces in both sides of the string</td>
    <td>str.trim(" Bro Code ") = "Bro Code"</td>
    <td>spaces present in between the characters of the string are not removed, just the ones in the sides are trimmed</td>
  </tr>
    <tr>
    <td>string toUpperCase(string)</td>
    <td>covert all the characters to uppercase</td>
    <td>str.toUpperCase() = "JAVASCRIPT"</td>
    <td></td>
  </tr>
    <tr>
    <td>string toLowerCase(string)</td>
    <td>covert all the characters to lowercase</td>
    <td>str.toLowerCase = "javascript"</td>
    <td></td>
  </tr>
    <tr>
    <td>string repeat(int)</td>
    <td>repeats the string specific times</td>
    <td>str.repeat(2) = "JavascriptJavascript"</td>
    <td>str.repeat(-8) = RangeError</td>
  </tr>
    <tr>
    <td>bool startsWith(char)</td>
    <td>returns true if strings starts with char</td>
    <td>str.startsWith("Java") = true</td>
    <td>str.startsWith("") = true</td>
    </tr>
    <tr>
    <td>bool endsWith(char)</td>
    <td>returns true if string end with char</td>
    <td>str.endsWith("script") = true</td>
    <td>str.endsWith("") = true</td>
    </tr>
    <tr>
    <td>bool includes(char)</td>
    <td>returns true if char is present in string</td>
    <td>str.includes("J") = true</td>
    <td>str.includes("Javo") = false bcoz all characters are considered to be in a series</td>
    </tr>
    <tr>
    <td>string replaceAll(char1,char2)</td>
    <td>replaces all the appearances of char1 with char2</td>
    <td>str.replaceAll("a","o") = "Jovoscript"</td>
    <td>if char1 is not present in str the no changes is applied</td>
    </tr>
    <tr>
    <td>string padStart(int,char)</td>
    <td>pad the string with char from the start until length is achieved</td>
    <td>str.padStart(15,"o") = "oooooJavascript"</td>
    <td>if value less than the length of the string is passed then only the string will be returned</td>
    </tr>
    <tr>
    <td>string padEnd(int,char)</td>
    <td>pad the string with char from the end until length is achieved</td>
    <td>str.padEnd(15,"o") = "Javascriptooooo"</td>
    <td>if value less than the length of the string is passed then only the string will be returned</td>
  </tr>
  <tr>
    <td><b>int length<b/></td>
    <td><b>returns the length of the string<b/></td>
    <td><b>str.length = 10<b/></td>
    <td><b><b/></td>
  </tr>
</table>



