---
description: ''
layout: schema
name: PropertyAttributes
properties_list:
- description: ''
  name: name
  type: string
- description: Always edge for event forwarding properties.
  name: platform
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/event-forwarding-property-attributes-schema.json
slug: event-forwarding-property-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PropertyAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"Always edge for event forwarding properties.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/event-forwarding-property-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: PropertyAttributes
---
