---
description: DescribeFileSystemsResponse schema from Amazon EFS Amazon Elastic File System (EFS) API
layout: schema
name: DescribeFileSystemsResponse
properties_list:
- description: ''
  name: FileSystems
  type: array
- description: ''
  name: Marker
  type: string
- description: ''
  name: NextMarker
  type: string
provider_name: Amazon EFS
provider_slug: amazon-efs
schema_file: json-schema/efs-openapi-describe-file-systems-response-schema.json
slug: efs-openapi-describe-file-systems-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/json-schema/efs-openapi-describe-file-systems-response-schema.json\",\n  \"title\": \"DescribeFileSystemsResponse\",\n  \"description\": \"DescribeFileSystemsResponse schema from Amazon EFS Amazon Elastic File System (EFS) API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FileSystems\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FileSystem\"\n      }\n    },\n    \"Marker\": {\n      \"type\": \"string\"\n    },\n    \"NextMarker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-efs/refs/heads/main/json-schema/efs-openapi-describe-file-systems-response-schema.json
tags:
- Amazon Web Services
- AWS
- EFS
- Elastic File System
- File Storage
- NFS
- Serverless
- Storage
title: DescribeFileSystemsResponse
---
