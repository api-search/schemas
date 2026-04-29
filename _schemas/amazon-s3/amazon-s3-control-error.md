---
description: ''
layout: schema
name: Error
properties_list:
- description: ''
  name: Code
  type: string
- description: ''
  name: Message
  type: string
- description: ''
  name: Resource
  type: string
- description: ''
  name: RequestId
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-control-error-schema.json
slug: amazon-s3-control-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Code\": {\n      \"type\": \"string\"\n    },\n    \"Message\": {\n      \"type\": \"string\"\n    },\n    \"Resource\": {\n      \"type\": \"string\"\n    },\n    \"RequestId\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-control-error-schema.json
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
