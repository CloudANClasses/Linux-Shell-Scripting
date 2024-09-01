## Day 5 Linux Users & groups,cheat sheet USER & Group, File Permissions

## ADD user,Set Password & Switch User
  - Practical
## Add
  - Practical
## Add User, Group & User into Group
  - Practical
## Delete user and Groups
  - Practical

## The /etc shadow file

  - This file stores users’ password and password related information. Just like /etc/passwd file,
  - this file also uses an individual line for each entry.

  - Username
  - Encrypted password
  - Number of days when password was last changed
  - Number of days before password can be changed
  - Number of days after password must be changed
  - Number of days before password expiry date to display the warning message
  - Number of days to disable the account after the password expiry
  - Number of days since the account is disabled
  - Reserved field

## User and Group Cheat sheets

  - useradd		Create a user RedHat
  - adduser		Creates user ubuntu
  - id		Shows user info
  - groupadd		Create group
  - usermod -aG grpnam usrname	Adds user to group
  - passwd		set/reset password
  - userdel -r		removes user with home dir
  - groupdel		removes group
  - last		shows last login in system
  - who		who is logged into system
  - whoami		username
  - lsof -u user		list files opened by user

## File Permissions

## Viewing Permissions from the commnad-line

  - File permissions may be viewed using ls -l
  - ls -l /bin/login

  - Four symbols are used when displaying permissions

  - r: permission to read a file or list a directory contents
  - w: permission to write to a file or create and remove files from a directory
  - x: permission to execute a program or change into a directory and do a long listing of the directory
  - -: no permission (in place of the r,w,x)


  - Student work:
  - Write an Article & post it on LinkedIn the Linux Commands

[← Previous Day](../Day04/README.md) | [Next Day →](../Day06/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)

