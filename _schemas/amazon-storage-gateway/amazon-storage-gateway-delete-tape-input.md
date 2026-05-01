---
description: DeleteTapeInput
layout: schema
name: DeleteTapeInput
properties_list:
- description: ''
  name: GatewayARN
  type: object
- description: ''
  name: TapeARN
  type: object
- description: ''
  name: BypassGovernanceRetention
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-tape-input-schema.json
slug: amazon-storage-gateway-delete-tape-input
source_filename: amazon-storage-gateway-delete-tape-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-input-schema.json\",\n  \"title\": \"DeleteTapeInput\",\n  \"description\": \"DeleteTapeInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GatewayARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GatewayARN\"\n        },\n        {\n          \"description\": \"The unique Amazon Resource Name (ARN) of the gateway that the virtual tape to delete is associated with. Use the <a>ListGateways</a> operation to return a list of gateways for your account and Amazon Web Services Region.\"\n        }\n      ]\n    },\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the virtual tape to delete.\"\
  \n        }\n      ]\n    },\n    \"BypassGovernanceRetention\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"Set to <code>TRUE</code> to delete an archived tape that belongs to a custom pool with tape retention lock. Only archived tapes with tape retention lock set to <code>governance</code> can be deleted. Archived tapes with tape retention lock set to <code>compliance</code> can't be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GatewayARN\",\n    \"TapeARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-input-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteTapeInput
---
