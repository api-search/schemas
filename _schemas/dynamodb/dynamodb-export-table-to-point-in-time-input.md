---
description: ''
layout: schema
name: ExportTableToPointInTimeInput
properties_list:
- description: ARN of the table to export
  name: TableArn
  type: string
- description: Time in the past from which to export table data
  name: ExportTime
  type: string
- description: Idempotency token
  name: ClientToken
  type: string
- description: Name of the S3 bucket to export to
  name: S3Bucket
  type: string
- description: Account ID of the S3 bucket owner
  name: S3BucketOwner
  type: string
- description: S3 key prefix for the export
  name: S3Prefix
  type: string
- description: ''
  name: S3SseAlgorithm
  type: string
- description: ''
  name: S3SseKmsKeyId
  type: string
- description: ''
  name: ExportFormat
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-export-table-to-point-in-time-input-schema.json
slug: dynamodb-export-table-to-point-in-time-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExportTableToPointInTimeInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TableArn\": {\n      \"type\": \"string\",\n      \"description\": \"ARN of the table to export\"\n    },\n    \"ExportTime\": {\n      \"type\": \"string\",\n      \"description\": \"Time in the past from which to export table data\"\n    },\n    \"ClientToken\": {\n      \"type\": \"string\",\n      \"description\": \"Idempotency token\"\n    },\n    \"S3Bucket\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the S3 bucket to export to\"\n    },\n    \"S3BucketOwner\": {\n      \"type\": \"string\",\n      \"description\": \"Account ID of the S3 bucket owner\"\n    },\n    \"S3Prefix\": {\n      \"type\": \"string\",\n      \"description\": \"S3 key prefix for the export\"\n    },\n    \"S3SseAlgorithm\": {\n      \"type\": \"string\"\n    },\n    \"S3SseKmsKeyId\": {\n      \"type\": \"\
  string\"\n    },\n    \"ExportFormat\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-export-table-to-point-in-time-input-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: ExportTableToPointInTimeInput
---
