## Day 14 Shell Scripting Assign a Command's Output to a Variable && Create a Read-only Variable in shell script

  - Suppose we want to store a command output to a variable in a serval way.
  - `we can use the back tick `
  - VARIABLE_NAME=`command_here`
  - we can use the brackets (recommend way)
  - VARIABLE_NAME=$(command_here)
  - EXAMPLE:
#!/bin/bash
CURRENT_WORKING_DIR=$(pwd)
VARIABLE_SECOND_METHOD=`pwd`
echo "${CURRENT_WORKING_DIR}"
echo "${VARIABLE_SECOND_METHOD}"
date_time=$(date +"%D-%T")
echo "${date_time}"

  - OUTPUT:
  ./assign-command-output.sh

## How to create a read-only variable in Shell Script

  - We can create read-only variable in shell script using readonly
  - Syntax:
  - $ readonly VARIABLE_NAME
  - let's take below example.
 #!/bin/bash
name="hinal"
# readonly name
echo "${name}"
unset name
# name="gaurav"
echo "${name}"

  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.


 [← Previous Day](../Day13/README.md) | [Next Day →](../Day15/README.md)

 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
