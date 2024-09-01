## Day 12 Shell Scripting User Define Variables, System Variable.

## User Define Variables
  - A variable is a character string to which we assign a value
  - A variable is nothing more than a pointer to the actual data. The shell enables you to create, assignn,selete variables.

## Rules
  - Then name of a variable can contain only letters (a to z or A to Z), numbers (0 to 9) or the inderscore character(_).
  - Variables names cannot be reserved words.
  - Variable name cannot have whitespace in between.
  - The variable name cannot have special characters.
  - The first character of the variable name cannot be a number.
  - The following examples are valid variable names.

## Defining Variables
  - Variables are defined as follows
  - variable_name=variable_value
  - For Example
  - MY_MESSAGE="Hello World"
  - Write a code
  - Now lets run the above code

## System Variable in Shell Script
  - Below are some of the most common environment variables:
  - USER - The current logged in user.
  - HOME - The home directory of the current user.
  - EDITOR - The default file editor to be used. This is the editor that will be used in your terminal
  - SHELL - The path of the current user's shell, such as bash or zsh.
  - LOGNAME - The name of the current user.
  - PATH - A list of directories to be searched when executing commands. When you run a command the system will search those directories in this order adn use the first found executable.
  - LANG - The current locales settings. 
  - TERM - The current terminal emulation.

  - #!/bin/bash
# System define variables.

 - echo ${SHELL}
 - echo ${HOME} # will show the home directory of current user
 - echo ${OSTYPE} # type type of operating system.
 - echo $PATH # A list of directories to be searched when executing commands.
 - echo ${$} # process id
 - echo ${PPID} # parent process id

 - echo $PWD # present working directory
 - echo $HOSTNAME # hostname of machine.
 - echo $UID # user id
 - # UID="5000"
 - echo $UID
 - sleep 5
 - echo ${SECONDS}

  - now let's run the above shell script and see the output.
  - ./variable.sh

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day11/README.md) | [Next Day →](../Day13/README.md)


- All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
