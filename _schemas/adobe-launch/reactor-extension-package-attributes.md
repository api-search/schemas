---
description: ''
layout: schema
name: ExtensionPackageAttributes
properties_list:
- description: The unique name of the extension package.
  name: name
  type: string
- description: The human-readable display name.
  name: display_name
  type: string
- description: A description of the extension package.
  name: description
  type: string
- description: The current version.
  name: version
  type: string
- description: The platform the extension package supports.
  name: platform
  type: string
- description: ''
  name: author
  type: object
- description: ''
  name: availability
  type: string
- description: ''
  name: discontinued
  type: boolean
- description: ''
  name: status
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/reactor-extension-package-attributes-schema.json
slug: reactor-extension-package-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExtensionPackageAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the extension package.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the extension package.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The current version.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform the extension package supports.\"\n    },\n    \"author\": {\n      \"type\": \"object\"\n    },\n    \"availability\": {\n      \"type\": \"string\"\n    },\n    \"discontinued\": {\n      \"type\": \"boolean\"\n    },\n    \"status\": {\n      \"type\": \"\
  string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/reactor-extension-package-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: ExtensionPackageAttributes
---
