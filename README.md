# backup-script
Simple python script for RDS encrypted backup and export to S3 bucket.
Usage example: 


--db_instance grafana-test --s3_bucket 'se.test.upload.wh.geniussports.com' --kms_key '2e20af4f-52df-4d93-8723-3809a7990f8a' --iam_role_arn 'arn:aws:iam::239990938293:role/rds-s3-export-role'
