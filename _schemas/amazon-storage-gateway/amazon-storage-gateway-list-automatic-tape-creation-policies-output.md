---
description: ListAutomaticTapeCreationPoliciesOutput schema from Amazon Storage Gateway API
layout: schema
name: ListAutomaticTapeCreationPoliciesOutput
properties_list:
- description: ''
  name: AutomaticTapeCreationPolicyInfos
  type: object
provider_name: Amazon Storage Gateway
provider_slug: amazon-storage-gateway
schema_file: json-schema/amazon-storage-gateway-list-automatic-tape-creation-policies-output-schema.json
slug: amazon-storage-gateway-list-automatic-tape-creation-policies-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-automatic-tape-creation-policies-output-schema.json\",\n  \"title\": \"ListAutomaticTapeCreationPoliciesOutput\",\n  \"description\": \"ListAutomaticTapeCreationPoliciesOutput schema from Amazon Storage Gateway API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AutomaticTapeCreationPolicyInfos\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AutomaticTapeCreationPolicyInfos\"\n        },\n        {\n          \"description\": \"Gets a listing of information about the gateway's automatic tape creation policies, including the automatic tape creation rules and the gateway that is using the policies.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-storage-gateway/refs/heads/main/json-schema/amazon-storage-gateway-list-automatic-tape-creation-policies-output-schema.json
tags:
- AWS
- Backup
- File Storage
- Gateway
- Hybrid Cloud
- Storage
title: ListAutomaticTapeCreationPoliciesOutput
---
