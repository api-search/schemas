---
description: ''
layout: schema
name: TableDetail
properties_list:
- description: The name of the table.
  name: name
  type: string
- description: The Amazon Resource Name (ARN) of the table.
  name: tableARN
  type: string
- description: ''
  name: namespace
  type: array
- description: The version token of the table.
  name: versionToken
  type: string
- description: The S3 URI location of the table metadata.
  name: metadataLocation
  type: string
- description: The S3 URI of the warehouse location for the table.
  name: warehouseLocation
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: createdBy
  type: string
- description: ''
  name: modifiedAt
  type: string
- description: ''
  name: modifiedBy
  type: string
- description: ''
  name: managedByService
  type: string
- description: ''
  name: ownerAccountId
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: format
  type: string
provider_name: Amazon S3
provider_slug: amazon-s3
schema_file: json-schema/amazon-s3-tables-table-detail-schema.json
slug: amazon-s3-tables-table-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TableDetail\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the table.\"\n    },\n    \"tableARN\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the table.\"\n    },\n    \"namespace\": {\n      \"type\": \"array\"\n    },\n    \"versionToken\": {\n      \"type\": \"string\",\n      \"description\": \"The version token of the table.\"\n    },\n    \"metadataLocation\": {\n      \"type\": \"string\",\n      \"description\": \"The S3 URI location of the table metadata.\"\n    },\n    \"warehouseLocation\": {\n      \"type\": \"string\",\n      \"description\": \"The S3 URI of the warehouse location for the table.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"createdBy\": {\n      \"type\": \"string\"\n    },\n    \"modifiedAt\": {\n   \
  \   \"type\": \"string\"\n    },\n    \"modifiedBy\": {\n      \"type\": \"string\"\n    },\n    \"managedByService\": {\n      \"type\": \"string\"\n    },\n    \"ownerAccountId\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"format\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3/refs/heads/main/json-schema/amazon-s3-tables-table-detail-schema.json
tags:
- Archive
- AWS
- Backup
- Cloud Storage
- Data Storage
- Object Storage
- Scalable Storage
title: TableDetail
---
