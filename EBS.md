### So here we are going to perform EBS tasks so for that we need to follow below steps also you can follow EBS-Configuration file for reference.

------------------------------------------------------------------------------------------------------------------------------------------

#### Step 1:-

So as per our task we need to create two volume and attach it to respective insance.hence we have created two volume

1) 10 GiB
2) 15 GiB

For volume creation kindly follow EBS-configuration file.

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/f20312ce-50dc-467a-8896-a822b3f5f6e4)

#### Step 2:-

Go to action button and attach both volumes to the EC2 Instance which is created in us-east-1 region.

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/4710b90a-d829-47d7-8d60-4758f3625e44)

follow the same process for another volume...

#### Step 3:-

Connect to EC2 Instance and list the available disk devices to verify the attachment hrough below command.

      lsblk



#### Step 4:-

Create File Systems using the below command
      sudo mkfs -t xfs /dev/xvdf
      sudo mkfs -t xfs /dev/xvdk






