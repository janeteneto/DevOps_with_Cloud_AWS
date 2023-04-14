1. **Make sure you have an instance already created and connected with ssh on your aws and local machine first.**

2. Stop your current instance

**3. Create AMI's in the image of your instance:**

- On the Instances page, select your instance --> Actions --> Create Image

- Now configure your AMI with the following settings (my name is just for demonstration), then create image:

![2023-04-14 (2)](https://user-images.githubusercontent.com/129942042/232038956-b6891d23-3bcf-4856-aa71-7b6b2d954bbf.png)

- After the image starts getting created, open the AMI:

![2023-04-14 (3)](https://user-images.githubusercontent.com/129942042/232039408-a53e7f1b-f5c9-4a3b-b1b5-53f024ec6c08.jpg)

- Add a name tag to your image:

![2023-04-14 (4)](https://user-images.githubusercontent.com/129942042/232039674-b008cb5e-25d5-455e-9d73-ce3406f1b618.png)

4. Then after the image's status is 'Available', lets launch an instance by pressing the button on top right "Launch an instance"

5. The proccess to create an instance based on an image is the same. Let's add a different name to this instance something like `yourname_ec2_using_nginx_ami`.

6. To connect your instance via SSH, there is one slight difference. The user is not `root`, but instead is `ubuntu`, so we must ammend the code line on our terminal. Instead of 

````
ssh -i "tech221.pem" root@ec2-54-74-205-71.eu-west-1.compute.amazonaws.com
````

It should be: 

````
ssh -i "tech221.pem" ubuntu@ec2-54-74-205-71.eu-west-1.compute.amazonaws.com
````

And it must look like this:

![2023-04-14 (9)](https://user-images.githubusercontent.com/129942042/232040797-87e9cce2-d6aa-4483-a506-9fdf41975acc.png)

7. The process to install nginx is the same as before.
