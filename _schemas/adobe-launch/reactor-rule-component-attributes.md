---
description: ''
layout: schema
name: RuleComponentAttributes
properties_list:
- description: The human-readable name of the rule component.
  name: name
  type: string
- description: The descriptor ID identifying the component type from an extension package.
  name: delegate_descriptor_id
  type: string
- description: The execution order within its type group.
  name: order
  type: integer
- description: The order relative to other components in the rule.
  name: rule_order
  type: number
- description: A JSON-encoded string of settings for the component.
  name: settings
  type: string
- description: Timeout in milliseconds for the component.
  name: timeout
  type: integer
- description: Whether to delay the next action.
  name: delay_next
  type: boolean
- description: Whether to negate the condition result.
  name: negate
  type: boolean
- description: Whether the rule component is enabled.
  name: enabled
  type: boolean
- description: ''
  name: published
  type: boolean
- description: ''
  name: dirty
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-rule-component-attributes-schema.json
slug: reactor-rule-component-attributes
source_filename: reactor-rule-component-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RuleComponentAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable name of the rule component.\"\n    },\n    \"delegate_descriptor_id\": {\n      \"type\": \"string\",\n      \"description\": \"The descriptor ID identifying the component type from an extension package.\"\n    },\n    \"order\": {\n      \"type\": \"integer\",\n      \"description\": \"The execution order within its type group.\"\n    },\n    \"rule_order\": {\n      \"type\": \"number\",\n      \"description\": \"The order relative to other components in the rule.\"\n    },\n    \"settings\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON-encoded string of settings for the component.\"\n    },\n    \"timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Timeout in milliseconds for the component.\"\
  \n    },\n    \"delay_next\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to delay the next action.\"\n    },\n    \"negate\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to negate the condition result.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the rule component is enabled.\"\n    },\n    \"published\": {\n      \"type\": \"boolean\"\n    },\n    \"dirty\": {\n      \"type\": \"boolean\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-rule-component-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: RuleComponentAttributes
---
