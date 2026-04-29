---
description: ''
layout: schema
name: PropertyAttributes
properties_list:
- description: The name of the property.
  name: name
  type: string
- description: The platform type (web, mobile, or edge).
  name: platform
  type: string
- description: A list of domains associated with the property.
  name: domains
  type: array
- description: Whether the property is enabled.
  name: enabled
  type: boolean
- description: Whether the property is in development mode.
  name: development
  type: boolean
- description: The default privacy setting.
  name: privacy
  type: string
- description: Whether SSL is enabled.
  name: ssl_enabled
  type: boolean
- description: Whether rule component sequencing is enabled.
  name: rule_component_sequencing_enabled
  type: boolean
- description: Whether undefined data element variables return empty strings.
  name: undefined_vars_return_empty
  type: boolean
- description: A unique token for the property.
  name: token
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-property-attributes-schema.json
slug: reactor-property-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PropertyAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the property.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform type (web, mobile, or edge).\"\n    },\n    \"domains\": {\n      \"type\": \"array\",\n      \"description\": \"A list of domains associated with the property.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the property is enabled.\"\n    },\n    \"development\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the property is in development mode.\"\n    },\n    \"privacy\": {\n      \"type\": \"string\",\n      \"description\": \"The default privacy setting.\"\n    },\n    \"ssl_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SSL is enabled.\"\
  \n    },\n    \"rule_component_sequencing_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether rule component sequencing is enabled.\"\n    },\n    \"undefined_vars_return_empty\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether undefined data element variables return empty strings.\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"A unique token for the property.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-property-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: PropertyAttributes
---
