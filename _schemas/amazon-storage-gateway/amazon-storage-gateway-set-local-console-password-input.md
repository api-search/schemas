---
description: SetLocalConsolePasswordInput
layout: schema
name: SetLocalConsolePasswordInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: LocalConsolePassword
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-set-local-console-password-input-schema.json
slug: amazon-storage-gateway-set-local-console-password-input
source_filename: amazon-storage-gateway-set-local-console-password-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-set-local-console-password-input-schema.json\",\n  \"title\": \"SetLocalConsolePasswordInput\",\n  \"description\": \"SetLocalConsolePasswordInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    },\n    \"LocalConsolePassword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocalConsolePassword\"\n        },\n        {\n          \"description\": \"The password you want to set for your VM local console.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"LocalConsolePassword\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-set-local-console-password-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: SetLocalConsolePasswordInput
---
