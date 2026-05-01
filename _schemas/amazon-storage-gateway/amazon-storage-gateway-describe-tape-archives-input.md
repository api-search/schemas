---
description: DescribeTapeArchivesInput
layout: schema
name: DescribeTapeArchivesInput
properties_list:
- description: ''
  name: TapeARNs
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: Limit
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-describe-tape-archives-input-schema.json
slug: amazon-storage-gateway-describe-tape-archives-input
source_filename: amazon-storage-gateway-describe-tape-archives-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tape-archives-input-schema.json\",\n  \"title\": \"DescribeTapeArchivesInput\",\n  \"description\": \"DescribeTapeArchivesInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARNs\"\n        },\n        {\n          \"description\": \"Specifies one or more unique Amazon Resource Names (ARNs) that represent the virtual tapes you want to describe.\"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"An opaque string that indicates the position at which to begin describing virtual tapes.\"\n        }\n      ]\n    },\n    \"Limit\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveIntObject\"\n        },\n        {\n          \"description\": \"Specifies that the number of virtual tapes described be limited to the specified number.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-describe-tape-archives-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DescribeTapeArchivesInput
---
