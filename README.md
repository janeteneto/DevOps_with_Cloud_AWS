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


5.
