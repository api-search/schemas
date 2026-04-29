---
description: DeleteTapeArchiveInput
layout: schema
name: DeleteTapeArchiveInput
properties_list:
- description: ''
  name: TapeARN
  type: object
- description: ''
  name: BypassGovernanceRetention
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-delete-tape-archive-input-schema.json
slug: amazon-storage-gateway-delete-tape-archive-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-archive-input-schema.json\",\n  \"title\": \"DeleteTapeArchiveInput\",\n  \"description\": \"DeleteTapeArchiveInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TapeARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TapeARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the virtual tape to delete from the virtual tape shelf (VTS).\"\n        }\n      ]\n    },\n    \"BypassGovernanceRetention\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/boolean\"\n        },\n        {\n          \"description\": \"Set to <code>TRUE</code> to delete an archived tape that belongs to a custom pool with tape retention lock. Only archived tapes with tape retention\
  \ lock set to <code>governance</code> can be deleted. Archived tapes with tape retention lock set to <code>compliance</code> can't be deleted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TapeARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-delete-tape-archive-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: DeleteTapeArchiveInput
---
