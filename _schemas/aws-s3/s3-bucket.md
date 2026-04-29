---
description: In terms of implementation, a Bucket is a resource. An Amazon S3 bucket name is globally unique, and the namespace is shared by all Amazon Web Services accounts.
layout: schema
name: Bucket
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: CreationDate
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-bucket-schema.json
slug: s3-bucket
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Bucket\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {},\n    \"CreationDate\": {}\n  },\n  \"description\": \" In terms of implementation, a Bucket is a resource. An Amazon S3 bucket name is globally unique, and the namespace is shared by all Amazon Web Services accounts. \"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-bucket-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: Bucket
---
