---
description: ListVaultsOutput schema from api
layout: schema
name: ListVaultsOutput
properties_list:
- description: ''
  name: VaultList
  type: array
- description: ''
  name: Marker
  type: string
provider_name: Amazon S3 Glacier
provider_slug: amazon-s3-glacier
schema_file: json-schema/amazon-s3-glacier-api-list-vaults-output-schema.json
slug: amazon-s3-glacier-api-list-vaults-output
source_filename: amazon-s3-glacier-api-list-vaults-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/json-schema/amazon-s3-glacier-api-list-vaults-output-schema.json\",\n  \"title\": \"ListVaultsOutput\",\n  \"description\": \"ListVaultsOutput schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VaultList\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DescribeVaultOutput\"\n      }\n    },\n    \"Marker\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-s3-glacier/refs/heads/main/json-schema/amazon-s3-glacier-api-list-vaults-output-schema.json
tags:
- Archive
- Backup
- Storage
title: ListVaultsOutput
---
