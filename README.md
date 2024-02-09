# terraform-interview-task

Please, create a separate module for each of the resources below (VPC, EC2, S3, Route53)
1. Clone this repository and give us a link to it when you are complete 
2. Using Terraform deploy to the eu-west-1 region:

   a. 1x VPC (192.168.50.0/16) with 4 subnets:

   	  i. 2x Public Subnets

   	  ii. 2x Private Subnets

   b. 1x EC2 Instance (t3.nano)

   	  i. Deploy the instance to one of the Private Subnets

   c. 1x S3 Bucket - you can use the random function in terraform to get the name of this

   	  i. The bucket must use the appropriate encryption

   	  ii. The bucket's policy must allow only the account owner to perform all the "s3:*" operations

   	  iii. Anyone else should have limited permissions: s3:ListBucket, s3:GetObject  

   d. 1x Internal Route53 Zone controller-test.com

   e. 1x Route53 Record brand-test.controller-test.com pointing to the Instance's Private IP Address created in step 1.b.

1. The Terraform State file can be stored where you like.

1. Commit the changes to the repository.
