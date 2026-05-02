---
description: A plugin resource in the JetBrains Marketplace.
layout: schema
name: JetBrains Marketplace Plugin
properties_list:
- description: Unique numeric identifier of the plugin.
  name: id
  type: integer
- description: Name of the plugin.
  name: name
  type: string
- description: XML/plugin ID used for installation.
  name: xmlId
  type: string
- description: Description of the plugin.
  name: description
  type: string
- description: Plugin vendor information.
  name: vendor
  type: object
- description: Total download count.
  name: downloads
  type: integer
- description: Average user rating.
  name: rating
  type: number
- description: Latest version string.
  name: version
  type: string
- description: List of compatible JetBrains products.
  name: compatibleProducts
  type: array
- description: Plugin tags/categories.
  name: tags
  type: array
provider_name: JetBrains
provider_slug: jetbrains
schema_file: json-schema/plugin.json
slug: plugin
source_filename: plugin.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jetbrains-plugin.json\",\n  \"title\": \"JetBrains Marketplace Plugin\",\n  \"description\": \"A plugin resource in the JetBrains Marketplace.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique numeric identifier of the plugin.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the plugin.\"\n    },\n    \"xmlId\": {\n      \"type\": \"string\",\n      \"description\": \"XML/plugin ID used for installation.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the plugin.\"\n    },\n    \"vendor\": {\n      \"type\": \"object\",\n      \"description\": \"Plugin vendor information.\",\n      \"properties\": {\n        \"name\": { \"type\": \"string\" },\n        \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    },\n\
  \    \"downloads\": {\n      \"type\": \"integer\",\n      \"description\": \"Total download count.\"\n    },\n    \"rating\": {\n      \"type\": \"number\",\n      \"description\": \"Average user rating.\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"description\": \"Latest version string.\"\n    },\n    \"compatibleProducts\": {\n      \"type\": \"array\",\n      \"description\": \"List of compatible JetBrains products.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"productCode\": { \"type\": \"string\" },\n          \"name\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Plugin tags/categories.\",\n      \"items\": { \"type\": \"string\" }\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/json-schema/plugin.json
tags:
- CI/CD
- Developer Tools
- IDE
title: JetBrains Marketplace Plugin
---
