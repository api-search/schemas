---
description: The <code>TestRoleRequest</code> structure.
layout: schema
name: TestRoleRequest
properties_list:
- description: ''
  name: Role
  type: object
- description: ''
  name: InputBucket
  type: object
- description: ''
  name: OutputBucket
  type: object
- description: ''
  name: Topics
  type: object
provider_name: Amazon Elastic Transcoder
provider_slug: amazon-elastic-transcoder
schema_file: json-schema/amazon-elastic-transcoder-test-role-request-schema.json
slug: amazon-elastic-transcoder-test-role-request
source_filename: amazon-elastic-transcoder-test-role-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-test-role-request-schema.json\",\n  \"title\": \"TestRoleRequest\",\n  \"description\": \" The <code>TestRoleRequest</code> structure. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Role\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Role\"\n        },\n        {\n          \"description\": \"The IAM Amazon Resource Name (ARN) for the role that you want Elastic Transcoder to test.\"\n        }\n      ]\n    },\n    \"InputBucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket that contains media files to be transcoded. The action attempts to read from this bucket.\"\n        }\n      ]\n    },\n    \"OutputBucket\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BucketName\"\n        },\n        {\n          \"description\": \"The Amazon S3 bucket that Elastic Transcoder writes transcoded media files to. The action attempts to read from this bucket.\"\n        }\n      ]\n    },\n    \"Topics\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SnsTopics\"\n        },\n        {\n          \"description\": \"The ARNs of one or more Amazon Simple Notification Service (Amazon SNS) topics that you want the action to send a test notification to.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Role\",\n    \"InputBucket\",\n    \"OutputBucket\",\n    \"Topics\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-elastic-transcoder/refs/heads/main/json-schema/amazon-elastic-transcoder-test-role-request-schema.json
tags:
- Amazon Web Services
- AWS
- Media
- Transcoding
- Video
title: TestRoleRequest
---
