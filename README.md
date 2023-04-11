# Using SSH with GitHub

We first learned how to push our local changes to our remote repository on GitHub using HTTPS, and now we will learn the stpes to the same thing but using SSH which is a cryptographic network protocol used to secure remote access to a computer or server. There are 5 main steps to achieve this:


**1. Create an SSH key** in local computer

**2. Register padlock** at GitHub

**3. Add private key to SSH register** in local computer

**4. Create a test repo** on GitHub

**5. Use SSH to push changes** in local computer

- We will break this down into smaller steps while following that same order:

1. Open Git bash to create new directory called ".ssh" using the following command and press enter:

![2023-04-11](https://user-images.githubusercontent.com/129942042/231201636-d3421564-bbff-4eda-be87-3c701473b74f.png)

2. After having pressed enter, a file has been created. To get inside the file and verify it exists enter the command "cd .ssh", and then we will generate the key on our local computer following the second command (replace youremail@gmail.com for your real e-mail address):

![2023-04-11 (2)](https://user-images.githubusercontent.com/129942042/231203814-946cc9e8-ff1f-4066-8af4-33c0cfe790d5.png)

3. After pressing enter, the terminal will ask for a name for the key, and we can personalise this to make it convenient:

![2023-04-11 (3)](https://user-images.githubusercontent.com/129942042/231208310-adc32ebc-ce7f-4a8a-b87f-6cd7411bd194.png)

4. Press enter twice leaving the passphrase empty and you will be able to see this:

![2023-04-11 (4)](https://user-images.githubusercontent.com/129942042/231210473-8fa93dab-8532-472a-bd73-db8210a7ee86.jpg)


5. Now, to get our public version of the key to copy and paste to register on GitHub, enter the following commands and you should get a very long set of characteres:

![2023-04-11 (7)](https://user-images.githubusercontent.com/129942042/231215899-e670fc3d-94a7-46ca-9b41-e4a7d3d1dc3f.png)
![2023-04-11 (8)](https://user-images.githubusercontent.com/129942042/231215948-57ebb0bd-98e2-40de-840d-ddaddf770a26.png)


6. We are now able to register the padlock on GitHub by following these steps:

![2023-04-11 (5)](https://user-images.githubusercontent.com/129942042/231222174-823dab02-2611-495e-aeb5-0727b9a25d81.jpg)
![2023-04-11 (11)](https://user-images.githubusercontent.com/129942042/231222256-7d45fa87-f4b5-49f3-a823-a8d75ce36b3d.jpg)

Now, copy and paste the set of characters from the terminals that starts with ssh and ends with your e-mail:

![2023-04-11 (11)](https://user-images.githubusercontent.com/129942042/231222975-0baad20d-ad46-4446-8e2a-7214c2ef994b.png)

7. After adding the key and verified it has been registered on GitHub, we need to add the private key to SSH Register. Enter the command to start running the process:

![2023-04-11 (12)](https://user-images.githubusercontent.com/129942042/231225777-a28faac9-1c81-4531-8d06-90b6fefb71b5.png)

"Agent pip" messages should pop up then enter this command:

![2023-04-11 (13)](https://user-images.githubusercontent.com/129942042/231229599-f126dadd-5d7d-4f99-a21e-6f2afdc07f71.png)

And this command after the "Identity added" message pops up and press enter and verify if entity has been created:

![2023-04-11 (14)](https://user-images.githubusercontent.com/129942042/231229690-dd495855-cae5-48a9-a68f-5c34ecaf7722.png)
![2023-04-11 (15)](https://user-images.githubusercontent.com/129942042/231230610-ce887624-eb4f-405b-a0c6-db60a12e969e.png)

8. We can now move on to create a test repo on GitHub called "tech221-aws" and get the SSH link:

![2023-04-11 (17)](https://user-images.githubusercontent.com/129942042/231232043-3487d5b2-87fd-4d6c-afd9-48a85074d9e7.jpg)

9. Go back from the .shh file using the "cd .." command then create a new repository with the same name as on GitHub:

![2023-04-11 (18)](https://user-images.githubusercontent.com/129942042/231233782-0c37322d-5eb9-49d4-a707-3e25e25eee43.png)

10. Once you are inside the file, we can create a new file using the "touch" command:

![2023-04-11 (19)](https://user-images.githubusercontent.com/129942042/231235139-fd7649dd-a209-4491-9829-06dc24b35f92.png)

11. Now, we will start pushing changes using SSH, and first we used the nano editor to enter a line to our README file and then push it:
Type in "nano README.md" and the nano editor will open, then you can type any change you want, or something like this:

![2023-04-11 (21)](https://user-images.githubusercontent.com/129942042/231236548-fe7e487c-296e-41a4-8edc-ce215aea0a78.png)

12. Press CTRL + S to save, then CTRL + X to exit the editor.

13. Now we can push the changes to our remote branch. First, follow the commands to initialize git:

![2023-04-11 (22)](https://user-images.githubusercontent.com/129942042/231238747-5ab9e524-9605-4d40-b64a-39c458515708.png)

14. Now, finish pushing the change using the following commands:

![2023-04-11 (26)](https://user-images.githubusercontent.com/129942042/231239243-8482a046-7d35-42db-ad61-ca93fc071d61.png)
![2023-04-11 (25)](https://user-images.githubusercontent.com/129942042/231239288-0671e137-724d-4420-a130-491303cde94b.png)
