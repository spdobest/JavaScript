# JAVASCRIPT INTERVIEW QUESTIONS  
  
**1. What is JavaScript?**  
  
JavaScript is a client-side as well as server side scripting language that can be inserted into HTML pages and is understood by web browsers. JavaScript is also an Object based Programming language  
  
**2. Enumerate the differences between Java and JavaScript?**  
  
Java is a complete programming language. In contrast, JavaScript is a coded program that can be introduced to HTML pages. These two languages are not at all inter-dependent and are designed for the different intent. Java is an object - oriented programming (OOPS) or structured programming language like C++ or C whereas JavaScript is a client-side scripting language.
  
**3. What are JavaScript Data Types?**  
  
Following are the JavaScript Data types:  
***Number  
Undefined
Null
Boolean
String
Symbol
Number
Object***   
  
**4. What is the use of isNaN function?** 
  
isNan function returns true if the argument is not a number otherwise it is false.  
  
**5. Between JavaScript and an ASP script, which is faster?**  
  
JavaScript is faster. JavaScript is a client-side language and thus it does not need the assistance of the web server to execute. On the other hand, ASP is a server-side language and hence is always slower than JavaScript. Javascript now is also a server side language (nodejs).  
**6. What is negative infinity?**  
Negative Infinity is a number in JavaScript which can be derived by dividing negative number by zero.  
  
**7. Is it possible to break JavaScript Code into several lines?**  
Breaking within a string statement can be done by the use of a backslash, '\', at the end of the first line  
Example:  
document.write("This is \a program");  
And if you change to a new line when not within a string statement, then javaScript ignores break in line.  
Example:   
var x=1, y=2,  
z=  x+y;  
The above code is perfectly fine, though not advisable as it hampers debugging.  
  
**8. Write the code for adding new elements dynamically?**  
  
        ```  
        <html> 
        <head> 
        <title>t1</title> 
        <script type="text/javascript"> 
          function addNode() { var newP = document.createElement("p"); 
          var textNode = document.createTextNode(" This is a new text node"); 
          newP.appendChild(textNode); document.getElementById("firstP").appendChild(newP); } 
        </script> </head> 
        <body> <p id="firstP">firstP<p> </body> 
        </html>```  
          
**9.What are global variables? How are these variable declared and what are the problems associated with using them?**  
  
Global variables are those that are available throughout the length of the code, that is, these have no scope. The var keyword is used to declare a local variable or object. If the var keyword is omitted, a global variable is declared.  
  
Example:  
// Declare a global globalVariable = "Test";  
The problems that are faced by using global variables are the clash of variable names of local and global scope. Also, it is difficult to debug and test the code that relies on global variables.   
  
**10. What is the difference between ViewState and SessionState?**  
  
'ViewState' is specific to a page in a session.  
  
'SessionState' is specific to user specific data that can be accessed across all pages in the web application.  
  
**11. What is === operator?**  
  
=== is called as strict equality operator which returns true when the two operands are having the same value without any type conversion.  
  
**12. Explain how can you submit a form using JavaScript?**  
    
To submit a form using JavaScript use document.form[0].submit();  
document.form[0].submit();  
  
**13. How can the style/class of an element be changed?**   
  
It can be done in the following way: 
document.getElementById("myText").style.fontSize = "20?;  
or  
document.getElementById("myText").className = "anyclass";  
  
**14. Explain how to read and write a file using JavaScript?**  
  
There are two ways to read and write a file using JavaScript
  
Using JavaScript extensions  
Using a web page and Active X objects  
  
**15. Explain how to detect the operating system on the client machine?**  
  
In order to detect the operating system on the client machine, the navigator.platform string (property) should be used.  
  
**16. What is the function of delete operator?**  
  
The delete keyword is used to delete the property as well as its value.   
Example  
var student= {age:20, batch:"ABC"};  
delete student.age;  
  
**17. What is an undefined value in JavaScript?**  
  
Undefined value means the   
Variable used in the code doesn't exist  
Variable is not assigned to any value  
Property doesn't exist  
  
**18.What are all the types of Pop up boxes available in JavaScript?**  
  
***Alert  
Confirm and  
Prompt***  
  
**19.What is the use of Void(0)?**  
  
Void(0) is used to prevent the page from refreshing and parameter "zero" is passed while calling.  
Void(0) is used to call another method without refreshing the page.  
  
**20.Mention what is the disadvantage of using innerHTML in JavaScript?**  
  
If you use innerHTML in JavaScript the disadvantage is  
  
Content is replaced everywhere  
We cannot use like "appending to innerHTML"  
Even if you use +=like "innerHTML = innerHTML + 'html'" still the old content is replaced by html  
The entire innerHTML content is re-parsed and build into elements, therefore its much slower  
The innerHTML does not provide validation and therefore we can potentially insert valid and broken HTML in the document and break it  
  
**21.Which keywords are used to handle exceptions?**  

      ```  
      Try… Catch---finally is used to handle exceptions in the JavaScript

      Try{
        Code
      }
      Catch(exp){
        Code to throw an exception
      }
      Finally{
        Code runs either it finishes successfully or after catch
      }```
        
**22.Which keyword is used to print the text in the screen?***  
  
document.write("Welcome") is used to print the text – Welcome in the screen.  
  
**23.What is the use of blur function?**  
Blur function is used to remove the focus from the specified object.  

**24.What are the different types of errors in JavaScript?**  
   
There are three types of errors:  
  
**Load time errors:** Errors which come up when loading a web page like improper syntax errors are known as Load time errors and it generates the errors dynamically.  
**Run time errors:**  Errors that come due to misuse of the command inside the HTML language.  
**Logical Errors:** These are the errors that occur due to the bad logic performed on a function which is having different operation.  
   
**25. What is the 'Strict' mode in JavaScript and how can it be enabled?**  
  
Strict Mode adds certain compulsions to JavaScript. Under the strict mode, JavaScript shows errors for a piece of codes, which did not show an error before, but might be problematic and potentially unsafe. Strict mode also solves some mistakes that hamper the JavaScript engines to work efficiently.  
  
Strict mode can be enabled by adding the string literal "use strict" above the file. This can be illustrated by the given example:  
      ```
      function myfunction() {
          "use strict";
          var v = "This is a strict mode function";
      }```
          
**26.What is the way to get the status of a CheckBox?**  
  
The status can be acquired as follows -  
alert(document.getElementById('checkbox1').checked);  
If the CheckBox will be checked, this alert will return TRUE.  
  
**27.Explain window.onload and onDocumentReady?**  
  
The onload function is not run until all the information on the page is loaded. This leads to a substantial delay before any code is executed.  
   
onDocumentReady loads the code just after the DOM is loaded. This allows early manipulation of the code.

**28.How will you explain closures in JavaScript? When are they used?**
  
Closure is a locally declared variable related to a function which stays in memory when the function has returned.    
  
**29.How can a value be appended to an array?**  
 
A value can be appended to an array in the given manner -  
arr[arr.length] = value;  
  
**30.  What is the difference between .call() and .apply()?**  
  
The function .call() and .apply() are very similar in their usage except a little difference. .call() is used when the number of the function's arguments are known to the programmer, as they have to be mentioned as arguments in the call statement. On the other hand, .apply() is used when the number is not known. The function .apply() expects the argument to be an array.  
  
The basic difference between .call() and .apply() is in the way arguments are passed to the function.    

**31. Write the point of difference between web-garden and a web-farm?**  
  
Both web-garden and web-farm are web hosting systems. The only difference is that web-garden is a setup that includes many processors in a single server while web-farm is a larger setup that uses more than one server.  
 
**32.How are object properties assigned?**  
  
Assigning properties to objects is done in the same way as a value is assigned to a variable. For example, a form object's action value is assigned as 'submit' in the following manner - Document.form.action="submit"  

**33.What is the method for reading and writing a file in JavaScript?**  
  
This can be done by Using JavaScript extensions (runs from JavaScript Editor), example for opening of a file -  
fh = fopen(getScriptPath(), 0);  
**34.How are DOM utilized in JavaScript?**    
  
DOM stands for Document Object Model and is responsible for how various objects in a document interact with each other. DOM is required for developing web pages, which includes objects like paragraph, links, etc. These objects can be operated to include actions like add or delete. DOM is also required to add extra capabilities to a web page. On top of that, the use of API gives an advantage over other existing models.  

**35.How are event handlers utilized in JavaScript?**  
  
Events are the actions that result from activities, such as clicking a link or filling a form, by the user. An event handler is required to manage proper execution of all these events. Event handlers are an extra attribute of the object. This attribute includes event's name and the action taken if the event takes place.  

**36.Explain the role of deferred scripts in JavaScript?**  
  
By default, the parsing of the HTML code, during page loading, is paused until the script has not stopped executing. It means, if the server is slow or the script is particularly heavy, then the webpage is displayed with a delay. While using Deferred, scripts delays execution of the script till the time HTML parser is running. This reduces the loading time of web pages and they get displayed faster.  

**37.What are the various functional components in JavaScript?**  
  
The different functional components in JavaScript are-  
First-class functions: Functions in JavaScript are utilized as first class objects. This usually means that these functions can be passed as arguments to other functions, returned as values from other functions, assigned to variables or can also be stored in data structures.  
  
Nested functions: The functions, which are defined inside other functions, are called Nested functions. They are called 'everytime' the main function is invoked.  

**38.What are the decodeURI() and encodeURI()?**
  
EncodeURl() is used to convert URL into their hex coding. And DecodeURI() is used to convert the encoded URL back to normal.
          
          ```
          <script>
            var uri="my test.asp?name=ståle&car=saab";

            document.write(encodeURI(uri)+ "<br>");

            document.write(decodeURI(uri));
          </script> 
          ```  
**Output -** 

my%20test.asp?name=st%C3%A5le&car=saab

my test.asp?name=ståle&car=saab

**39.Why it is not advised to use innerHTML in JavaScript?**  
  
innerHTML content is refreshed every time and thus is slower. There is no scope for validation in innerHTML and, therefore, it is easier to insert rouge code in the document and, thus, make the web page unstable.  
  
**40.What does the following statement declares?**  
  
var myArray = [[[]]];  
It declares a three dimensional array.  

**41.How are JavaScript and ECMA Script related?**  

ECMA Script are like rules and guideline while Javascript is a scripting language used for web development.  
  
**42.What is namespacing in JavaScript and how is it used?**  
  
Namespacing is used for grouping the desired functions, variables etc. under a unique name. It is a name that has been attached to the desired functions, objects and properties. This improves modularity in the coding and enables code reuse.  
  
**43.How can JavaScript codes be hidden from old browsers that don't support JavaScript?**  
  
For hiding JavaScript codes from old browsers:  
  
Add "<!--" without the quotes in the code just after the <script> tag.  
  
Add "//-->" without the quotes in the code just before the <script> tag.  
  
Old browsers will now treat this JavaScript code as a long HTML comment. While, a browser that supports JavaScript, will take the "<!--" and "//-->" as one-line comments.  
  
**44.What are the advantages of using External JavaScript?**  
  
Using External JavaScript in our code has many advantages as stated below.  
***Separation of Code is done.***    
***Code Maintainability is Easy.***      
***Performance is better.***    
  
**45.What is the difference between test () and exec () methods?**  
  
Both test () and exec () are RegExp expression methods.  
  
Using test (), we will search a string for a given pattern, if it finds the matching text then it returns the Boolean value ‘true’ and else it returns ‘false’.  
  
But in exec (), we will search a string for a given pattern, if it finds the matching text then it returns the pattern itself and else it returns ‘null’ value.  

**46.What are the Advantages of JavaScript?**  
  
JavaScript Scripting language has many advantages as stated below.  
  
***Lightweight:*** JavaScript is easy to implement. It has small memory footprints.  
***Interpreted:*** It is an interpreted language. Instructions are executed directly.  
***Object-oriented:*** JavaScript is an object-oriented language.  
***First class functions:*** In JavaScript, a function can be used as a value.  
***Scripting Language:*** It’s a language in which instructions are written for a run-time environment.   
  
**47. What are the distinct types of Error Name Values?**  
  
There are 6 types of values in ‘Error Name’ Property.  
  
**Error**               	**Description**
***Range Error***   	  We will get this error if we use a number outside the range  
***Syntax Error***	    This error raises when we use the incorrect syntax.   
***Reference Error***	  This error is thrown if used an undeclared variable.  
***Eval Error***	      Thrown due to the error in eval(). New JavaScript version doesn’t have this error   
***Type Error***	      Value is outside the range of types used.  
***URI Error***         Due to the usage of illegal characters.  

**48.What is JavaScript Hoisting?**  
  
Using ‘JavaScript Hoisting’ method, when an interpreter runs the code, all the variables are hoisted to the top of the original /current scope. If you have a variable declared anywhere inside the JavaScript code then it is brought to the top.  
  
This method is only applicable for the declaration of a variable and is not applicable for initialization of a variable.   Functions are also hoisted to the top, whereas function explanations are not hoisted to the top.  
  
**49.What is the difference between ‘var’ and ‘let’ keyword?88**    
  
The Differences are as follows:  

***var*** keyword was introduced in JavaScript code from the beginning Stage itself.	
***let*** keyword is introduced in 2015 only.  
***Var*** keyword has function scope. 
The variable defined with ***var*** is available anywhere within the function.  
A variable declared with ***let*** keyword has a scope only with in that block. So, 
***let*** has a Block Scope.  
The variable declared with ***var*** be hoisted	The variable declared with ‘let’ be hoisted  
  
**50.What are all the best practices for writing JavaScript Code? How do you write better code?**  
  
This has many different answers. Some of the best ways are:  

1. Always initialize the variables before you use them.  
2. Always use === equals instead of ==.  
3. Wrapping code that could thrown errors at run time and feature-based code in try...catch block.  
4. Don’t pollute global scope and don’t use global variables.  
5. Always use "use strict";.  
6. Use lint tools to validate JavaScript code and avoid any potential risks.  
7. Wrap your code in an anonymous function or Immediately Invoked Function Expressions (IIFE), so that it will affect the global scope.  
8. Give clear name for variables and functions.  
9. Give comments wherever needed so that the other developer understands the code better.  
10. Place all your scripts at end.  
11. Reduce DOM manipulations and if you need to add large dom elements by script, use document.createDocumentFragment.    
  
**51. What is ECMAScript 6? What are the new features?**  
  
ECMAScript was created to standardize JavaScript. The latest standardized JavaScript version is called ECMAScript 6 also known as ECMAScript 2015.  
ES6 includes the following new features:  
**arrow function
Template strings
rest and spread operators
Symbols data type
Promises
generators**  

**52.What is Ajax?**  
  
AJAX stands for Asynchronous JavaScript And XML. AJAX’s most appealing characteristic is its “asynchronous” nature, which means it can communicate with the server, exchange data, and update the page without having to refresh the page. In a nutshell, it is the use of the XMLHttpRequest object to communicate with servers. It can send and receive information in various formats, including JSON, XML, HTML, and text files.  
The two major features of AJAX allow you to do the following:  
***Make requests to the server without reloading the page  
Receive and work with data from the server***   

**53. Difference between == and === ?**  
When we compare two variables of different type e.g. a boolean with a string or a number with String using == operator, it automatically converts one type into another and return value based upon content equality, while === operator is strict equality operator in Java, and only return true if both variable of same type and also contains same value. This will be much clear with following example of == and === operator in JavaScript :  

0==false   // true, because false is equivalent of 0  
0===false  // false, because both operands are of different type  
2=="2"     // true, auto type coercion, string converted into number  
2==="2"    // false, since both operands are not of same type  
  
**54. What exactly are the JavaScript cookies?**  
These are basically the test files have smaller size and are generally stored in a workstation. They get created automatically when a user opens a webpage. This is for the information they need to store. This could be details of the username and the information related to what they are interested in.   

**55. What exactly do you know about the variable typing in JavaScript?**  
It is basically an approach with the help of which it is possible for the developers to assign a number to any variable which can further be assigned to a string. It is also called a variable typing.  
  
**56. What are the scopes of a variable in JavaScript?**  
  
The scope of a variable is the region of your program in which it is defined. JavaScript variable will have only two scopes.
***• Global Variables*** − A global variable has global scope which means it is visible everywhere in your JavaScript code.
***• Local Variables*** − A local variable will be visible only within a function where it is defined. Function parameters are always local to that function.  

**57. What is the purpose of ‘This’ operator in JavaScript?**  
  
The JavaScript this keyword refers to the object it belongs to. This has different values depending on where it is used. In a method, this refers to the owner object and in a function, this refers to the global object.  
  
**58.What is Callback?**  
  
A callback is a plain JavaScript function passed to some method as an argument or option. It is a function that is to be executed after another function has finished executing, hence the name ‘call back‘. In JavaScript, functions are objects. Because of this, functions can take functions as arguments, and can be returned by other functions.  
  
**59.What are the variable naming conventions in JavaScript?**  
  
The following rules are to be followed while naming variables in JavaScript:  
  
*.You should not use any of the JavaScript reserved keyword as variable name. For example, break or boolean variable names are not valid.  
*.JavaScript variable names should not start with a numeral (0-9). They must begin with a letter or the underscore character. For example, 123name is an invalid variable name but _123name or name123 is a valid one.  
*. JavaScript variable names are case sensitive. For example, Test and test are two different variables.  

**60. How does TypeOf Operator work?**  
  
The typeof operator is used to get the data type of its operand. The operand can be either a literal or a data structure such as a variable, a function, or an object. It is a unary operator that is placed before its single operand, which can be of any type. Its value is a string indicating the data type of the operand.  
  
**61.How to create a cookie using JavaScript?**  
  
The simplest way to create a cookie is to assign a string value to the document.cookie object, which looks like this-  
  
***Syntax :
document.cookie = "key1 = value1; key2 = value2; expires = date";***  
  
**62.How to read a cookie using JavaScript?**  
  
Reading a cookie is just as simple as writing one, because the value of the document.cookie object is the cookie. So you can use this string whenever you want to access the cookie.  
  
The document.cookie string will keep a list of name = value pairs separated by semicolons, where name is the name of a cookie and value is its string value.  
You can use strings’ split() function to break the string into key and values.  

**63.How to delete a cookie using JavaScript?**  
  
If you want to delete a cookie so that subsequent attempts to read the cookie return nothing, you just need to set the expiration date to a time in the past. You should define the cookie path to ensure that you delete the right cookie. Some browsers will not let you delete a cookie if you don’t specify the path.  
  
Now let’s move on to the next section of JavaScript interview questions.  
  
**64.What is the difference between Attributes and Property?**  
  
***Attributes-***  provide more details on an element like id, type, value etc.  
  
***Property-***  is the value assigned to the property like type=”text”, value=’Name’ etc.  
  
**65.List out the different ways an HTML element can be accessed in a JavaScript code.**  
  
Here are the list of ways an HTML element can be accessed in a Javascript code:
(i) getElementById(‘idname’): Gets an element by its ID name
(ii) getElementsByClass(‘classname’): Gets all the elements that have the given classname.
(iii) getElementsByTagName(‘tagname’): Gets all the elements that have the given tag name.
(iv) querySelector(): This function takes css style selector and returns the first selected element.  
  
**66.In how many ways a JavaScript code can be involved in an HTML file?**  
  
There are 3 different ways in which a JavaScript code can be involved in an HTML file:  
  
***Inline
Internal
External***  
  
An inline function is a JavaScript function, which is assigned to a variable created at runtime. You can differentiate between Inline Functions and Anonymous since an inline function is assigned to a variable and can be easily reused. When you need a JavaScript for a function, you can either have the script integrated in the page you are working on, or you can have it placed in a separate file that you call, when needed. This is the difference between an internal script and an external script.  

**67.What are the ways to define a variable in JavaScript?**  
  
The three possible ways of defining a variable in JavaScript are:  
  
***Var –***The JavaScript variables statement is used to declare a variable and, optionally, we can initialize the value of that variable. Example: var a =10; Variable declarations are processed before the execution of the code.  
***Const –*** The idea of const functions is not allow them to modify the object on which they are called. When a function is declared as const, it can be called on any type of object.  
***Let –*** It is a signal that the variable may be reassigned, such as a counter in a loop, or a value swap in an algorithm. It also signals that the variable will be used only in the block it’s defined in.  
  
**68.What is a Typed language?**  
  
Typed Language is in which the values are associated with values and not with variables. It is of two types:

***Dynamically:*** in this, the variable can hold multiple types; like in JS a variable can take number, chars.  
***Statically:*** in this, the variable can hold only one type, like in Java a variable declared of string can take only set of characters and nothing else.  
  
**69. What is the difference between Local storage & Session storage?**   
  
***Local Storage –*** The data is not sent back to the server for every HTTP request (HTML, images, JavaScript, CSS, etc) – reducing the amount of traffic between client and server. It will stay until it is manually cleared through settings or program.  
  
***Session Storage –*** It is similar to local storage; the only difference is while data stored in local storage has no expiration time, data stored in session storage gets cleared when the page session ends. Session Storage will leave when the browser is closed.  
  
**70. What is the difference between window & document in JavaScript?**  
  
***Window***	
***JavaScript window*** is a global object which holds variables, functions, history, location.	
***Document-*** The document also comes under the window and can be considered as the property of the window.  
  
**71.What is the difference between innerHTML & innerText?**  
  
***innerHTML –*** It will process an HTML tag if found in a string  
  
***innerText –*** It will not process an HTML tag if found in a string   

**WHat is the use of close function**  
  
In Javascript close() method is used to close the current window. You must write window.close() to ensure that this command is associated with a window object and not some other JavaScript object.  
  
  





  







  
