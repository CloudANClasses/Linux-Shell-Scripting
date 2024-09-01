## Day 13 Shell Scripting Read Input from user &  Command line Arguments in shell script.

## Read Input from user in Shell Script

   - We can simply get user from the read command in BASH. It provides a lot of options with it more flexible usage.

## Read Basic Value from User

#!/bin/bash
read name
echo "Hello ${name}"

#!/bin/bash
read name
read age
echo "Hello ${name}, and your age is ${age}"

## Read With Prompt Message

#!/bin/bash
read -p "please enter your name " name
read -p "please enter your age " age
echo "Hello ${name}, and your age is ${age}"

## Read Secret Text With Prompt Message
#!/bin/bash
read -p "please enter your password " -s password
echo "your password is ${password}"

## lets create a file with below content and execute
#!/bin/bash
read -p "please enter your name " name
read -p "please enter your age " age
read -p "please enter your password " -s password
echo "Hello ${name}, and your age is ${age} and your password is ${password}"

## Output

  - ./readvariable.sh

## Command Line Arguments in Shell Script

  - Arguments are inputs that are necessary to process the flow. Instead of getting input from a shell script or assigning it to the program, the arguments are passed in the execution part.
 
## Positional Parameters
  - Command-line arguments are passed in the positonal way in the same way how they are given in the program
  - let's see it with an example
#!/bin/bash
name=${1}
age=${2}

echo "Hello my name is ${name} and my age is ${age}"
  - now let's give execute permission to this program and execute it.
  - chmod +x commandlineargs.sh
  - ./commandlineargs.sh 

## Suggestions: please use ${1} instead of $1.
#!/bin/bash
name=${1}
age=${2}
echo ${1}
echo ${2}
echo ${3}
echo ${4}
echo ${5}
echo ${6}

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day12/README.md) | [Next Day →](../Day14/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
