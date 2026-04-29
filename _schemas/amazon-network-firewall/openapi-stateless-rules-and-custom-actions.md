---
description: Stateless inspection criteria. Each stateless rule group uses exactly one of these data types to define its stateless rules.
layout: schema
name: StatelessRulesAndCustomActions
properties_list:
- description: ''
  name: StatelessRules
  type: object
- description: ''
  name: CustomActions
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-stateless-rules-and-custom-actions-schema.json
slug: openapi-stateless-rules-and-custom-actions
source_filename: openapi-stateless-rules-and-custom-actions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateless-rules-and-custom-actions-schema.json\",\n  \"title\": \"StatelessRulesAndCustomActions\",\n  \"description\": \"Stateless inspection criteria. Each stateless rule group uses exactly one of these data types to define its stateless rules. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StatelessRules\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StatelessRules\"\n        },\n        {\n          \"description\": \"Defines the set of stateless rules for use in a stateless rule group. \"\n        }\n      ]\n    },\n    \"CustomActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CustomActions\"\n        },\n        {\n          \"description\": \"Defines an array of individual custom action definitions\
  \ that are available for use by the stateless rules in this <code>StatelessRulesAndCustomActions</code> specification. You name each custom action that you define, and then you can use it by name in your <a>StatelessRule</a> <a>RuleDefinition</a> <code>Actions</code> specification.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"StatelessRules\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateless-rules-and-custom-actions-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: StatelessRulesAndCustomActions
---
