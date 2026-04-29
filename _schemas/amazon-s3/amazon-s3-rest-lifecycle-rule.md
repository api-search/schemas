---
description: A lifecycle rule for individual objects in an Amazon S3 bucket.
layout: schema
name: LifecycleRule
properties_list:
- description: Unique identifier for the rule.
  name: ID
  type: string
- description: The filter used to identify objects for the rule.
  name: Filter
  type: object
- description: If Enabled, Amazon S3 executes the lifecycle actions. If Disabled, Amazon S3 ignores the lifecycle actions.
  name: Status
  type: string
- description: ''
  name: Expiration
  type: object
- description: ''
  name: Transition
  type: array
- description: ''
  name: NoncurrentVersionExpiration
  type: object
- description: ''
  name: NoncurrentVersionTransition
  type: array
- description: ''
  name: AbortIncompleteMultipartUpload
  type: object
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-rest-lifecycle-rule-schema.json
slug: amazon-s3-rest-lifecycle-rule
source_filename: amazon-s3-rest-lifecycle-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LifecycleRule\",\n  \"type\": \"object\",\n  \"description\": \"A lifecycle rule for individual objects in an Amazon S3 bucket.\",\n  \"properties\": {\n    \"ID\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the rule.\"\n    },\n    \"Filter\": {\n      \"type\": \"object\",\n      \"description\": \"The filter used to identify objects for the rule.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"If Enabled, Amazon S3 executes the lifecycle actions. If Disabled, Amazon S3 ignores the lifecycle actions.\"\n    },\n    \"Expiration\": {\n      \"type\": \"object\"\n    },\n    \"Transition\": {\n      \"type\": \"array\"\n    },\n    \"NoncurrentVersionExpiration\": {\n      \"type\": \"object\"\n    },\n    \"NoncurrentVersionTransition\": {\n      \"type\": \"array\"\n    },\n    \"AbortIncompleteMultipartUpload\": {\n \
  \     \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-rest-lifecycle-rule-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: LifecycleRule
---
