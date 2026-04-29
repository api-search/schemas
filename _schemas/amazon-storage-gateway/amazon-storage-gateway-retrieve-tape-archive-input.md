---
description: RetrieveTapeArchiveInput
layout: schema
name: RetrieveTapeArchiveInput
properties_list:
- description: ''
  name: TapeARN
  type: object
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-retrieve-tape-archive-input-schema.json
slug: amazon-storage-gateway-retrieve-tape-archive-input
source_filename: amazon-storage-gateway-retrieve-tape-archive-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-retrieve-tape-archive-input-schema.json\",\n  \"title\": \"RetrieveTapeArchiveInput\",\n  \"description\": \"RetrieveTapeArchiveInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the virtual tape you want to retrieve from the virtual tape shelf (VTS).\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the gateway you want to retrieve the virtual tape to. Use the <a>ListGateways</a> operation to return a\
  \ list of gateways for your account and Amazon Web Services Region.</p> <p>You retrieve archived virtual tapes to only one gateway and the gateway must be a tape gateway.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TapeARN\",\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-retrieve-tape-archive-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: RetrieveTapeArchiveInput
---
