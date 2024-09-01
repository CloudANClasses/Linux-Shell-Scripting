## Day 19 Shell Scripting if With command and If With Number

## If with command in Shell Script

  - This block will process if the exit status of command is zero or command execute successfully
if COMMAND
then
# if Block
# Your code here.
fi
  - Example: let's create a file with the name if-condition.sh with the below content
#!/bin/bash
if grep -i localhost /etc/hosts>/dev/null
then
  echo "Grep Command Executed successfully"
fi
echo "I am Here"

  - let's execute that file and see the output
┌──(test㉿cloudan)-[~/shellscript-youtube]
└─$ ./if-condition.sh
Grep Command Executed successfully
I am Here
  - now let's do somec changes in the if-condition.sh file and try to search for another word that is not in the /etc/hosts file.

#!/bin/bash
if grep -i gauravyt /etc/hosts>/dev/null
then
  echo "Grep Command Executed successfully"
fi
echo "I am Here"
  
  - now let's check the ouput
  - ./if-condition.sh

## If with Number in shell Script

  - we can use IF with the test command
  
#!/bin/bash

number=5

if test $number -eq 5
then
  echo "number is euqal to five"
fi
  - Instead of test command, we can use its alias that is [.
  - eq use for equals operations.
  - lt is used for less than.
  - gt is used for greater then
  - le is used for less than or equal.
  - ge is used for greater than or equal.
  - ne is used for not equal. 

#!/bin/bash
number=15
# eq is for equal, if number is equal to 5 then the below condition will become true.
if [ $number -eq 5 ]
then
  echo "number is eq 5"
fi

# lt is for less then, if number is less than 11 then the below condition will become true.
if [ $number -lt 10 ]
then
  echo "number is less than 10"
fi

# gt is for greater then, if number is greater than 4 then the below condition will become true.
if [ $number -gt 4 ]
then
  echo "number is greater then 4"
fi
# ge is for greater then or equal, if number is greater than or equal to 5 then the below condition will become true.
if [ $number -ge 5 ]
then
  echo "number is grater than or equal to 5"
fi
# le is for less then or equal, if number is less than or equal to 5 then the below condition will become true.
if [ $number -le 5 ]
then
  echo "number is less than or equal to 5"
fi
# ne is for not equal, is number is not euqal to 5 then below condition will become true.
if [ $number -ne 5 ]
then
  echo "number is not equal to five."
fi

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day18/README.md) | [Next Day →](../Day20/README.md)
 

 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
