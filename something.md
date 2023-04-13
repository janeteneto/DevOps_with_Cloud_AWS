cat (filename) - to see whats inside

head to see first line of code
nl to see all of them
tail to see last line of code
ps to see times and pids?

top to see verythinf dates and pids users

cat tech221.txt | grep test - grabs the word in the file if it eists

ls | tail - 1 : shows the last file created

ls | 

ps aux | grep bash : to find everything bash is running locally

sudo su - to go to the admin user? then exit to go out

sudo apt install (what u wnat to install) - downloads stuff

sudo apt update - downloads updates

sudo apt upgrade - does the actual upgrade

add `-y` to confrim we already said yes

sudo systemctl status nginx - check nginx

copy ip address on instance and check if its working on the browser

sudo nano provision.sh - create file

sudo chmod +x provision.sh - makes it executable

#!bin/bash

\# update
sudo apt update -y

\# upgrade
sudo apt upgrade -y

\# instal Nginx
sudo apt install nginx

\# restart nginx
sudo systemctl restart nginx

\# enable nginx
sudo systemctl enable nginx

