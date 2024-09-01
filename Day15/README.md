## Day 15 Shell Scriptig Convert String & Substring in Script

  - Convert First Character to upper Case in Shell Script
#!/bin/bash
string="my name is CloudAN"
echo "${string^}" # My name is CloudAN

  - Convert a String to Upper case in Shell Script
#!/bin/bash
string="my name is CloudAN"
echo "${string^^}" # MY NAME IS CloudAN

  - Convert First Character to Lower Case in Shell Script
#!/bin/bash
string="My name is CloudAN"
echo "${string,}" # my name is CloudAN

  - Convert a String to Lower Case in Shell Script
#!/bin/bash
string="My name is CloudAN"
echo "${string,,}" # my name is CloudAN

  - Get the Length of String in Shell Script
#!/bin/bash
string="My name is CloudAN"
echo "length of string variable is ${#string}"

#!/bin/bash
string="my name is CloudAN"
echo "${string}"   # my name is CloudAN
echo "${string^}"  # My name is CloudAN
echo "${string^^}" # MY NAME IS CloudAN
string="My name is Gaurav"
echo "${string}"  # My name is CloudAN
echo "${string,}" # my name is CloudAN
echo "${string,,}" # my name is CloudAN
echo "length of string variable is ${#string}"

 - Output
 - ./string-variable.sh

## Substring in Shell Script

 - Get Substring from a String
 - Syntax
${string:position}
 - example
#!/bin/bash
string="abcgauravabcxyz"
echo "${string:0}"  # output -> abcgauravabcxyz
echo "${string:1}"  # bcgauravabcxyz
echo "${string:4}"  # auravabcxyz

## Get Last n Character from a String
#!/bin/bash
string="abcgauravabcxyz"
echo "${string: -3}" # xyz

## Get Substring with specific Length from String
#!/bin/bash
string="abcgauravabcxyz"
echo "${string:0:3}"
echo "${string:3:3}"

## Get Shortest Match from Starting in a String
#!/bin/bash
string="abcgauravabcxyz"
echo "${string#a*c}" # from starting, shortest match

## Get Longest Match from Starting in A String
#!/bin/bash
string="abcgauravabcxyz"
echo "${string##a*c}" # from starting, longest match


## Get Shortest Match from the End
#!/bin/bash
string="abcgauravabcxyz"
echo ${string%b*z} # from ending, shortest match

## Get Longest Match from the End
#!/bin/bash
string="abcgauravabcxyz"
echo "${string%%b*z}" # from ending, longest match

## Let's create a single script and execute it
#!/bin/bash

string="abcgauravabcxyz"

echo "${string:0}"
echo "${string:1}"
echo "${string:4}"
echo "${string:0:3}"
echo "${string:3:3}"
echo "${string: -5}"

echo "${string#a*c}"  # from starting, shortest match
echo "${string##a*c}" # from starting, longest match

echo ${string%b*z}  # from ending, shortest match
echo "${string%%b*z}" # from ending, longest match

string="abcgauravabcxyz"

echo "${string/abc/xyz}"
echo "${string//abc/xyz}"

echo "${string/abc}"
echo "${string//abc}"

  - Output
  - ./substring.sh

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day14/README.md) | [Next Day →](../Day16/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
