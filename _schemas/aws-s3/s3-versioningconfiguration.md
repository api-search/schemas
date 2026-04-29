---
description: Describes the versioning state of an Amazon S3 bucket. For more information, see <a href="https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTVersioningStatus.html">PUT Bucket versioning</a> in the <i>Amazon S3 API Reference</i>.
layout: schema
name: VersioningConfiguration
properties_list:
- description: ''
  name: MFADelete
  type: object
- description: ''
  name: Status
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-versioningconfiguration-schema.json
slug: s3-versioningconfiguration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersioningConfiguration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"MFADelete\": {},\n    \"Status\": {}\n  },\n  \"description\": \"Describes the versioning state of an Amazon S3 bucket. For more information, see <a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/API/RESTBucketPUTVersioningStatus.html\\\">PUT Bucket versioning</a> in the <i>Amazon S3 API Reference</i>.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-versioningconfiguration-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: VersioningConfiguration
---
