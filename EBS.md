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

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/20828ab0-1e81-4546-a530-201bbc07a82f)
 

#### Step 4:-

Create a file system on the volume (e.g., ext4). we have two volume so we need to create two file system.

      sudo mkfs -t ext4 /dev/xvdf
      sudo mkfs -t ext4 /dev/xvdp

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/f43af34b-b825-47b4-8439-fef868088551)


#### Step 5:-

Create a directory as a mount point.

      mkdir dir1
      mkdir dir2

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/caff4eb6-b73e-4fe5-9586-afe6fd9a0f3d)


#### Step 6:- 

Now mount the volumes on this mount point(directory) and verify it with below commands.

      sudo mount /dev/xvdf dir1
      sudo mount /dev/xvdf dir2

      Now verify it using below command

      lsblk
      df -h

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/6feb0e12-189b-4e8d-b73f-ed48c8d44ad8)


#### Step 7:- 

So now we need to delete one volume after detaching it and extend the size of the other volume.

      For unmount the volume use below command

      sudo umount /dev/xvdf

now go to volume section and detach the same volume from the instance and later delete that volume.

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/3aa0cf96-c2c5-4d11-8e65-6337f6152893)


#### Step 8:-

So as per remaining task we need to extend size of other volume.

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/6fe852dc-95b7-464c-8799-bea1566530bd)


#### Step 9:-

And in last we have to take snapshot of our remaining volume so for this follow the below step.

![image](https://github.com/Kunal-Pere/AWS_Multi-region-Project/assets/157100045/135c7aaa-7adc-406a-b82c-bec306ec1bc3)


### Thank You

### Kunal Pere











