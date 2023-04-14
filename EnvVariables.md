## - Create instance with user data:

1. Press "Launch Instance" on the Instances page on top right then fill all settings as normal

2. Additionally, we need to press "Advanced Settings", scroll until the bottom, then add the scrip code lines as follows:

![2023-04-14 (10)](https://user-images.githubusercontent.com/129942042/232071027-a87c8927-90a7-4b6a-9905-5efe6449a014.png)

````
#!/bin/bash
sudo apt update -y
sudo apt upgrade -y
sudo apt install nginx -y
sudo systemctl restart nginx
sudo systemctl enable nginx
````

## - If there are no blockers, the instance has been launched with ngnix. Now let's move to create environments and variables in Linux.:

1. Connect instance via SSH. The process is the same as usual.

2. Find info on the available environments with command `printenv`

3. Find your env current location with command `printenv pwd`

4. To see env info, simply type command `env`

5. To exit env, simply type `exit`. And to login just use the last command runned on master user

6. *It is simple to creable a varible. Just type:*
 
````
variablename=valueofvariable
````

- Use command `echo $variablename` to see value of variable

- Command `export variablename=valueofvariable` to export

** Environments are not persistent.** Which means every variable created on in will disappear if we exist. To make it persistent we need to source the bash environemnt:

1. First, let's add a variable to the bash env, by running the following command that opens nano and allows us to edit it:
````
sudo nano .bashrc
````
- Type in a variable name and value in the format `variablename=valueofvariable`

2. Save and exist nano by pressing `CTRL + S` then `CTRL + X` 

3. Run the command:
````
source .bashrc
````

4. Lastly, if we want to test the env we can exit, login again and run the command `printenv variablename`.
