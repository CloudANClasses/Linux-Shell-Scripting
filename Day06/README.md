## Day 7 Sudoers file and Sofware Management

## Sudo 

  - sudo gives power to a normal user to execute commands which is owned by root user.
  - Example shown below:
  - If a user has already full sudoers privilege, it can become a root user anytime.
  - ➔ sudo -i changes from normal user to root user

  - Note: User imran was already a sudo user with full privilege.
  - ➔ Adding user sam in sudoers list.

  - ➔ Like a user a group can also be added into sudoers list.
  - ➔ Every time you enter sudo command it asks your own password. To turn that off use
  - NOPASSWD in sudoers file.
  - ➔ Changing to any other user with “su -” command.
  - ➔ Become a root user from sam user login.

## Software Mangement

  - ➔ Download package from internet.
  - For CentOS
  - To install Tree
# curl https://rpmfind.net/linux/centos/7.9.2009/os/x86_64/Packages/tree-1.6.0-10.el7.x86_64.rpm -o tree-1.6.0-
  - 10.el7.x86_64.rpm
# rpm -ivh tree-1.6.0-10.el7.x86_64.rpm

  - To install httpd
# curl https://rpmfind.net/linux/centos/7.9.2009/os/x86_64/Packages/httpd-2.4.6-95.el7.centos.x86_64.rpm -o httpd-
  - 2.4.6-95.el7.centos.x86_64.rpm
# rpm -ivh httpd-2.4.6-95.el7.centos.x86_64.rpm

  - download and install new software, resolves software dependencies and installs the required RPM package
  - files. YUM Repository configuration files must: be located in /etc/yum.repos.d
# ls /etc/yum.repos.d/

  - Shows the usage of YUM Command with options
# yum –help

  - To Update all your packages
# yum update

  - To install httpd
# yum install httpd -y

  - To remove httpd
# yum remove httpd -y

  - To update all your package lists
#apt update

  - TO search for a <package> apache2
# apt search apache2

  - To install apache2
# apt install apache2 -y

  - To remove apache2
# apt remove apache2 -y

## More commands of Packages with Description

  - Student will study with the notes


  - Student work:
  - Write an Article & post it on LinkedIn the Linux Commands

[← Previous Day](../Day06/README.md) | [Next Day →](../Day08/README.md)


 - All the Best !! Happy Learning
 - CloudAN Classes
 - Website: cloudanclasses.com
 - Email: info@cloudanclasses.com
 - Mob: 94649-47360 (Maninder Singh)
