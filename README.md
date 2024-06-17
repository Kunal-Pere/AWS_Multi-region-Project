# AWS_Multi-region-Project
Multi-region Web Server Deployment with EBS Volume Management

#### In this project we are going to deploy web server in multi-region and manage the EBS volume.

#### Step 1 :-

Follow the EC2-Configuration file to create ec2 instance in us-east-1 (North-Virginia) region.

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/5e0352fe-d3a3-468d-a01d-a30c5990ea53)

#### Step 2 :-

Once the instance get launch connect it and update the instance with below command.

     sudo apt update -y
#### Step 3 :-

As per given task we need to replicate the instance in the US-West-2(Oregon) region hence we need to create image of this us-east-1 region instance and once the image create then follow the below steps.

    1) Go to AMI section.
    2) Select that created image.
    3) Go to Action button.
    4) select copy AMI.

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/846a9d6d-3e1f-4fce-96ca-b1541591e9a2)


    Now we have to copy our image in required region which is us-west-2 (Oregon) and give name to that AMI.

#### Step 4 :- 

Now got to us-west-2(Oregon) region and follow the below steps.

     1) Go to AMI section.
     2) Select copied AMI.
     3) Click on launch instance from AMI.


     

