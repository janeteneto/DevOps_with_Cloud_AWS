# Connect Instance

During the morning session, we learned how to launch an instance with EC2. We followed the process and lauched the instance with a SSH and HTTP rule. Then for demonstration and trainning puroposes, we deleted the SSH rule, then added again, and then re-connected with the following steps:
1. First select your instance, press security and select the security group previously created:

![2023-04-13 (8)](https://user-images.githubusercontent.com/129942042/231762985-8081bc7f-e5a0-430f-bcfb-a960559d1091.jpg)

2. Then, scroll down to Edit inbound rules:

![2023-04-13 (9)](https://user-images.githubusercontent.com/129942042/231763986-fde2e0cb-8526-4745-af61-192d051906c3.jpg)

3. Press add rule and the settings you select should look like this:

![2023-04-13 (10)](https://user-images.githubusercontent.com/129942042/231764487-b13c480a-98c7-4e83-baeb-b4287a71fd3c.jpg)

4. Now we can connect the instance using the Git terminal with the commands found on AWS with these steps:

- On the instances page press connect:
![2023-04-13 (8)](https://user-images.githubusercontent.com/129942042/231765270-479a4c8c-767d-4499-a7a7-ca6bcd544561.jpg)

- Now, make sure that on Git terminal you `cd .ssh` to get in the right folder

- Then press SSH Client and copy the first command `chmod 400 tech221.pem` and paste it into the git terminal;

- After that paste the second command seen on the image into the terminal:

![2023-04-13 (12)](https://user-images.githubusercontent.com/129942042/231765651-2bbefa51-c719-479f-a9e5-702c9e04af9c.jpg)

- Now all that is left is to type `yes` and you are connected! It should look like this:

![2023-04-13 (13)](https://user-images.githubusercontent.com/129942042/231766744-dd2dcdfa-1355-41f5-8120-19a2b80a2916.png)
