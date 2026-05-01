---
description: DeleteTapeOutput
layout: schema
name: DeleteTapeOutput
properties_list:
- description: ''
  name: TapeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-tape-output-schema.json
slug: amazon-storage-gateway-delete-tape-output
source_filename: amazon-storage-gateway-delete-tape-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-output-schema.json\",\n  \"title\": \"DeleteTapeOutput\",\n  \"description\": \"DeleteTapeOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the deleted virtual tape.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteTapeOutput
---
