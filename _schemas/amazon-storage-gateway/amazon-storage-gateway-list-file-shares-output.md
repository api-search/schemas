---
description: ListFileShareOutput
layout: schema
name: ListFileSharesOutput
properties_list:
- description: ''
  name: Marker
  type: object
- description: ''
  name: NextMarker
  type: object
- description: ''
  name: FileShareInfoList
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-file-shares-output-schema.json
slug: amazon-storage-gateway-list-file-shares-output
source_filename: amazon-storage-gateway-list-file-shares-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-file-shares-output-schema.json\",\n  \"title\": \"ListFileSharesOutput\",\n  \"description\": \"ListFileShareOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"If the request includes <code>Marker</code>, the response returns that value in this field.\"\n        }\n      ]\n    },\n    \"NextMarker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"If a value is present, there are more file shares to return. In a subsequent request, use <code>NextMarker</code> as the value for <code>Marker</code> to retrieve the next set\
  \ of file shares.\"\n        }\n      ]\n    },\n    \"FileShareInfoList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FileShareInfoList\"\n        },\n        {\n          \"description\": \"An array of information about the S3 File Gateway's file shares.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-file-shares-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListFileSharesOutput
---
