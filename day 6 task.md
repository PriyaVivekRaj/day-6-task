
 ###GUVI: Zen Class — Part 3: Find the culprits and nail them — debugging javascript
##1. Fix the code to get the largest of three.


Answer:
=======



aa = (f,s,t) => {
  
    console.log(f,s,t);//1 2 3
    if(f>s &&f>t)
    console.log(f);
    else if(s>f && s>t)
    console.log(s);
    else
    console.log(t);//3
   }
   aa(1,2,3);
-----------------------------------------------------------------------------------------------------------------------------------------------
###2. Fix the code to Sum of the digits present in the number
================================================================


Answer:
==========
let n = [1,2,3];
console.log(add(n));//6
function add(n)
{
let sum = 0;
for(var i=0;i<n.length;i++){
 sum+=n[i]
 }
 return sum;
}
------------------------------------------------------------------------------------------------------------------------------------------------

###3. Fix the code to Sum of all numbers using IIFE function
===============================================================


Answer:
=======
const arr = [9,8,5,6,4,3,2,1];
(function() {
 let sum = 0;
 for (var i = 0; i < arr.length; i++)
 sum += arr[i];
 
 console.log(sum);
 
})();
------------------------------------------------------------------------------------------------------------------------------------------------

###4. Fix the code to gen Title caps.
=====================================

Answer:
========

var arro = ['guvi', 'geek', 'zen', 'fullstack'];
var ano = function() {
 for (var i = 0; i <arro.length; i++) {
 console.log(arro[i][0].toUpperCase() + arro[i].substr(1));
 }
}
ano();
--------------------------------------------------------------------------------------------------------------------------------------------------

###6. Fix the code to sum the number in that array
================================================

answer:
=======
const num = [10, 20, 30, 40,50,60,70,80,90,100] 
var sum = (a, b) =>
 a + b
 sum = num.reduce(sum)
console.log(sum);
--------------------------------------------------------------------------------------------------------------------------------------------------
###7. Fix the code to rotate an array by k times and return rotated array using IIFE function
==========================

 Answer:
=========
 var arr = [1, 2, 3, 6, 8, 6, 1, 9, 10, 12, 13];
var k = 3;
k = arr.length % k;
(function() {
 // arr = [];
 out = arr.slice(k + 1, arr.length);
 var count = out.length;
 for (var i = 0; i < k + 1; i++) {
 out[count] = arr[i];
 count += 1;
 }
 console.log(out);})();


-----------------------------------------------------------------------------------------------------------------------------------------------
###8. Fix the code to gen Title caps.
==================================


Answer:
========
var arr = ['guvi', 'geek', 'zen', 'fullstack'];
(function() {
for (var i = 0; i < arr.length; i++) {
console.log(arr[i][0].toUpperCase() + arr[i].substr(1));
}
})();

--------------------------------------------------------------------------------------------------------------------------------------------------



###Answer:
=======
var arr = [1, 2, 3, 5, 7, 79, 7, 2, 6, 9, 4];
(function() {
 for (var i = 0; i < arr.length; i++) 
 if (arr[i] % 2 != 0) 
 console.log(arr[i]);
 
})();



------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
###10. Fix the code to reverse.
============================


Answer:
=======
(function(str){
    str1 = str.split('').reverse().join('');
    console.log(str1); 
   })('abcd')
   
----------------------------------------------------------------------------------------------------------------------------------------------------------
###11. Fix the code to remove duplicates.
======================================

    
Answer:
======= 
var res = function(arr){
    for(var i=0; i < arr.length; i++){
    var newArr = [];
    if(newArr.indexOf(arr[i]) == -1) {
    newArr.push(arr[i]);
    } }
    console.log(newArr)
   }
   res(['guvi','geek','guvi','duplicate','geeK'])   
----------------------------------------------------------------------------------------------------------------------------------------------------
###12. Fix the code to give the below output:
==========================================
Expected Output:
================


Answer:
=======
var array =[[['firstname','vasanth'],['lastname','Raje'],['age',24],['role','JSWizard']],[['firstname','Sri'],['lastname','Devi'],['age',28],['role', 'Coder']]];
var final=[]
while(array.length!=0)
{
 var outer_remove = array.shift();
 var new_object=[];
 while(outer_remove.length!=0)
 {
 var inner_remove = outer_remove.shift()
 var key = inner_remove[0]
 var value =inner_remove[1]
 new_object[key]=value
 }
 final.push(new_object)
}
console.log(final);

----------------------------------------------------------------------------------------------------------------------------------------------------------

14. Fix the code to give the below output:
==========================================
Swap the odd and even digits
=============================

Answer:
=======
var aa = data=>{
 var a=data;
for(var i=0;i<a.length-1;i++){
 var l='';
 var s=a[i+1]
 var b=a[i]
 l+=s
 l+=b
 i=i+1
}
if((a.length%2)!=0){
 l+=a[a.length-1]
}
console.log(l);
}
aa('1234');

--------------------------------------------------------------------------------------------------------------------------------------------------
###GUVI: Zen Class — Part 1: Find the culprits and nail them — debugging javascript
Once you are familiar with basic syntax you can reinforce your understanding by solving these simple snippets

###Find the culprit


###Answer:

!DOCTYPE html>
<!DOCTYPE html>
<html>
<body>
 <script>
 alert("I\'m JavaScript!");
 </script>
 Whats the error in this ?
</body>
</html>
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Find the culprit and invoke the alert


Answer:
<!DOCTYPE html>
<html>
<body>
 Answer:   
 <script src="script.js"></script>
</body>
    </html>

scripts.js:
alert(" I'\m invoked! ");

— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Explain the below how it works


Answer:
    <!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
    </html>


    script.js 
alert("I'm JavaScript!");
alert('Hello'); 
alert(`Wor
 ld`);
alert(3 +
1
+ 2); 

— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the below to alert Guvi geek


Answer:

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>

script.js:

let admin=9, fname=10.5; 
fname = "Guvi";
lname = "geek"//using nothing declaration.
admin = fname+lname;
alert( admin );// Guvi geek
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the below to alert hello Guvi geek

Answer:

< !DOCTYPE html >
<html>
<body>
 <script src="script.js"></script>
</body>
</html>


let fname=10.5; 
fname = "Guvi";
lname = "geek";
let name = fname+lname;
alert(`hello ${name}`);
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the below to alert sum of two numbers

Answer:

let a = parseInt(prompt("First Number?"));
let b = parseInt(prompt("Second Number"));
alert(a+b);
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the below to alert sum of two numbers

Answer:
=======

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
    </html>
    script.js
    let a = parseInt(prompt("First number?"));
let b = parseInt(prompt("Second number?"));
alert(a + b);
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###If you run the below scritpt you will get “Code is Blasted”

Explain Why the Code is blasted and how to diffuse it and get “Diffused”.


Answer:

<!DOCTYPE html>
<html>
<body>
 <script src=”script.js”></script>
</body>
</html>

// script.js

var a = "2" > "12";//true
//Don't touch below this
if (a) {
  console.log("Code is Blasted")// type of a is boolean the value of a is true so we get code is blasted
}
else
{
  console.log("Diffused") 
}


var a = "2" < "12";//false
if (a) {
  console.log("Code is Blasted")
}
else
{
  console.log("Diffused")/// type of a is boolean the value of a is false so we get diffused 
}
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###How to get the success in console.

Answer:
<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>
const a = prompt("Enter a number?");
//Don't modify any code below this
if (a) {
 console.log( 'OMG it works for any number inc 0' );
}
else
{
 console.log( "Success" );
}
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###How to get the correct score in console.

Answer:

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>
script.js

const value = parseInt(prompt('How many runs you scored in this ball'));
if (value === 4) 
      console.log("You hit a Four");
 else if (value === 6) 
      console.log("You hit a Six");
 else 
      console.log("I couldn't figure out");

— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the code to welcome the Employee

fix.html

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>
script.js

let login = 'Employee';
let message = (login == 'Employee') ? (login == 'Director') ? 'Greetings' :
  (login == '') ? 'No login' :  'Hello': '0' ;
console.log(message);
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the code to welcome the boss

Answer:

  <!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>

let message;
if (null || 2 || undefined )
{
  message = "welcome boss";//in let redeclaration is not possible
}
else
{
  message = "Go away";
}
  console.log(message);
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the code to welcome the boss


Answer:

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>

script.js

  let message;
let lock = " ";
//Dont change any code below this 
if (null || lock || undefined )
{
  message = "Go away";
}
else
{
 message = "welcome";
}
  console.log(message);
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the code to welcome the boss

Answer:
<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>

script:

let message;
let lock = " ";
//Dont change any code below this
if (lock && " " || undefined )
{
  message = "Go away";
}
else
{
 message = "welcome";
}
console.log(message);
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Change the code to print


Answer:

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>
script.js

var i = 3;
while (i) 
  console.log( --i );//2 1 0


— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Change the code to print even numbers

Answer:

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>
script.js


for (var num = 2; num <= 20; num += 1) {
    console.log(num)
  }
— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Change the code to print all the gifts

Answer:

<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>
let gifts = ["teddy bear", "drone", "doll"];
for (let i = 0; i < 3; i++) {
  console.log(`Wrapped ${gifts[i]} and added a bow!`);
}


— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Fix the code to disarm the bomb.

Answer:
<!DOCTYPE html>
<html>
<body>
 <script src="script.js"></script>
</body>
</html>


let countdown = 100;
while (countdown > 0) {
  countdown--;
  if(countdown == 0)
  {
   console.log("bomb triggered");
  }
}

— — — — — — — — — — — — — — — — — — — — — — — — — — — — — — -

###Whats the msg printed and why?

Answer:

var lemein = "0";
var lemeout = 0;
var msg = "";
if (lemein) {
 msg += "hi";
 }
if (lemeout) {
 msg += "Hello";
}
console.log(msg);//hi
------------------------------------------------------------------
###Whats the msg printed and why? Guess you answer before running it.


Answer:

var lemein = "0";
var lemeout = 0;
var msg = "";
if (lemein) {
 msg += " hi";
 }
if (lemeout) {
 msg += "Hello";
}
console.log(msg);//hi
===========================================================================================================================================

###Write a code to print the numbers in the array

Answer:
var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var new_string = "";
 
for (var i = 0; i < numsArr.length; i++) {
 new_string += numsArr[i] 
}
console.log(new_string);
==========================================================================
###Write a code to print the numbers in the array


Answer:
=======

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var new_string ="" ;
 
for (var i = 0; i < numsArr.length; i++) {
  if(i==0)
   new_string = numsArr[i];
 else
 new_string +=  "," + numsArr[i] ;
}
console.log(new_string);

================================================================================================================
###Write a code to print from last to first with spaces (Make sure there is no space after the last element 1)


Answer:
=======

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var new_string = "";
 
for (var i = 10; i >= 0; i --) {
  if(i==0)
  new_string += numsArr[i];
    else 
 new_string +=  numsArr[i] + " " ;


====================================================================================================================
###Write a code to replace the array value — If the number is even, replace it with ‘even’.

Output:[ 1, “even”, 3, “even”, 5, “even”, 7, “even”, 9, “even”, … ]


Answer:
=======
var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
for (var i = 0; i <=10; i++) {
 if(numsArr[i] %2 == 0 )
 {
 numsArr[i] = "even";
 }
}
console.log(numsArr);
=======================================================================================================================
###Write a code to replace the array value — If the index is even, replace it with ‘even’.

Output: [ “even”, 2, “even”, 4, “even”, 6, “even”, 8, “even”, 10, … ]

Answer:
==========
var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
for (var i = 0; i <=10; i++) {
 if(numsArr[i] %2 != 0 )
 {
 numsArr[i] = "even";
 }
}
console.log(numsArr);
========================================================================================================================
###Write a code to add all the numbers in the array

Output: 66

Answer:
var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];var sum=0;
for (var i = 0; i <=10; i++) {
 
 sum += numsArr[i]
}
console.log(sum);
==========================================================================================================================
Write a code to add the even numbers only
Output: 30

Answer:
var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var sum=0;
for (var i = 0; i <10; i++) {
 if(numsArr[i]%2==0)
 sum += numsArr[i]
}
console.log(sum);
===============================================================================================================================
Write a code to add the even numbers and subract the odd numbers
Output: 94

Answer:

var numsArr = [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11];
var sum=0;
for (var i = 0; i <=10; i++) {
 if(numsArr[i]%2!=0)
 
 sum += numsArr[i];
 
 else
 
 sum -= numsArr[i];
 
}
console.log(sum);
==================================================================================================================================
Write a code to print inner arrays
Answer:

var numsArr = [[1, 2, 3, 4, 5],[ 6, 7, 8, 9, 10, 11]];
for (var i = 0; i < numsArr.length; i++) 
{
 console.log( numsArr[i]);
}

===========================================================================================================================================
Write a code to print elements in the inner arrays

Answer:

var numsArr = [[1, 2, 3, 4, 5],[ 6, 7, 8, 9, 10, 11]];
var str_all="";
for (var i = 0; i < numsArr.length; i++) {
 var inner_array = numsArr[i];
 for(var j = 0 ; j < inner_array.length;j++ )
     str_all +=inner_array[j]
}
console.log(str_all);
===========================================================================================================================================
Write a code to replace the array value — If the index is even, replace it with ‘even’.

Output: [ [“even”, 2, “even”, 4, “even”], [6, “even”, 8, “even”, 10, …] ]


Answer:

var numsArr = [[1, 2, 3, 4, 5],[ 6, 7, 8, 9, 10, 11]];
var str_all=[];
for (var i = 0; i < numsArr.length; i++) {
 var inner_array = numsArr[i];
 for(var j = 0 ; j < inner_array.length;j++ ) {
      if(inner_array[j] %2 == 0 )
      {
         
         str_all[j] = inner_array[j];
       } else {
         str_all[j] = 'even';
       }
 }
 numsArr[i] = str_all;
 str_all =[];
}
console.log(numsArr);

===========================================================================================================================================
Write a code to print elements in the inner arrays in reverse
Output: 11 10 9 8 7 6 5 4 3 2 1

Answer:
=======
var numsArr = [[1, 2, 3, 4, 5],[ 6, 7, 8, 9, 10, 11]];
var str_all='';
for (var i = numsArr.length-1; i >= 0 ; i--) {
 var inner_array = numsArr[i];
 
 for(var j = inner_array.length-1; j >= 0 ;j-- ) {
    
     str_all += inner_array[j] + ' ';
  
}
}
console.log(str_all);




===========================================================================================================================================










