---
description: Schema for a Zudoku plugin configuration. Plugins extend the platform with additional functionality such as search (Pagefind, Inkeep), analytics (Sentry), and custom pages.
layout: schema
name: Zudoku Plugin
properties_list:
- description: Plugin name identifier, e.g. 'search-pagefind', 'sentry', or a custom plugin name.
  name: name
  type: string
- description: Plugin-specific configuration options. Structure varies by plugin.
  name: config
  type: object
provider_name: Zudoku
provider_slug: zudoku
schema_file: json-schema/plugin.json
slug: plugin
source_filename: plugin.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zudoku/blob/main/json-schema/plugin.json\",\n  \"title\": \"Zudoku Plugin\",\n  \"description\": \"Schema for a Zudoku plugin configuration. Plugins extend the platform with additional functionality such as search (Pagefind, Inkeep), analytics (Sentry), and custom pages.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Plugin name identifier, e.g. 'search-pagefind', 'sentry', or a custom plugin name.\"\n    },\n    \"config\": {\n      \"type\": \"object\",\n      \"description\": \"Plugin-specific configuration options. Structure varies by plugin.\",\n      \"additionalProperties\": true\n    }\n  },\n  \"required\": [\"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/json-schema/plugin.json
tags:
- Developer Tools
- Documentation
title: Zudoku Plugin
---
