### set up a VPC with an Internet gateway, create a public subnet with 256 IP addresses, a private subnet with 156 IP addresses, make a route table connecting the Internet gateway and the subnets, and launch a Linux EC2 instance by using the above vpc and public subnet.

Created VPC using vpc console as shown below with CIDR value of 10.0.0.0/16:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/80890fb3-7040-47f0-a562-8da7bed2b3cf)

Then created 4 subnets 2 public and 2 private subnets(each 256 IPs)

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/f93f0d77-4032-4b3d-b3ac-10a4f53933c1)

Then created Internet gateway and attached the created VPC:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/ecefb2ed-bb34-474f-a042-2e999cf662b8)

Created Route table and associated the public subnets to route tables:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/dd93d4d7-a431-4210-a5d0-df235ef68ee8)

Added public route to the route table for the public subnets associated through internet gatway which is created:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/da89384a-4a5b-40c3-978d-93c9b6be5413)

Created NAT gatway for instance connections inside vpc:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/47c59587-f03b-4093-bbca-e025b3277472)

Created another route table wityh private IPs and associated the NAT gatway:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/3ea8a548-5c30-4ee5-ac93-7cc3d6c7825a)

Finally creating the EC2 machine using my custom vpc and public subnet as shown in the picture:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/bd41433b-37fc-4c83-a79d-83be193379d5)

Loggged into the EC2 machine and installed httpd service to check and found it works:

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/f0a99f58-e20a-4d8b-b0be-f51510f88fc3)


![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/976b4004-e333-4187-8c3f-5e826e15b1ca)



