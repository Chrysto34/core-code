                                                                   #Weekly Summary

<details><summary>Week 01</summary>
<p>

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

</p>
</details> 
 
<details><summary>Week 02</summary>
<p>

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

</p>
</details> 
 
<details><summary>Week 03</summary>
<p> 

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

--------------------------------------------------------------------------------------------------------------------------

Codewars Tuesday 01/25/2022

Codewar# 1

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
  return result.join('');
}















Codewar# 2

var reg = /\d/;

function order(words){
  // ...
  return words.split(' ').sort(comparator).join(' ');
  
}

function comparator(word, nextWord){
  return +word.match(reg) - +nextWord.match(reg)
}



Codewar# 3
function pigIt(str){
  //Code here
  str = str.trim().split(/\s{1,}/);
    return str.map(val => {
        if (/^[A-Za-z]+$/.test(val)) {
            return `${val.slice(1)}${val.slice(0, 1)}ay`;
        }
        return val;
    }).join(' ');
}

--------------------------------------------------------------------------------------------------------------------------------------------------------------


Codewar#1

function validParentheses(parens) {
  // your code here ..

  let a = 0;
  let o = 0;
  if(parens.length == 1 || parens[0] == ")") return false;
  for(let i = 0;i< parens.length; i++){
    
    if(parens[i] == '('){
     a++  
    }else if(parens[i] == ')'){
      a--
       if(a < 0){
   return false;}
    }
    
  }
  
  return a == 0;
}

Codewar#2

function toCamelCase(str){
var strArray;
  if (str.indexOf('-') !== -1){ //if delineated by -
    strArray = str.split('-');
  } else {
    strArray = str.split('_');  //if delineated by _
  }

  let fnlstr = strArray[0];
  for(let i = 1; i < strArray.length; i++){
    fnlstr += strArray[i].substr(0,1).toUpperCase()+strArray[i].slice(1);
  }
  
return fnlstr;  
}


Codewar#3

var uniqueInOrder=function(iterable){
  //your code here - remember iterable can be a string or an array
  const result = []
  
  for(let i = 0; i < iterable.length; i++){
    if(iterable[i] !== iterable[i + 1]){
      result.push(iterable[i])
    }
  }
  
  return result
}
------------------------------------------------------------------------------

01/27/2022

Kata# 1

function foldArray(array, runs) {
    let counterRuns = 0;
    let arrayPrimary = [...array];
    let result = [];
    while (counterRuns != runs) {
        result = arrayPrimary.map((value, index, arr) => {
            if (index != arr.length - 1) {
                value += arr[arr.length - 1];
            }
            arr.pop();
            return value;
        });
        arrayPrimary = result.filter((num) => num != undefined);
        counterRuns++;
    }
    return result.filter((num) => num != undefined);
    
    
Kata #2

var encryptThis = function(text) {
  // Implement me! :)
  let rr = text.split(' ');
  let output = [];
  
  rr.forEach(str => {
    if (str.length === 1) {
      output.push(str.charCodeAt(0));
    } 
    else {
      let tempStr = str.split('');
      tempStr[0] = str.charCodeAt(0);
      tempStr[1] = str[str.length - 1];
      tempStr[str.length - 1] = str[1];
      output.push(tempStr.join(''));
    }
  });
  
  return output.join(' ');
}


Kata #3

function list(names){
  //your code here
  const coma = ', ';
  const sign = ' & ';
  return names.reduce((pre, curr, indice)=> `${pre}${(indice==names.length-1 ? sign : coma)}${curr.name}`, '').slice(2).trim();
}



------------------------------------------------------------------------------------------------------------------------------------------------------

 </p>
</details> 
 
 
 <details><summary>Week 04</summary>
<p> 
 
                                                                                     Monday 01/31/2022

Watched videos.


                                                                                     Tuesday 02/01/2022


First type script Ex
export type User = {name: string; age: number; occupation: string};

export const users: User[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    }
];

export function logPerson(user: User) {
    console.log(` - ${user.name}, ${user.age}`);
}

console.log('Users:');
users.forEach(logPerson);

Second type script Ex

interface User {
    name: string;
    age: number;
    occupation: string;
}

interface Admin {
    name: string;
    age: number;
    role: string;
}

export type Person = User | Admin;

export const persons: Person[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Jane Doe',
        age: 32,
        role: 'Administrator'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    },
    {
        name: 'Bruce Willis',
        age: 64,
        role: 'World saver'
    }
];

export function logPerson(user: Person) {
    console.log(` - ${user.name}, ${user.age}`);
}

persons.forEach(logPerson);


                                                                               Third Typescript Excercise


interface User {
    name: string;
    age: number;
    occupation: string;
}

interface Admin {
    name: string;
    age: number;
    role: string;
}

export type Person = User | Admin;

export const persons: Person[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Jane Doe',
        age: 32,
        role: 'Administrator'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    },
    {
        name: 'Bruce Willis',
        age: 64,
        role: 'World saver'
    }
];

export function logPerson(person: Person) {
    let additionalInformation: string;
    if ('role' in person) {
        additionalInformation = person.role;
    } else {
        additionalInformation = person.occupation;
    }
    console.log(` - ${person.name}, ${person.age}, ${additionalInformation}`);
}

persons.forEach(logPerson);

// In case if you are stuck:
// https://www.typescriptlang.org/docs/handbook/advanced-types.html#using-the-in-operator


                                                                                     Kata#1 Tuesday Week 4

function findOdd(A) {
  //happy coding!

var count = 0;
  for(var i = 0; i<A.length; i++){
    for(var j = 0; j<A.length; j++){
      if(A[i] == A[j]){
        count++;
      }
    }
    if(count % 2 != 0 ){
      return A[i];
    }
  }
}



                                                                                    Kata#2 Tuesday Week 4

function spinWords(string){
  //TODO Have fun :)
    const stringArray = string.split(' ');
  let result = '';
  stringArray.map((str, i) => {
    if (str.length >= 5){
      stringArray[i] = str.split('').reverse().join('');
    } else {
      stringArray[i] = str;
    }
  result = stringArray.join(' ');
  });
return result;
}


                                                                                  Kata#1 Wednesday Week 4
                                                                                  
function arrayDiff(a, b) {
  if(b.length === 0)return a;
  return a.filter((num) => !b.includes(num));
}
                                                                                  
                                                                                  
                                                                                  
                                                                                  Kata#2 Wednesday Week 4

function createPhoneNumber(numbers){
  let first = "";
  let second = "";
  let third = "";
  for(let i = 0; i < numbers.length; i++){
    if(i < 3){
     first = first.concat(numbers[i].toString())
    } else if(i < 6){
     second = second.concat(numbers[i].toString())
    } else{
     third = third.concat(numbers[i].toString())
    }
  
  }
  return `(${first}) ${second}-${third}`
}



                                                                              Kata#1 Thursday Week 4


function isPangram(string){
    //...
    string = string.toLowerCase();
    
    for(let i = 97; i <= 122; i++) {
        if(string.indexOf(String.fromCharCode(i)) < 0) return false;
    }
    return true;
}


                                                                              Kata#2 Thursday Week 4

function findMissingLetter(array)
{
  var string = array.join("");
  for (var i = 0; i < string.length; i++) {
    if (string.charCodeAt(i + 1) - string.charCodeAt(i) != 1) {
      return String.fromCharCode(string.charCodeAt(i) + 1);
    }
  }
}


                                                                              Kata#3 Thursday Week 4
function findUniq(arr) {
  // do magic 
   arr.sort((a,b)=>a-b);
  return arr[0]==arr[1]?arr.pop():arr[0]
}












                                                                              Kata#4 Thursday Week 4

function revrot(str, sz) {
    // your code
  if(sz <= 0 || sz > str.length) return '';
  let regex = new RegExp(`(\\d){${sz}}`, 'g');
  console.log(str.match(regex));
  return str.match(regex).reduce((prev, curr) => {
    let mod = curr.split('').reduce((pre, current) => {
      return pre + Math.pow(current, 3);
    },0);
    return `${prev}${
      mod % 2 === 0? curr.split('').reverse().join('')
      : `${curr.substring(1, curr.length)}${curr[0]}`
    }`;
  }, '');
}


                                                                              Kata#5 Thursday Week 4


function find(rats) {
    // return number of poisoned bottle
  
  return rats.reduce((a,b) => a + Math.pow(2, b),0);
}

 
 
 </p>
</details>  
  
  
 
<details><summary>Week 05</summary>
<p>
  
  
                                                          Kata#2 Monday Week 5


export function squareSum(numbers: number[]): number {
    return numbers.reduce( (total, current) => total + Math.pow(current,2),0);
}

  
                                                          Kata#3 Monday Week 5

export class G964 {
        // your code
public static nbYear = (p0: number,percent: number,aug: number,p: number) => {
    let years = 0;
    while (p > p0) {
      p0 += p0 * (percent / 100) + aug;
      years++;
    }
    return years;
  };
    
}

                                                         Kata#4 Monday Week 5

export function accum(s: string): string {
   return s.split("").reduce((prev, curr, index, arr) => {
    return `${prev}${curr[0].toUpperCase()}${curr.repeat(index).toLowerCase()}${
      index < arr.length - 1 ? "-" : ""
    }`;
  }, "");
}


                                                          Kata#5 Monday Week 5  

export function warnTheSheep(queue: string[]): string {
 let wolf = queue.indexOf('wolf');
  return wolf === queue.length -1 ? 'Pls go away and stop eating my sheep' : `Oi! Sheep number ${queue.length - wolf -1}! You are about to be eaten by a wolf!`
}

  
                                                        Kata#1 Tuesday Week 5
                        
                        
                                                        Kata#2 Tuesday Week 5

    export class G964 {

    public static digPow = (n: number, p: number) => {
      let arr: number[] = String(n).split("").map((n)=>{
          return Number(n)
        })

      let arrRes = arr.reduce((acum, act, i, arr) => acum + (Math.pow(arr[i], p+i)), 0) / n;
      return (''+arrRes).includes('.') ? -1 : arrRes;
    }
}     
                        
</p>
</details> 
  
  
<details><summary>Week 06</summary>
<p>
  
  
  
</p>
</details> 
  

<details><summary>Week 07</summary>
<p>
  
  
  
</p>
</details> 
  
  
<details><summary>Week 08</summary>
<p>
  
  
  
</p>
</details> 

  
  
<details><summary>Week 09</summary>
<p>
  
  
  
</p>
</details> 

  
<details><summary>Week 10</summary>
<p>
  
  
  
</p>
</details> 
  

<details><summary>Week 11</summary>
<p>
  
  
  
</p>
</details> 
  
  
<details><summary>Week 12</summary>
<p>
  
  
  
</p>
</details> 
