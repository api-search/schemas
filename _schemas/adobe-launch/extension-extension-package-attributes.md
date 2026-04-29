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
- description: A description of the extension package capabilities.
  name: description
  type: string
- description: The current version using semantic versioning.
  name: version
  type: string
- description: The platform the extension supports.
  name: platform
  type: string
- description: Information about the extension package author.
  name: author
  type: object
- description: The availability level of the extension package.
  name: availability
  type: string
- description: Whether the extension package has been discontinued.
  name: discontinued
  type: boolean
- description: The current processing status.
  name: status
  type: string
- description: The URL on Adobe Exchange for public extensions.
  name: exchange_url
  type: string
- description: Path to the extension icon within the package.
  name: icon_path
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: Adobe Launch
provider_slug: adobe-launch
schema_file: json-schema/extension-extension-package-attributes-schema.json
slug: extension-extension-package-attributes
source_filename: extension-extension-package-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExtensionPackageAttributes\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name of the extension package.\"\n    },\n    \"display_name\": {\n      \"type\": \"string\",\n      \"description\": \"The human-readable display name.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the extension package capabilities.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"The current version using semantic versioning.\"\n    },\n    \"platform\": {\n      \"type\": \"string\",\n      \"description\": \"The platform the extension supports.\"\n    },\n    \"author\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the extension package author.\"\n    },\n    \"availability\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The availability level of the extension package.\"\n    },\n    \"discontinued\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the extension package has been discontinued.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current processing status.\"\n    },\n    \"exchange_url\": {\n      \"type\": \"string\",\n      \"description\": \"The URL on Adobe Exchange for public extensions.\"\n    },\n    \"icon_path\": {\n      \"type\": \"string\",\n      \"description\": \"Path to the extension icon within the package.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-launch/refs/heads/main/json-schema/extension-extension-package-attributes-schema.json
tags:
- Data Collection
- Edge Network
- Event Forwarding
- Marketing Technology
- Tag Management
title: ExtensionPackageAttributes
---
