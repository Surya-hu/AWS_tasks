### Create a S3 bucket, with no public access and upload files to the bucket & view the logs using Cloudwatch for the uploaded files.

Created s3 bucket with no public access in the name of suryak:  
Click on "Create bucket".  
Enter a unique bucket name and choose the region.  
Uncheck "Block all public access".  
Leave other options as default and click "Create bucket".  

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/50bff7cd-5e15-4127-be9f-9a7a514a18af)

Set up CloudWatch Logging for S3 Access Logs:<br>
Go to the S3 console.<br>
Select your bucket.<br>
Click on the "Properties" tab.<br>
Under "Server access logging", click "Edit".<br>
Choose the target bucket for your access logs and click "Save".<br>

Then uploaded the files in bucket and waited for logs to be created.<br>

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/8b97d6ba-1f76-421e-a3ee-bc3afb5d0e04)

Logs were successfully created.

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/ddbc18cb-466b-4e97-aff0-c9993c98f10d)


![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/1392bc17-42ca-4bc1-b6fc-3a8da0bdc002)


### Launch two ec2-instances and connect it to an application load balancer, where the output traffic from the server must be a load balancer IP address"

Launched 2 ec2 instances

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/b1520c46-1e2b-495f-8cb5-2083a1979e61)

Create Load Balancer:

In the EC2 Dashboard, under "Load Balancing" in the navigation pane, click on "Load Balancers".  
Click the "Create Load Balancer" button.  
Choose the appropriate load balancer type based on your requirements (Application Load Balancer, Network Load Balancer, or Classic Load Balancer).  

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/3c0aec44-77b3-4b6a-a304-df20e84b96e2)

Created Target group and associated this with instances created

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/8c242fa5-345a-4743-9127-75cfeaef1eab)


For the testing purpose installed inginx and httpd in each servers and used the load balanacer DNS and successfully connected to the server. Load balancer worked as expected.

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/bd068298-6dfd-4632-a7fb-dd4f4a9dbd8a)

![image](https://github.com/Surya-hu/AWS_tasks/assets/119995742/c89459d1-0eb9-4832-8722-a7ad21d2a398)





