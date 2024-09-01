## Day 22 While loop in Shell Script and Read File in Shell Script

## While loop in Shell Script

  - A While loop is a statement that iterates over a block of code till the condition specified is evaluated to true. We can use this statement or loop in our program when do not know many times the condition is going to evaluate to false before evaluating is true.
  - This repeats until the condition become false.
  - Syntax
  while [[ condition ]]
  do
    # statements
    # commands
  done

  while [ condition ]
  do
    # statements
    # commands
d  one

  - Example 1 
#!/bin/bash
  while [[ $answer != "yes" ]]
  do
    read -p "please enter yes " answer
  done
  - output ./while-loop.sh

## Read File in Shell Script
   
  - We can read a file with the help of read and while. The return code of read command is zero, unless the end of life is encountered

#!/bin/bash
  file_path="/etc/passwd"
  while read line
  do
    echo "$line"
    sleep 0.20
  done < $file_path
  
  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day21/README.md) | [Next Day →](../Day23/README.md)

 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
