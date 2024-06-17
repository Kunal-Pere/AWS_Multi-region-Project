So here we are going to perform EBS tasks so for that we need to follow below steps also you can follow EBS-Configuration file for reference.

#### Step 1:-

Follow the steps given in EBS-Configuration and create 2 volumes of 10 GiB and 15 GiB

#### Step 2:-

Attach both volumes to the EC2 Instance created in us-east-1 region

#### Step 3:-

Connect to your EC2 Instance

#### Step 4:-

Create File Systems using the below command
      sudo mkfs -t xfs /dev/xvdf
      sudo mkfs -t xfs /dev/xvdk


![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/7f3e2570-8ad4-43a8-9ab1-d4bc3d2cf253)


![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/f20312ce-50dc-467a-8896-a822b3f5f6e4)
