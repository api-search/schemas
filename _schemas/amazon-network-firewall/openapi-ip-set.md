---
description: A list of IP addresses and address ranges, in CIDR notation. This is part of a <a>RuleVariables</a>.
layout: schema
name: IPSet
properties_list:
- description: ''
  name: Definition
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-ip-set-schema.json
slug: openapi-ip-set
source_filename: openapi-ip-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-ip-set-schema.json\",\n  \"title\": \"IPSet\",\n  \"description\": \"A list of IP addresses and address ranges, in CIDR notation. This is part of a <a>RuleVariables</a>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VariableDefinitionList\"\n        },\n        {\n          \"description\": \"The list of IP addresses and address ranges, in CIDR notation. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Definition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-ip-set-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: IPSet
---
