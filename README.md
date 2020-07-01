# backup-script
Simple python script for RDS encrypted backup and export to S3 bucket.
Usage example: 

python rds_backup.py --db_instance <rds_instance_name> --s3_bucket <your_bucket_name> --kms_key <kms_key_used_for_encryption> --iam_role_arn <iam_role_arn>

For the script to work properly you need to run it with a role tha has the following permissions:
For RDS, the following permissions are required:

rds:CopyDBSnapshot

rds:DescribeDBClusters 

rds:DescribeDBClusterSnapshots 

rds:DeleteDBSnapshot 

rds:DescribeDBInstances 

rds:DescribeDBSnapshots 

For S3, the following permissions are required:

s3:ListBucket

s3:GetBucketLocation

s3:PutObject*

s3:GetObject*

s3:DeleteObject*

For KMS, the following permissions are required:

kms:Decrypt

kms:Encrypt

kms:DescribeKey

More: https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles_use_passrole.html
