# Linux Guide

- During the morning session, we learned how to launch an instance with EC2 and connect it with SSH using the Git Bash terminal. We then, in the afternoon, learned how to launch a nginx web server, and learned other Linux permissions executions via the terminal.

## How to launch an instance on AWS:

1. On AWS, search for EC2 and select the first one, then press Launch instance:

![2023-04-13 (23)](https://user-images.githubusercontent.com/129942042/231832059-8c1c996b-beab-41a0-a779-8b89ae1b3b43.png)

2. Before we launch, we must set the configurations of the settings. Follow the following steps on the images:

- Select Ubuntu:

![2023-04-13 (17)](https://user-images.githubusercontent.com/129942042/231832511-920d0e12-3db9-447b-9dd1-a8bd608c2c72.jpg)

- Select the correct key pair and select t.2micro:

![2023-04-13 (20)](https://user-images.githubusercontent.com/129942042/231833105-6bb3f97d-febf-431f-a973-0989231df38c.png)

- Lastly, configure the security group to look like this; you can also edit the name of the SG from `launch_wizard` to something you prefer by pressing Edit, but this is optional:

![2023-04-13 (18)](https://user-images.githubusercontent.com/129942042/231832845-51e23406-8569-45e0-97e1-578ec0249772.jpg)

4. Now finish by pressing the Launch instance button, and if there are no blockers, the instance has succefully been created. We can move on and connect the instance using the Git terminal with the commands found on AWS with these steps:

- On the instances page press connect:

![2023-04-13 (8)](https://user-images.githubusercontent.com/129942042/231765270-479a4c8c-767d-4499-a7a7-ca6bcd544561.jpg)

- Now, make sure that on Git terminal you `cd .ssh` to get in the right folder

- Then press SSH Client and copy the first command `chmod 400 tech221.pem` and paste it into the git terminal;

- After that paste the second command seen on the image into the terminal:

![2023-04-13 (12)](https://user-images.githubusercontent.com/129942042/231765651-2bbefa51-c719-479f-a9e5-702c9e04af9c.jpg)

- Now all that is left is to type `yes` and you are connected! It should look like this:

![2023-04-13 (13)](https://user-images.githubusercontent.com/129942042/231766744-dd2dcdfa-1355-41f5-8120-19a2b80a2916.png)


