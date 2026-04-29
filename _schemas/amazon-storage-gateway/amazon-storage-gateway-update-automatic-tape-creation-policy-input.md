---
description: UpdateAutomaticTapeCreationPolicyInput schema from Amazon Storage Gateway API
layout: schema
name: UpdateAutomaticTapeCreationPolicyInput
properties_list:
- description: ''
  name: AutomaticTapeCreationRules
  type: object
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-update-automatic-tape-creation-policy-input-schema.json
slug: amazon-storage-gateway-update-automatic-tape-creation-policy-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-automatic-tape-creation-policy-input-schema.json\",\n  \"title\": \"UpdateAutomaticTapeCreationPolicyInput\",\n  \"description\": \"UpdateAutomaticTapeCreationPolicyInput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutomaticTapeCreationRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomaticTapeCreationRules\"\n        },\n        {\n          \"description\": \"An automatic tape creation policy consists of a list of automatic tape creation rules. The rules determine when and how to automatically create new tapes.\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\n    }\n  },\n  \"required\": [\n    \"AutomaticTapeCreationRules\"\
  ,\n    \"GatewayARN\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-update-automatic-tape-creation-policy-input-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: UpdateAutomaticTapeCreationPolicyInput
---
