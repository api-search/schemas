---
description: ''
layout: schema
name: CreateTableRequest
properties_list:
- description: The name for the table.
  name: name
  type: string
- description: The format of the table. Currently only ICEBERG is supported.
  name: format
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-tables-create-table-request-schema.json
slug: amazon-s3-tables-create-table-request
source_filename: amazon-s3-tables-create-table-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTableRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name for the table.\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The format of the table. Currently only ICEBERG is supported.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-tables-create-table-request-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: CreateTableRequest
---
