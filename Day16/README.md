## Day 16 Shell Scripting Set Default Value & Arthmetic Operations

  - If parameter is unset or null set default value
${parameter:-word}
  - If parameter is unset or null the expansion of word is substituted. Otherwise the value of parameter is substitued. 
  - If parameter is unset then set default value
${parameter-word}
  - If parameter is unset the expansion of word is substitued. Otherwise the value of parameter is substitued
  - let's create a script and execute it for practice purpose
#!/bin/bash

read -p " please enter your name " name

name=${name:-World}

echo "Hello ${name^}"

yourname=${unsetvariable-Manish}
echo $yourname

myname=""
mytestname=${myname:-kali}
echo ${mytestname}

   - Output:
   - ./default.sh
   - Check a Variable is set or not using below script
#!/bin/bash
# name="gaurav"
: ${1:?" please set variable values. "}
echo "i am here."
  - Output:
  - ./if-variable-not-set.sh

## Arithmetic Operations in Shell Script

  - We can do arithmetci operations in shell script in a several way (using let command, using expr command but we will recommend using brackets for that
  - Different ways to compute Arithmentic Operations in Bash
  - Using Double Parenthesis
  - Using let command
  - Using expr command

## Using Double Paraenthesis
  - Addition
Sum=$((20+2))
echo "Sum = ${Sum}" # output will be 22
  - Subtraction
sub=$((29-2))
echo "sub = ${sub}" # output will be 27
  - Multiplication
mul=$((20*4))
echo "Multiplication = ${mul}"  # output will be 80
  - Division
div=$((10/3))
echo "Division = ${div}" # output will be 3

  - Let's create shell script that will perform some arithmetic operations and decrement operations.
#!/bin/bash
a=5
b=6
echo "$((a+b))"
echo "$((a-b))"
echo "$((a*b))"
echo "$((a/b))" # 5/6
echo "$((a%b))"
echo "$((2**3))" # 2*2*2
((a++)) # a=a+1
echo $a
((a+=3)) # a=a+3
echo $a
  - Output
  - ./arth-operator.sh

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day15/README.md) | [Next Day →](../Day17/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
