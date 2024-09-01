## Day 4 I/O Redirection, Find, Users and Groups

## I/O Redirection 

  - Redirection is a process where you can copy the output of any command (s), file (s) into a new file. Ther are 2 ways of redirecting the output into a file.
  - using > or >> filename after the command and
  - ➔ Appending another output in same file with “>>” .
  - ➔ Create a file named devopstools with below content.
  ➔ Search for text “tech” replace it with “tools” and redirect output to a new file.
  - ➔ Appending another output in same file with “>>” .
  - ➔ Redirecting only error to a file “2>>”.
  - ➔ Redirecting all the output to a file “&>>”.

## Piping

  - So far we've dealt with sending data to and from files. Now we'll take a look at a
mechanism for sending data from one program to another. It's called piping and the
operator we use is ( | ). What this operator does is feed the output from the program on
the left as input to the program on the right.

## Find

  - Find command is used to find or directory path, it is exactly like the find option in windows where you can search for a file

  - option -name
  - ption -inum
  - option -type
  - option -user
  - option -group

## Users and Groups

## Users
  - Some important points related to Users:
  - Users and groups are used to control access to files and resources
  - Users login to the system by supplying their username and password
  - Every file on the system is owned by a user and associated with a group
  - Every process has an owner and group affiliation and can only access the resources its owner or group can access
  - Every user of the system is assigned a unique user ID number
  - User password is stored in /etc shadow is encrypted form.
  - Users are assigned a home directory and a program that is run when they login
  - Users cannot read, write or execute each other files without permission

  - Types of user
  - 
  - Root
  - Regualar
  - Service

  - In Linux there are three types of users

  - 1) Super user or root user
  - Super user or the root user is the most poweful user. He is the administrator user.
  - 2) System user
  - System users are the users created by the softwares or applications. For example if we install Apache it will create a user apache. These kinds of users are known as system users
  - 3) Normal user
  - Noraml users are the users created by root user. They are normal users like Rahul, Muab etc. Only the root user has the permission to create or remove a user

## Passswd file
  - /etc/passwd

## Group file
  - /etc/group
  - The file /etc/group stores group information. Each line in this file stores one group entry.


  - Student work:
  - Write an Article & post it on LinkedIn the Linux Commands

[← Previous Day](../Day03/README.md) | [Next Day →](../Day05/README.md)

 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
