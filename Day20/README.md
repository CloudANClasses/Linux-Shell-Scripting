## Day 20 Shell Scripting If With Files & Not Operator in Shell Script

  - Suppose we want to check that file is a regular file or directory, the file have read, write or execute then again we have use test command with if Condition
  
  - Here is an example

   #!/bin/bash
   file_full_path="/home/kali/abc.txt"

   # check file is a directory.
   if [[ -d $file_full_path ]]
   then
   echo  "${file_full_path} is a dir"
   fi

# -b means file is block device.
   if [[ -b $file_full_path ]]
   then
   echo  "${file_full_path} is a block device"
   fi

#check, file is a char device.
   if [[ -c $file_full_path ]]
   then
   echo  "${file_full_path} is a char device"
   fi

#check, file exists.
   if [[ -e $file_full_path ]]
   then
   echo  "${file_full_path} is a exist device"
   fi

#check, file have read permission.
   if [[ -r $file_full_path ]]
   then
   echo  "${file_full_path} have read permission"
fi

# check, file have write permission
   if [[ -w $file_full_path ]]
   then
   echo  "${file_full_path} have write permission"
   fi
# check file have execute permission.
   if [[ -x $file_full_path ]]
   then
   echo  "${file_full_path} have execute permission"
   fi

## Not Operator in shell Script

  - The NOT logical operator reverses the true/false outcome of the expression that immediately follows.
  - For example, If a file does not exist then display an error on the screen.

#!/bin/bash
   name="saurav sharma"
   othername="gaurav sharma"
   if [[ ! ${othername} == ${name} ]]
   then
    echo "both are same"
   fi

  - now let's run the above the program
  - ./if-not.sh

## OR || Operator in shwll Script

  - This is logical OR. if one of the operatot is true, then the condition becomes true.
  - syntax: 
     command1 && command2
  - command2 will execute if command1 has failed
  - and it returns false only and if all commands return not zero exit code
   cloudan㉿test)-[~/shellscript-youtube]
   $ ping -c 1 8.8.8.8>/dev/null || echo "Internet is not working."
   Internet is not working.
  - Example
#!/bin/bash
# os == linux && user == root
   OS_TYPE=$(uname)
   if [[ ${OS_TYPE} == "Linux" || ${UID} -eq 0 ]]
   then
  echo "user is root user or os is linux."
   fi
  - let's execute the above program as a non-root user and see the output
   test㉿cloudan)-[~/shellscript-youtube]
   └─$ ./if-or-operator.sh
   user is root user or os is linux.

  - now let's run the same program as a root user.
   ┌──(test㉿cloudan)-[~/shellscript-youtube]
   └─$ sudo su                                                                       1 ⨯
   [sudo] password for gaurav:
   ┌──(root💀-cloudan)-[/home/kali/shellscript-youtube]
   └─# ./if-or-operator.sh
   user is root user or os is linux.



  - Student work:
  - Write an Article & post it on LinkedIn Shell Scripting.

 [← Previous Day](../Day19/README.md) | [Next Day →](../Day21/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
