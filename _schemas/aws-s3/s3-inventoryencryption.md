---
description: Contains the type of server-side encryption used to encrypt the inventory results.
layout: schema
name: InventoryEncryption
properties_list:
- description: ''
  name: SSES3
  type: object
- description: ''
  name: SSEKMS
  type: object
provider_name: Amazon S3 API
provider_slug: aws-s3
schema_file: json-schema/s3-inventoryencryption-schema.json
slug: s3-inventoryencryption
source_filename: s3-inventoryencryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"InventoryEncryption\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SSES3\": {},\n    \"SSEKMS\": {}\n  },\n  \"description\": \"Contains the type of server-side encryption used to encrypt the inventory results.\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aws-s3/refs/heads/main/json-schema/s3-inventoryencryption-schema.json
tags:
- AWS
- Cloud Storage
- Object Storage
- Storage
title: InventoryEncryption
---
