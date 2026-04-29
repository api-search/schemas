---
description: Additional settings for a stateful rule. This is part of the <a>StatefulRule</a> configuration.
layout: schema
name: RuleOption
properties_list:
- description: ''
  name: Keyword
  type: object
- description: ''
  name: Settings
  type: object
provider_name: Amazon Network Firewall
provider_slug: amazon-network-firewall
schema_file: json-schema/openapi-rule-option-schema.json
slug: openapi-rule-option
source_filename: openapi-rule-option-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rule-option-schema.json\",\n  \"title\": \"RuleOption\",\n  \"description\": \"Additional settings for a stateful rule. This is part of the <a>StatefulRule</a> configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Keyword\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Keyword\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    },\n    \"Settings\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Settings\"\n        },\n        {\n          \"description\": \"<p/>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Keyword\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-network-firewall/refs/heads/main/json-schema/openapi-rule-option-schema.json
tags:
- AWS
- Firewall
- Intrusion Detection
- Network Security
- VPC
title: RuleOption
---
