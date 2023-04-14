**Here are some of the commands used for the AWS session** (tech221 is just for illustration, change for filename):

`ls` - sees inside folder

`whoami` - checks who is the user

`pwd` - sees present directory

`uname` - name of program

`uname -a` - all details of program

`touch tech221.txt` - creates tech221.txt file

`nano tech221.txt` - opens nano editor to edit file

`cat tech221.txt` - shows file's content

`cp tech221.txt tech221` - copies file to other location

`rm tech221.txt` - removes file

`mv tech221.txt tech221` - moves file

`ll` - shows permissions

`top` - to see every command's date and pid user

`history` - to see every command made during that session and that user

`head` - to see first line of code in a file

`nl` - to see all lines of code in a file

`tail` - to see last line of code

`| grep test` - grabs the word in the file if it exists

`ls | tail - 1` - shows the last file created

`ps aux | grep bash` - to find everything bash is running locally

`sudo su` - to go to the admin user. then type `exit` to leave

`sudo apt install (+ what you want to install)` - downloads stuff

`sudo apt update` - downloads updates

`sudo apt upgrade` - does the actual upgrade

add `-y` to confrim we already said yes

`sudo systemctl status nginx` - check nginx status

`sudo nano provision.sh` - create file

`sudo chmod +x provision.sh` - makes it executable

**provision.ch - shell cript code:**

````
#!/bin/bash
sudo apt update -y
sudo apt upgrade -y
sudo apt install nginx -y
sudo systemctl restart nginx
sudo systemctl enable nginx
````
