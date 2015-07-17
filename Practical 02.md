####ESBII Lab 02 - Creating an Amazon  EBS-Backed Linux AMI

#Creating the AMI from an Instance


#### 1.Open the Amazon EC2 console
![](https://cloud.githubusercontent.com/assets/13186210/8744632/48560436-2c96-11e5-8a5b-761a08dc9918.png) 

#### 2. In navigation pane click Instances>Actions>select image>Create image
![](https://cloud.githubusercontent.com/assets/13186210/8744663/7190a84c-2c96-11e5-9f8b-877cabb2dfe0.png)

#### 3. Put a Unique name(Test Linux) for the image and create image####
![](https://cloud.githubusercontent.com/assets/13186210/8744725/19ace1b2-2c97-11e5-8e16-4969e8134d5c.png)


#### 4. Click AMI then the status of your AMI is available####
![](https://cloud.githubusercontent.com/assets/13186210/8744737/2680e9ce-2c97-11e5-97c7-b9df7a86f671.png)

#### 4. Click Snapshots to view the snapshot that was created for the new AMI. 
![](https://cloud.githubusercontent.com/assets/13186210/8744789/a243d1a2-2c97-11e5-846c-1e5f49064ce1.png)

#Creating the AMI from a Snapshot

#### 1.Open the Amazon EC2 console
![](https://cloud.githubusercontent.com/assets/13186210/8744632/48560436-2c96-11e5-8a5b-761a08dc9918.png) 

#### 2.Under Elastic Block Store choose Snapshots and then click Actions>Create Image
![](https://cloud.githubusercontent.com/assets/13186210/8744992/1aea9928-2c99-11e5-9da5-0c4c8596852f.png)

#### 3.In the Create image from EBS Snapshot complete fields(Architecture,Root device name,Virtualization type,Kernel ID,RAM disk ID,)
![](https://cloud.githubusercontent.com/assets/13186210/8744994/28ade312-2c99-11e5-833c-f274ca9eac12.png)

#### 4.Create Snapshot
![](https://cloud.githubusercontent.com/assets/13186210/8745002/37de6000-2c99-11e5-8c8a-8f82b23ae1a4.png)

#### 4.Click AMI then you can see both AMI.
![](https://cloud.githubusercontent.com/assets/13186210/8745008/41c720e8-2c99-11e5-80c0-44a1be7c93b7.png)