---
description: ''
layout: schema
name: TableSummary
properties_list:
- description: ''
  name: namespace
  type: array
- description: The name of the table.
  name: name
  type: string
- description: The type of the table.
  name: type
  type: string
- description: The Amazon Resource Name (ARN) of the table.
  name: tableARN
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: modifiedAt
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-tables-table-summary-schema.json
slug: amazon-s3-tables-table-summary
source_filename: amazon-s3-tables-table-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"namespace\": {\n      \"type\": \"array\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the table.\"\n    },\n    \"tableARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the table.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-tables-table-summary-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: TableSummary
---
