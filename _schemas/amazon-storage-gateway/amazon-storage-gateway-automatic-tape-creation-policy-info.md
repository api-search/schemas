---
description: Information about the gateway's automatic tape creation policies, including the automatic tape creation rules and the gateway that is using the policies.
layout: schema
name: AutomaticTapeCreationPolicyInfo
properties_list:
- description: ''
  name: AutomaticTapeCreationRules
  type: object
- description: ''
  name: GatewayARN
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-automatic-tape-creation-policy-info-schema.json
slug: amazon-storage-gateway-automatic-tape-creation-policy-info
source_filename: amazon-storage-gateway-automatic-tape-creation-policy-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-automatic-tape-creation-policy-info-schema.json\",\n  \"title\": \"AutomaticTapeCreationPolicyInfo\",\n  \"description\": \"Information about the gateway's automatic tape creation policies, including the automatic tape creation rules and the gateway that is using the policies.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutomaticTapeCreationRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomaticTapeCreationRules\"\n        },\n        {\n          \"description\": \"An automatic tape creation policy consists of a list of automatic tape creation rules. This returns the rules that determine when and how to automatically create new tapes.\"\n        }\n      ]\n    },\n    \"GatewayARN\": {\n      \"$ref\": \"#/components/schemas/GatewayARN\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-automatic-tape-creation-policy-info-schema.json
tags:
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: AutomaticTapeCreationPolicyInfo
---
