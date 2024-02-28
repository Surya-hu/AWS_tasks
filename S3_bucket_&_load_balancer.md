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


