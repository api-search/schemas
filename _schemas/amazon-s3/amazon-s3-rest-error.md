---
description: Container for all error elements.
layout: schema
name: Error
properties_list:
- description: The error code is a string that uniquely identifies an error condition. Examples include NoSuchBucket, NoSuchKey, AccessDenied, InvalidBucketName, etc.
  name: Code
  type: string
- description: A human-readable description of the error.
  name: Message
  type: string
- description: The bucket or object that is involved in the error.
  name: Resource
  type: string
- description: Unique identifier for the request.
  name: RequestId
  type: string
- description: A special token to help AWS troubleshoot problems.
  name: HostId
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-error-schema.json
slug: amazon-s3-rest-error
source_filename: amazon-s3-rest-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"Container for all error elements.\",\n  \"properties\": {\n    \"Code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code is a string that uniquely identifies an error condition. Examples include NoSuchBucket, NoSuchKey, AccessDenied, InvalidBucketName, etc.\"\n    },\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\"\n    },\n    \"Resource\": {\n      \"type\": \"string\",\n      \"description\": \"The bucket or object that is involved in the error.\"\n    },\n    \"RequestId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the request.\"\n    },\n    \"HostId\": {\n      \"type\": \"string\",\n      \"description\": \"A special token to help AWS troubleshoot problems.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-error-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: Error
---
