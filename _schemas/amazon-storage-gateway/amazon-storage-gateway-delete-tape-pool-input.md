---
description: DeleteTapePoolInput schema from Amazon Storage Gateway API
layout: schema
name: DeleteTapePoolInput
properties_list:
- description: ''
  name: PoolARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-tape-pool-input-schema.json
slug: amazon-storage-gateway-delete-tape-pool-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-pool-input-schema.json\",\n  \"title\": \"DeleteTapePoolInput\",\n  \"description\": \"DeleteTapePoolInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PoolARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PoolARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the custom tape pool to delete.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PoolARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-pool-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteTapePoolInput
---
