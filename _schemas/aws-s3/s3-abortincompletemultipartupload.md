---
description: Specifies the days since the initiation of an incomplete multipart upload that Amazon S3 will wait before permanently removing all parts of the upload. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/dev/mpuoverview.html#mpu-abort-incomplete-mpu-lifecycle-config"> Aborting Incomplete Multipart Uploads Using a Bucket Lifecycle Policy</a> in the <i>Amazon S3 User Guide</i>.
layout: schema
name: AbortIncompleteMultipartUpload
properties_list:
- description: ''
  name: DaysAfterInitiation
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-abortincompletemultipartupload-schema.json
slug: s3-abortincompletemultipartupload
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: AbortIncompleteMultipartUpload
---
