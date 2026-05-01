---
description: A single stateless rule. This is used in <a>StatelessRulesAndCustomActions</a>.
layout: schema
name: StatelessRule
properties_list:
- description: ''
  name: RuleDefinition
  type: object
- description: ''
  name: Priority
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-stateless-rule-schema.json
slug: openapi-stateless-rule
source_filename: openapi-stateless-rule-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateless-rule-schema.json\",\n  \"title\": \"StatelessRule\",\n  \"description\": \"A single stateless rule. This is used in <a>StatelessRulesAndCustomActions</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RuleDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuleDefinition\"\n        },\n        {\n          \"description\": \"Defines the stateless 5-tuple packet inspection criteria and the action to take on a packet that matches the criteria. \"\n        }\n      ]\n    },\n    \"Priority\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Priority\"\n        },\n        {\n          \"description\": \"<p>Indicates the order in which to run this rule relative to all of the rules that are defined for a\
  \ stateless rule group. Network Firewall evaluates the rules in a rule group starting with the lowest priority setting. You must ensure that the priority settings are unique for the rule group. </p> <p>Each stateless rule group uses exactly one <code>StatelessRulesAndCustomActions</code> object, and each <code>StatelessRulesAndCustomActions</code> contains exactly one <code>StatelessRules</code> object. To ensure unique priority settings for your rule groups, set unique priorities for the stateless rules that you define inside any single <code>StatelessRules</code> object.</p> <p>You can change the priority settings of your rules at any time. To make it easier to insert rules later, number them so there's a wide range in between, for example use 100, 200, and so on. </p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RuleDefinition\",\n    \"Priority\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-stateless-rule-schema.json
tags:
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: StatelessRule
---
