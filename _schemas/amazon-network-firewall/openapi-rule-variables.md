---
description: Settings that are available for use in the rules in the <a>RuleGroup</a> where this is defined.
layout: schema
name: RuleVariables
properties_list:
- description: ''
  name: IPSets
  type: object
- description: ''
  name: PortSets
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-rule-variables-schema.json
slug: openapi-rule-variables
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rule-variables-schema.json\",\n  \"title\": \"RuleVariables\",\n  \"description\": \"Settings that are available for use in the rules in the <a>RuleGroup</a> where this is defined. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"IPSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IPSets\"\n        },\n        {\n          \"description\": \"A list of IP addresses and address ranges, in CIDR notation. \"\n        }\n      ]\n    },\n    \"PortSets\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PortSets\"\n        },\n        {\n          \"description\": \"A list of port ranges. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rule-variables-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: RuleVariables
---
