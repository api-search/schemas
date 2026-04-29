---
description: CreateTapePoolOutput schema from Amazon Storage Gateway API
layout: schema
name: CreateTapePoolOutput
properties_list:
- description: ''
  name: PoolARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-create-tape-pool-output-schema.json
slug: amazon-storage-gateway-create-tape-pool-output
source_filename: amazon-storage-gateway-create-tape-pool-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tape-pool-output-schema.json\",\n  \"title\": \"CreateTapePoolOutput\",\n  \"description\": \"CreateTapePoolOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PoolARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolARN\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) that represents the custom tape pool. Use the <a>ListTapePools</a> operation to return a list of tape pools for your account and Amazon Web Services Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-create-tape-pool-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: CreateTapePoolOutput
---
