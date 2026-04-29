---
description: ''
layout: schema
name: NamespaceDetail
properties_list:
- description: ''
  name: namespace
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: createdBy
  type: string
- description: ''
  name: ownerAccountId
  type: string
- description: ''
  name: tableBucketARN
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-tables-namespace-detail-schema.json
slug: amazon-s3-tables-namespace-detail
source_filename: amazon-s3-tables-namespace-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NamespaceDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"array\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\"\n    },\n    \"ownerAccountId\": {\n      \"type\": \"string\"\n    },\n    \"tableBucketARN\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-tables-namespace-detail-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: NamespaceDetail
---
