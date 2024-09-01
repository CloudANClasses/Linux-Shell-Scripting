## Day 21 If-Else in ShellScript and Elif in ShellScript

  - If the specified condition is not true in the if part then the else part will be executed
  - Syntax
  - if [ expression ]
  - then
   statement1
  - else
   statement2
  - fi
  - Example
#!/bin/bash
  - name=""
  - othername="saurav sharma"

  - if [[ -n ${name} ]]
  - then
    echo "length of string is non zero"
  - else
    echo "length of string is zero"
  - fi

  - if [[ -z ${name} ]]
  - then
    echo "length of string is zero -two"
  - else
    echo "length of string is non zero. = two"
  - fi

  - if [[ ${name} == ${othername} ]]
  - then
    echo "both string are equals - three"
  - else
    echo "both string are not equals. - three"
  - fi

  - if [[ ${name} != ${othername} ]]
  - then
    echo "both string are not equals -four"
  - else
    echo "both strings are equals -four"
  - fi

  - echo "I am Here"

  - Output
  - ./if-else.sh

## Elif in Shell Script

  - if..elif..else..fi statement (Else if ladder)
  - To use multiple conditions in one if-else block, then elif keyword is used in shell. If the expression1 is true then it executes statements 1 and 2, and this process continues.If none of the conditions is true then it processes else part.

  - Syntax
  - if [ expression1 ]
  - then
   statement1
   statement2
   .
   .
  - elif [ expression2 ]
  - then
   statement3
   statement4
   .
   .
  - else
   statement5
  - fi

  - Example:
#!/bin/bash
  - number=4

  - if [[ ${number} -eq 10 ]]
  - then
  -   echo "number is 10"
  - elif [[ ${number} -lt 10 ]]
  - then
  echo "number is less then 10"
  - elif [[ ${number} -lt 5 ]]
  - then
  echo "number is less then 5"
  - else
  echo "number is grater then 10"
  - fi
  - Output
  - ./elif.sh


  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day20/README.md) | [Next Day →](../Day21/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
