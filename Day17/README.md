## Day 17 Shell Scripting Functions & Pass a Parameters to a Function

## Functions in Shell Script
  - Shell Functions are used to specify the blocks of commands that may be repeatedly invoked at different stages of execution.
  - The Main advantags of using unix shell Functions are to reuse the code and to the code in a modular eay
  - The Purpose of the function
  - Don't repeat itself
  - Write once use many times
  - Reduce the script lenght
  - A Single place to edit and troubleshoot
  - Easier to maintain
  - If you are repeating yourself use a function
  - Reusable code
  - Must define before use
  - Has parameters supports
  - The best practice is to put all the functions on top of the script

## How to create Function in Shell Script
  - In shell Script we can write functions in a varirty of different ways.
# type one.
function function_name(){
    # code goes here
}

# type two
function_name(){
    # code goes here
}
# method three
function function_name {
   # function code here.
}
  - Simply use the function name as a command to run a function
# invode the function
function_name
  - Example
#!/bin/bash

# funtions
function install(){
  #### installations code.
  echo "installationscode1"
}
configuration(){
  # configurations code
  echo "configcode1"
}

function deploy {
  # deploy code.
  echo "deploy code 1"
}
configuration
install
deploy
 
  - let's run the code and see the output
  - ./functions.sh

## Pass Parameters to a Function

  - We can define a function that will accept parameters while calling the function. These parameters would be represented by $1, $2 and so on.
  
## Functions can be Recursive
  - A Function may return a value in one of four different ways
  - Change the state of a variable or variables
  - Use thereturncommand to end the function, and return the supplied value to the calling section of the shell script
  - echo output to stdout, which will be caught by the caller just as expr $a + $b is caught
  - we can get the function name using FUNCNAME variable.

  - Here code can be anything you choose here, but obviously you should choose something that is meaningful or useful in the context of your script as a whole.
  - Example
#!/bin/bash

function install(){
  echo "executing ${FUNCNAME} - start"
  echo "installing ${1}"
  echo "executing ${FUNCNAME} - end"
}
function configuration(){
  echo "config ${1}"
  echo "${FUNCNAME}"
}

function deploy() {
  echo "deploying ${1}"
  echo "${FUNCNAME}"
}
install "nginx"
configuration "nginx"
deploy "webapplication"

  - Output
  - ./functions-args.sh

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day16/README.md) | [Next Day →](../Day18/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)

