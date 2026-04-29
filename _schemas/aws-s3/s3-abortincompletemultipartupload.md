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
source_filename: s3-abortincompletemultipartupload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AbortIncompleteMultipartUpload\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DaysAfterInitiation\": {}\n  },\n  \"description\": \"Specifies the days since the initiation of an incomplete multipart upload that Amazon S3 will wait before permanently removing all parts of the upload. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/mpuoverview.html#mpu-abort-incomplete-mpu-lifecycle-config\\\"> Aborting Incomplete Multipart Uploads Using a Bucket Lifecycle Policy</a> in the <i>Amazon S3 User Guide</i>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-abortincompletemultipartupload-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: AbortIncompleteMultipartUpload
---
