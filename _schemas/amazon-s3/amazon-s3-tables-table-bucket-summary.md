---
description: ''
layout: schema
name: TableBucketSummary
properties_list:
- description: The Amazon Resource Name (ARN) of the table bucket.
  name: arn
  type: string
- description: The name of the table bucket.
  name: name
  type: string
- description: The account ID of the owner of the table bucket.
  name: ownerAccountId
  type: string
- description: The date and time when the table bucket was created.
  name: createdAt
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-tables-table-bucket-summary-schema.json
slug: amazon-s3-tables-table-bucket-summary
source_filename: amazon-s3-tables-table-bucket-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableBucketSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the table bucket.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table bucket.\"\n    },\n    \"ownerAccountId\": {\n      \"type\": \"string\",\n      \"description\": \"The account ID of the owner of the table bucket.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the table bucket was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-tables-table-bucket-summary-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: TableBucketSummary
---
