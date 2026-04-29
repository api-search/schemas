---
description: Identifier for a single stateless rule group, used in a firewall policy to refer to the rule group.
layout: schema
name: StatelessRuleGroupReference
properties_list:
- description: ''
  name: ResourceArn
  type: object
- description: ''
  name: Priority
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-stateless-rule-group-reference-schema.json
slug: openapi-stateless-rule-group-reference
source_filename: openapi-stateless-rule-group-reference-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateless-rule-group-reference-schema.json\",\n  \"title\": \"StatelessRuleGroupReference\",\n  \"description\": \"Identifier for a single stateless rule group, used in a firewall policy to refer to the rule group. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the stateless rule group.\"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"An integer setting that indicates the order in which to run the stateless rule groups in a single <a>FirewallPolicy</a>.\
  \ Network Firewall applies each stateless rule group to a packet starting with the group that has the lowest priority setting. You must ensure that the priority settings are unique within each policy.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceArn\",\n    \"Priority\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateless-rule-group-reference-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: StatelessRuleGroupReference
---
