---
description: ''
layout: schema
name: ListTableBucketsResponse
properties_list:
- description: ''
  name: tableBuckets
  type: array
- description: A continuation token for paginating the list.
  name: continuationToken
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-tables-list-table-buckets-response-schema.json
slug: amazon-s3-tables-list-table-buckets-response
source_filename: amazon-s3-tables-list-table-buckets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ListTableBucketsResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tableBuckets\": {\n      \"type\": \"array\"\n    },\n    \"continuationToken\": {\n      \"type\": \"string\",\n      \"description\": \"A continuation token for paginating the list.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-tables-list-table-buckets-response-schema.json
tags:
- Archive
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: ListTableBucketsResponse
---
