# backup-script
Simple python script for RDS encrypted backup and export to S3 bucket.
Usage example: 

python rds_backup.py --db_instance <rds_instance_name> --s3_bucket <your_bucket_name> --kms_key <kms_key_used_for_encryption> --iam_role_arn <iam_role_arn>
