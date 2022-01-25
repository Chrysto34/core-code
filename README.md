# First month of the bootcamp 
Day1: A bit of history and reviewed the tools. will see what the future holds

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Day2: 
1. Intermidiate code for interpretation languages, or also called bytecode

2.  Java language is compiled or interpreted? 
Java can be considered both a compiled and an interpreted language because its source code is first compiled into a binary byte-code. This byte-code runs on the Java Virtual Machine (JVM), which is usually a software-based interpreter. The use of compiled byte-code allows the interpreter (the virtual machine) to be small and efficient (and nearly as fast as the CPU running native, compiled code). In addition, this byte-code gives Java its portability: it will run on any JVM that is correctly implemented, regardless of computer hardware or software configuration. Most Web browsers (such as Microsoft Internet Explorer or Netscape Communicator) contain a JVM to run Java applets.

3. totdlsrs = 700; Total amount of dollars
USD = (totdlrs * 7.85);

4. Pseudocode is a way for us to structure our idea in order to translate it better to the actual programming language.

5. It is helpful because it helps us draw the structure and picture how we want the program to work. It also helps us write the code.


6. The user will be prompted to enter the year that they were born, we'll call this variable A
- Variable A will save the value entered, for example 1997
- There will be another variable called B that will contain the current year.
- There will be a variable C that will be the result of deducting B-A.
- In this case for example it'll be C =  B-A, the result for this one would be 25.
- There will be a window that shows "Your age is " + C

7. Reviewed article from lucidchart

8. They help us represent how our code is organized, how it's executed and how the system is ornganized in a visual manner.

9.  Low level and high level languages

- High level are the ones that we can understand easily, they can be interpreted and compiled.
- Low level are the ones where it's easier for the computer to understand
- Compilado alto nivel, objeto bajo nivel y organizado ya es un objeto ejecutable
- Assembler lenguaje low level
 



---------------------------------------------------------------------------------------------------------



Day3 

1. #Learn about binary, decimal and hexadecimal numbers

Decimal has a base of 10 for example 25 is 2x10 + 5x1, in the ones digit we have a one and in the 10 digits we have a 5. 10 to the 0 is equal to one.
Binary is a base 2 number system.
Hexadecimal is base 16, however when the number goes after 9 we start with A, B, C, D, E, or F


2.Translate the year you where born to binary, decimal and hexadecimal
Decimal: 1995
Binary:  Done with the table of 2 to the power of 10. The result is 11111001011
Hex: Done with division by 16, the result is 7CB


3. Convert Hex = CAFE  to   Binary = 1100101011111110 Decimal =  51966

4. Use a Low-level language, for example MIPS aseembler, to do so, you will need to follow this guide. We recomend to check the guide first but also this presentation could be helpful.

.data
    message: .asciiz "\nHello, World!\n"
  .text
    main:
      li $v0, 4
      la $a0, message
      syscall

5. Base on the examples and the guide of the low-level language: 5.1 Create a program to add two numbers given by the user 5.2 Create a program that display your name



Program to add two numbers

.data
msg1: .asciiz "\nIngrese un numero: "
msg2: .asciiz "\nIngrese un segundo numero: "
result: .asciiz "\nEl resultado es: "

.text
li $v0,4
la $a0,msg1
syscall

li $v0,5
syscall
move $t1,$v0

li $v0,4
la $a0,msg2
syscall

li $v0,5
syscall
move $t2,$v0

Add $t3,$t1,$t2

li $v0,4
la $a0,result
syscall

li $v0,1
move $a0,$t3
syscall

li $v0,10
syscall

Program to print name.

 .data
    message: .asciiz "\nMy name is Chrystopper!\n"
  .text
    main:
      li $v0, 4
      la $a0, message
      syscall
--------------------------------------------------------------------------------------------------------------------------------------------------------------------

Day 4, 01/13/2022

1. Famous/Real world applications done with Javascript:

- Netflix
- Facebook
- Candy Crush

2. Started the Udacity Git course for version control.

----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Week 2

Day 1

Created code wars user 
https://www.codewars.com/users/Chrysto34

Watched video.

-------------------------------------------------------------------------------------------------------------------------------------------------------------------

Day 2

Attended class

Watched video on how to google terms easier.

Codewars Solutions

Number 1

function multiply(a, b){
return  a * b
}

#2

function uniTotal (string) {
let suma = 0;
    for(let i = 0; i < string.length; i++) {
        let char_code = string[i].charCodeAt(0);
        suma += char_code;
    }
    return suma;
}





#3 
function getChar(index){
let char = String.fromCharCode(c);
return char
}


#4

function addBinary(a,b) {
let num = a + b;
let bin = num.toString(2);
  return bin;
}

#5

function finalGrade (exam, projects) {
  let total = 0;
  if (exam > 90 || projects > 10 ){
     total = 100;
  }else if (exam > 75 && projects >= 5){
    total = 90;
  } else if (exam > 50 && projects >= 2){
    total = 75; 
  }else { 
     total = 0;
  }
  
  return  total;
}


Day #3 -- CodeWars

#1
function dutyFree(normPrice, discount, hol){

  let totalb = hol/[normPrice*(discount/100) ]
  return Math.floor(totalb)
}



#2

function twiceAsOld(dadYearsOld, sonYearsOld) {
  // your code here
  let doub = Math.abs(dadYearsOld - (sonYearsOld*2));
  return doub;
}


#3


function validSpacing(s) {
  // write your code here
  const reg = /(^\s|\s$|\s{2,})/;
  return !(reg.test(s));
}

Could be done with trim 
https://developer.mozilla.org/es/docs/Web/JavaScript/Reference/Global_Objects/String/Trim
Validate the original string with the one that has been trimmed
Using find


#4

function fakeBin(x){
  var newStr = "";
  for(var i=0;i<x.length;i++){
    if(Number(x[i])>=5){
      newStr += "1"
    }
    else{
      newStr += "0";
    }
  }
  return newStr;
}

-------------------------------------------------------------------------------------------------------------------------

Day 4

I am Chrystopper. I'm currently working for a BPO in the customer experience department, I’ve been part of that industry for almost 7 years. Also learning coding on my own and how to develop websites, I have experience with CSS, HTML, and a bit of javascript, from online courses. I want to become a web developer within this year and start working in this field since it’s always been one of my passions. I adapt easily to different scenarios and keep learning and think that tech is a great field.

Day 5

Test

---------------------------------------------------------------------------------------------------------------------------------------------------------

Day 1 - Week 03 - 01/24/2022

Solution to codewars #1
function likes(names) {
  // TODO
let b = names.length - 2;
if(names.length == []){
 return("no one likes this");
} else if (names.length == 1 ){
return( names[0] + ' likes this');  
} else if (names.length == 2 ){
return( names[0] + ' and ' + names[1] + ' like this');  
} else if (names.length == 3 ){
return( names[0] + ", " +  names[1] + ' and ' + names[2] + ' like this');  
} else if (names.length == 4 ){
return( names[0] + ", " +  names[1] + ' and' + ' 2 others like this');  
} else if (names.length > 4 ){
return( names[0] + ", " +  names[1] + ' and '+ b + ' others like this');  
} 
}

codewars#2

var countBits = function(n) {
  // Program Me
  let b = (n).toString(2);
  let f = 0;

console.log(b);

for (let i = 0; i < b.length; i++) {
  if(b[i] == 1){
      f++;
  }
}

return(f);

};






codewars#3

decodeMorse = function(morseCode){
  //your code here
  morseCode = morseCode.trim();
  let refinedData = morseCode.split('   ');
  let result = [];
  
  for (let i = 0; i < refinedData.length; i++) {
    let temp = refinedData[i].split(' ');
    for (let j = 0; j < temp.length; j++) {
      if (MORSE_CODE[temp[j]]) {
        result.push(MORSE_CODE[temp[j]]);
      }
    }
    
    if (i !== refinedData.length - 1) {
    result.push(' ');
    }
  }



