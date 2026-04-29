---
description: DeleteTapeArchiveOutput
layout: schema
name: DeleteTapeArchiveOutput
properties_list:
- description: ''
  name: TapeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-tape-archive-output-schema.json
slug: amazon-storage-gateway-delete-tape-archive-output
source_filename: amazon-storage-gateway-delete-tape-archive-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-archive-output-schema.json\",\n  \"title\": \"DeleteTapeArchiveOutput\",\n  \"description\": \"DeleteTapeArchiveOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the virtual tape that was deleted from the virtual tape shelf (VTS).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-archive-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteTapeArchiveOutput
---
