---
description: RetrieveTapeRecoveryPointInput
layout: schema
name: RetrieveTapeRecoveryPointInput
properties_list:
- description: ''
  name: TapeARN
  type: object
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-retrieve-tape-recovery-point-input-schema.json
slug: amazon-storage-gateway-retrieve-tape-recovery-point-input
source_filename: amazon-storage-gateway-retrieve-tape-recovery-point-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-retrieve-tape-recovery-point-input-schema.json\",\n  \"title\": \"RetrieveTapeRecoveryPointInput\",\n  \"description\": \"RetrieveTapeRecoveryPointInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the virtual tape for which you want to retrieve the recovery point.\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    }\n  },\n  \"required\": [\n    \"TapeARN\",\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-retrieve-tape-recovery-point-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: RetrieveTapeRecoveryPointInput
---
