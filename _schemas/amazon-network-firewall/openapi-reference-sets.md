---
description: Contains a set of IP set references.
layout: schema
name: ReferenceSets
properties_list:
- description: ''
  name: IPSetReferences
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-reference-sets-schema.json
slug: openapi-reference-sets
source_filename: openapi-reference-sets-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-reference-sets-schema.json\",\n  \"title\": \"ReferenceSets\",\n  \"description\": \"Contains a set of IP set references.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IPSetReferences\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IPSetReferenceMap\"\n        },\n        {\n          \"description\": \"The list of IP set references.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-reference-sets-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: ReferenceSets
---
