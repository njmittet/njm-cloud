# www-njm-cloud

Website for www.njm.cloud.

## Deployment

This website is deployed to an [AWS S3](https://aws.amazon.com/s3/) bucket. The following [AWS CLI](https://aws.amazon.com/cli/) commands may come in handy:

```shell
# List buckets.
aws s3 ls

# List the content of a bucket.
aws s3 ls <bucket-name>

# Delete a file.
aws s3 rm s3://<bucket-name>/<filename>

# Upload a file.
aws s3 cp index.html s3://<bucket-name>

# Delete all files in a bucket.
aws s3 rm s3://<bucket-name> --recursive

# Sync a local directory with a bucket.
aws s3 sync . s3://<bucket-name>
```

The AWS CLI S3 documentation can be found at [https://docs.aws.amazon.com/cli/latest/userguide/cli-services-s3.html](https://docs.aws.amazon.com/cli/latest/userguide/cli-services-s3.html).
