---
description: RetrieveTapeArchiveOutput
layout: schema
name: RetrieveTapeArchiveOutput
properties_list:
- description: ''
  name: TapeARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-retrieve-tape-archive-output-schema.json
slug: amazon-storage-gateway-retrieve-tape-archive-output
source_filename: amazon-storage-gateway-retrieve-tape-archive-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-retrieve-tape-archive-output-schema.json\",\n  \"title\": \"RetrieveTapeArchiveOutput\",\n  \"description\": \"RetrieveTapeArchiveOutput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the retrieved virtual tape.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-retrieve-tape-archive-output-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: RetrieveTapeArchiveOutput
---
