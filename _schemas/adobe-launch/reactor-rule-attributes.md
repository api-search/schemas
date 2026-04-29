---
description: ''
layout: schema
name: RuleAttributes
properties_list:
- description: The human-readable name of the rule.
  name: name
  type: string
- description: Whether the rule is enabled.
  name: enabled
  type: boolean
- description: Whether the rule has been published.
  name: published
  type: boolean
- description: Whether the rule has unpublished changes.
  name: dirty
  type: boolean
- description: The current revision number.
  name: revision_number
  type: integer
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-rule-attributes-schema.json
slug: reactor-rule-attributes
source_filename: reactor-rule-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuleAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the rule.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rule is enabled.\"\n    },\n    \"published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rule has been published.\"\n    },\n    \"dirty\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rule has unpublished changes.\"\n    },\n    \"revision_number\": {\n      \"type\": \"integer\",\n      \"description\": \"The current revision number.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-rule-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: RuleAttributes
---
