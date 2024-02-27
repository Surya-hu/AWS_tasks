### Launch an EC2 instance (Linux and Windows) along with a web server. Then, create an EBS volume of 5 GB, attach it to an EC2 machine (Linux and Windows), and take a snapshot. Finally, create an EBS volume using the taken snapshot.

Created EBS volume using the documents provided and attached to the EC2 machine as shown below

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/3f5b8d74-7e72-4c01-b266-1f7c23ffca6b)


![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/78437840-4258-4b77-99ee-087f226adb5d)

Format and Mount the EBS Volume (Linux)

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/bf5fb9fe-6272-4bc5-b40e-7fbaf811f2f1)

Create a mount point for the volume:
`sudo mkdir /mnt/my_volume
sudo mount /dev/xvdf /mnt/my_volume`
updated /etc/fstab to automatically mount the volume on system boot using below details:
`sudo vi /etc/fstab`

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/254ebb26-990d-4b80-85bc-3e62e6d56449)

Found the directory has been mounted properly

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/17fe5081-4725-4453-ab47-abfba1157207)

Created snapshot

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/ee28c66c-70c0-4c16-ba9b-51005ac60abb)

Launched windows ec2 machine as shown in the picture:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/cfeb02f7-29cd-4a22-8d06-5c0ab66c7315)

Attached the EBS volume in windows EC2 machine:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/86a7ed16-c785-4a0f-80bf-63af06161c85)

Attached the EBS volune to windows machine as directed by Disk management portal make it online, Initialize Disc and create new volume, As it shows 5GB of local disc D created:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/7db7b804-aa1a-4389-b4b2-1bf64e4a34b1)

created snapshot using ebs volume:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/982dcb34-7e08-4910-b78c-540a5dd8d4cb)

Using the snapshot created volume and using that volume launced the EC2 also we can attach the same snapshot while creating the instance using snapshot ID option in add volume and checked the folder(files) if exists. successfully found the folder as shown below:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/2bd2ce82-852c-437a-860b-6deaf4e124f8)


![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/810c27dc-e19c-4ab1-8f21-a2a24bd1ccde)


![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/a553ed26-7094-445d-8773-dd3509088284)
