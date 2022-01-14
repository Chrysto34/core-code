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

Started the Udacity Git course for version control.




      


