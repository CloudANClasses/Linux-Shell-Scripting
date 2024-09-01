## Day 11 Shell Built-In Commands, Print Hello World in different color, Comments and Escape.

## Shell Built-in
  - Shell Built-in does not request another program to run a process because it is a shell built-in. so use shell built-in if it is available

  - A built in command is simply a command that the shell carries out itself, instead of interpreting it is a request. it is a request you to load and run some other program.

## Keywords
  - Keywords are the words whose meaning has already been explained to the shell. the keyword cannot be used as variable names because it is a reserved word containing reserved meanings.

## Sequece
  - When you run a command bash will search a function with the same name if the function with the same name is not present then bash will search it in builtins. if built is also not available then it will search the command at PATH locations.
  - uptime
  - type -a uptime
  - type -a echo
  - type -a pwd
  - type -a if
  - echo $PATH

## Print Hello World in Different Color

## echo command
   - All the parameters to the echo command are printed on the screen. with the help of echo command, we can print the text in different color
   - #!/bin/bash
   - echo this is gaurav sharma
   - echo "this is our first Shell Script"
   - now lets run the above script
   - ./echo.sh

## Comments and Escape
   - Comments are the useful information that the developers provide to make the reader understand the source code.
   - There are two types of comments
   - Single-line comment
   - Multo-line comment

## Single-line comments
   - A Single line comment starts with a hashtag symbol with no spaces (#) and lasts till the end of the line. If the comment exceeds one line the put a hashtag on the next line and continue the comment.
   - Syntax
   - #!/bin/bash
   - # this is a comment

## Muti-line comments
   - there are some tricky ways to do multi-line comments in shell script leyt me show you some tricks for the same
   - use to open and to close (make sure you have space between:and')

## Escape
   - The escape () preceding a character tells the shell interpret the character literally

   - A non quoted backslash () is the escape. it preserves the literal value of the next character that follows with the exception of <newline>.

   - This allows you to break very long commands / commands sequences (pipping and transforming output etc). in scripts into multiple lines for readability.

   - Enter the code in the file 
   - let's run the above script and see the output

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day10/README.md) | [Next Day →](../Day12/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)

