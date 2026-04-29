---
description: ''
layout: schema
name: SSESpecification
properties_list:
- description: Indicates whether server-side encryption is enabled
  name: Enabled
  type: boolean
- description: Server-side encryption type
  name: SSEType
  type: string
- description: The KMS key that should be used for server-side encryption
  name: KMSMasterKeyId
  type: string
provider_name: Amazon DynamoDB
provider_slug: dynamodb
schema_file: json-schema/dynamodb-sse-specification-schema.json
slug: dynamodb-sse-specification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SSESpecification\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether server-side encryption is enabled\"\n    },\n    \"SSEType\": {\n      \"type\": \"string\",\n      \"description\": \"Server-side encryption type\"\n    },\n    \"KMSMasterKeyId\": {\n      \"type\": \"string\",\n      \"description\": \"The KMS key that should be used for server-side encryption\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynamodb/refs/heads/main/json-schema/dynamodb-sse-specification-schema.json
tags:
- AWS
- Cloud
- Database
- Document Store
- Key-Value
- Managed Service
- NoSQL
- Serverless
title: SSESpecification
---
