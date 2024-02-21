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

