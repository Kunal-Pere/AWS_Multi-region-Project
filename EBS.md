### So here we are going to perform EBS tasks so for that we need to follow below steps also you can follow EBS-Configuration file for reference.

------------------------------------------------------------------------------------------------------------------------------------------

#### Step 1:-

So as per our task we need to create two volume and attach it to respective insance.hence we have created two volume

1) 10 GiB
2) 15 GiB

For volume creation kindly follow EBS-configuration file.

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/f20312ce-50dc-467a-8896-a822b3f5f6e4)



#### Step 2:-

Attach both volumes to the EC2 Instance created in us-east-1 region

#### Step 3:-

Connect to your EC2 Instance

#### Step 4:-

Create File Systems using the below command
      sudo mkfs -t xfs /dev/xvdf
      sudo mkfs -t xfs /dev/xvdk






