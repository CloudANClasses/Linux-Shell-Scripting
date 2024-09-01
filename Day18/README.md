## Day 18 Creating Local Variable & Return Status ($?) and test command

## Create Local Variable in Shell Script
  
  - All variables are global by default
  - Modifying a variable in a function changes it in the whole script. This could lead to issues.
  - local command can only be used within a function
  - It makes the variable name have a visible scope restricted to that function and its children only.
  - All function variables are local. This is a good programming practice.
  - example:
#!/bin/bash
packageName="nginx"
function install(){
    local myname="gaurav"
    echo "installing ${1}"
}

function configuration(){
    packageName="tomcat"
    echo "config ${1}"
}

echo "first ${packageName}"
echo "myname = ${myname}"
install "${packageName}"
echo "myname = ${myname}"
echo "second ${packageName}"
configuration "${packageName}"
echo "third ${packageName}"
  
  - output
  - ./variable-in-functions.sh

## Return Status ($?) and Test Command

## Exit Status
  - Every command returns on "exit status" 
  - A successful command returns a 0, While an unsuccessful one returns a non-zero value that usually can be interpreted as an error code.
  - Well-behaved unix Commands, programs and utilities return a 0 exit code upon successful completion through there are some exceptions.

┌──(test㉿-cloudan)-[~]
└─$ echo "cloudan"
cloudan

┌──(test㉿cloudan)-[~]
└─$ echo "echo: Command Not Found"
echo: Command Not Found

┌──(test㉿cloudan)-[~]
└─$ echo $?
0 # getting exit status is zero means last command executed successfully.

┌──(test㉿cloudan)-[~]
└─$ asdasd
asdasd: command not found

┌──(test㉿cloudan)-[~]
└─$ echo $?
127 # getting exit status as non zero means last command not exexuted successfully.

## Test Command
  - A test command is a command that is used to test the validity of a command.
  - It checks whether the command/expression is true or false.
  - It is used to check a number, string and file expression
  - It is used to check the type of file and the permissions related to a file.
  - Test command returns 0 as a successful exit status if the command/expression is true, and returns 1 if the command/expression is false.
  - Test is used by virtually every shell script written. It may not seem that way, because test is not often called directly. test is more frequently called as [. [ is a symbolic link to test, just to make shell programs more readable. It is also normally a shell builtin.

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day17/README.md) | [Next Day →](../Day19/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)

