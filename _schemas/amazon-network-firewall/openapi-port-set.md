---
description: A set of port ranges for use in the rules in a rule group.
layout: schema
name: PortSet
properties_list:
- description: ''
  name: Definition
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-port-set-schema.json
slug: openapi-port-set
source_filename: openapi-port-set-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-port-set-schema.json\",\n  \"title\": \"PortSet\",\n  \"description\": \"A set of port ranges for use in the rules in a rule group. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Definition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VariableDefinitionList\"\n        },\n        {\n          \"description\": \"The set of port ranges. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-port-set-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: PortSet
---
