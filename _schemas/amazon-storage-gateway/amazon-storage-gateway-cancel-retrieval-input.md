---
description: CancelRetrievalInput
layout: schema
name: CancelRetrievalInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: TapeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-cancel-retrieval-input-schema.json
slug: amazon-storage-gateway-cancel-retrieval-input
source_filename: amazon-storage-gateway-cancel-retrieval-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-cancel-retrieval-input-schema.json\",\n  \"title\": \"CancelRetrievalInput\",\n  \"description\": \"CancelRetrievalInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the virtual tape you want to cancel retrieval for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"TapeARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-cancel-retrieval-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CancelRetrievalInput
---
