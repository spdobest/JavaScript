# JavaScript
Javascript documentation and programs  
  
## Introduction to javascript   

* JavaScript is a programming language, which is used to create functionality in the web page
Functionality means, receiving inputs from the user and providing output to the user"  
  
* It can perform tasks such as calculations, decision making, repetitive tasks, dynamically displaying
the output, reading inputs from the user dynamically, updating content on the web page based on
the inputs, interacting with server, validations etc.  

* It's operators and control statements are similar to C Language 

* JavaScript is client-side (browser-side) language. That means it executes on the browser. It can also  be used in server by using Node JS.  

* JavaScript is a case sensitive language  

* It is Interpreter based language. That means the code will be converted to machine language line by line  
* It is developed by Netscape Corporation in 1996.  
* It is implementation of Ecmascript. Ecmascript is the specication of Javascript.  
* Initially it was called as Live Script before named as Javascript.  

## Syntax of Javascript  
<script type "text/javascript">  
// Your Javascript codes are here  
</script>  
  
** NOTE : You can write <script> </script> inside <head> or <body>, But its Recomended to write inside <body>  </body> . You can write multiple  <Script> </script>. **  
  
### console.log()  
console.log() is used to print message/log in the browser console.  
console.log("Message type here")  
  
### OPERATORS In JAVASCRIPT   
* Arithmatic Operator **( + , - , * , / , % )**  
* Assignment Operator **( = , += , -= , *= , /= , %= )**  
* Increment Decrement Operator **( ++ , -- )** 
* Logical Operator **( && , || , ! )**  
* Concat Operator **( + )**  

***ALL THE OPERATOR EXAMPLES ARE WRITTEN IN OPERATOR PACKAGE IN SOURCE CODE***  

### CONTROL STATEMENT  
* **IF ELSE**  
* **SWITCH STATEMENT**  
* **WHILE LOOP**  
* **DO WHILE LOOP**  
* **FOR LOOP**   
  
#### IF ELSE  
Its same as other programming language like java, python etc.  
type of If  
1. If  
2. if else    
3. else if  


           ```
            var name = document.getElementById('name').value;  
            var ageStr = document.getElementById('age').value;
            var age = parseInt(ageStr);

            if(age<=20){
                document.getElementById("details").innerHTML = name+" Have ENERGY AND TIME BUT NO MONEY";
            }
            else if(age>20 || age<40){
                document.getElementById("details").innerHTML = name+" Have ENERGY AND MONEY BUT NO TIME";
            }
            else{
                document.getElementById("details").innerHTML = name+" Have MONEY AND TIME BUT NO ENERGY";
            }```


