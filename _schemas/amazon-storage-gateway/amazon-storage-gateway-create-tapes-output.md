---
description: CreateTapeOutput
layout: schema
name: CreateTapesOutput
properties_list:
- description: ''
  name: TapeARNs
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-tapes-output-schema.json
slug: amazon-storage-gateway-create-tapes-output
source_filename: amazon-storage-gateway-create-tapes-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tapes-output-schema.json\",\n  \"title\": \"CreateTapesOutput\",\n  \"description\": \"CreateTapeOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARNs\"\n        },\n        {\n          \"description\": \"A list of unique Amazon Resource Names (ARNs) that represents the virtual tapes that were created.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tapes-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateTapesOutput
---
