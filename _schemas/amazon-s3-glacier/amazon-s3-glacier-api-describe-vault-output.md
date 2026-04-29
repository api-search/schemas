---
description: DescribeVaultOutput schema from api
layout: schema
name: DescribeVaultOutput
properties_list:
- description: ''
  name: VaultARN
  type: string
- description: ''
  name: VaultName
  type: string
- description: ''
  name: CreationDate
  type: string
- description: ''
  name: LastInventoryDate
  type: string
- description: ''
  name: NumberOfArchives
  type: integer
- description: ''
  name: SizeInBytes
  type: integer
provider_name: Amazon S3 Glacier
provider_slug: amazon-s3-glacier
schema_file: json-schema/amazon-s3-glacier-api-describe-vault-output-schema.json
slug: amazon-s3-glacier-api-describe-vault-output
source_filename: amazon-s3-glacier-api-describe-vault-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/json-schema/amazon-s3-glacier-api-describe-vault-output-schema.json\",\n  \"title\": \"DescribeVaultOutput\",\n  \"description\": \"DescribeVaultOutput schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VaultARN\": {\n      \"type\": \"string\"\n    },\n    \"VaultName\": {\n      \"type\": \"string\"\n    },\n    \"CreationDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"LastInventoryDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"NumberOfArchives\": {\n      \"type\": \"integer\"\n    },\n    \"SizeInBytes\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/json-schema/amazon-s3-glacier-api-describe-vault-output-schema.json
tags:
- Archive
- AWS
- Backup
- Storage
title: DescribeVaultOutput
---
