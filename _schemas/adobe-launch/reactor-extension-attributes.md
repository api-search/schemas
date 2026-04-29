---
description: ''
layout: schema
name: ExtensionAttributes
properties_list:
- description: The unique name of the extension.
  name: name
  type: string
- description: The human-readable display name.
  name: display_name
  type: string
- description: The version of the installed extension.
  name: version
  type: string
- description: The descriptor ID for the extension configuration.
  name: delegate_descriptor_id
  type: string
- description: A JSON-encoded string of settings.
  name: settings
  type: string
- description: Whether the extension is enabled.
  name: enabled
  type: boolean
- description: ''
  name: published
  type: boolean
- description: ''
  name: dirty
  type: boolean
- description: ''
  name: revision_number
  type: integer
- description: When the extension was deleted, if applicable.
  name: deleted_at
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-extension-attributes-schema.json
slug: reactor-extension-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExtensionAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the extension.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The version of the installed extension.\"\n    },\n    \"delegate_descriptor_id\": {\n      \"type\": \"string\",\n      \"description\": \"The descriptor ID for the extension configuration.\"\n    },\n    \"settings\": {\n      \"type\": \"string\",\n      \"description\": \"A JSON-encoded string of settings.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the extension is enabled.\"\n    },\n    \"published\": {\n      \"type\": \"boolean\"\n    },\n    \"dirty\": {\n\
  \      \"type\": \"boolean\"\n    },\n    \"revision_number\": {\n      \"type\": \"integer\"\n    },\n    \"deleted_at\": {\n      \"type\": \"string\",\n      \"description\": \"When the extension was deleted, if applicable.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-extension-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: ExtensionAttributes
---
