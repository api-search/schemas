---
description: Describes where logs are stored and the prefix that Amazon S3 assigns to all log object keys for a bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTlogging.html">PUT Bucket logging</a> in the <i>Amazon S3 API Reference</i>.
layout: schema
name: LoggingEnabled
properties_list:
- description: ''
  name: TargetBucket
  type: object
- description: ''
  name: TargetGrants
  type: object
- description: ''
  name: TargetPrefix
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-loggingenabled-schema.json
slug: s3-loggingenabled
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: LoggingEnabled
---
