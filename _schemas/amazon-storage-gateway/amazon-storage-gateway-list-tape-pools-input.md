---
description: ListTapePoolsInput schema from Amazon Storage Gateway API
layout: schema
name: ListTapePoolsInput
properties_list:
- description: ''
  name: PoolARNs
  type: object
- description: ''
  name: Marker
  type: object
- description: ''
  name: Limit
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-tape-pools-input-schema.json
slug: amazon-storage-gateway-list-tape-pools-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-tape-pools-input-schema.json\",\n  \"title\": \"ListTapePoolsInput\",\n  \"description\": \"ListTapePoolsInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PoolARNs\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolARNs\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of each of the custom tape pools you want to list. If you don't specify a custom tape pool ARN, the response lists all custom tape pools. \"\n        }\n      ]\n    },\n    \"Marker\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Marker\"\n        },\n        {\n          \"description\": \"A string that indicates the position at which to begin the returned\
  \ list of tape pools.\"\n        }\n      ]\n    },\n    \"Limit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveIntObject\"\n        },\n        {\n          \"description\": \"An optional number limit for the tape pools in the list returned by this call.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-tape-pools-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListTapePoolsInput
---
