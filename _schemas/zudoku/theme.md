---
description: Schema for the Zudoku theme and branding configuration that customizes colors, fonts, logos, and dark mode settings for the generated documentation portal.
layout: schema
name: Zudoku Theme Configuration
properties_list:
- description: Color palette for light mode.
  name: light
  type: object
- description: Color palette for dark mode.
  name: dark
  type: object
- description: Font family configuration for different text elements.
  name: fonts
  type: object
provider_name: Zudoku
provider_slug: zudoku
schema_file: json-schema/theme.json
slug: theme
source_filename: theme.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zudoku/blob/main/json-schema/theme.json\",\n  \"title\": \"Zudoku Theme Configuration\",\n  \"description\": \"Schema for the Zudoku theme and branding configuration that customizes colors, fonts, logos, and dark mode settings for the generated documentation portal.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"light\": {\n      \"$ref\": \"#/$defs/ThemeColors\",\n      \"description\": \"Color palette for light mode.\"\n    },\n    \"dark\": {\n      \"$ref\": \"#/$defs/ThemeColors\",\n      \"description\": \"Color palette for dark mode.\"\n    },\n    \"fonts\": {\n      \"type\": \"object\",\n      \"description\": \"Font family configuration for different text elements.\",\n      \"properties\": {\n        \"heading\": {\n          \"type\": \"string\",\n          \"description\": \"Font family for headings.\"\n        },\n        \"body\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"Font family for body text.\"\n        },\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Font family for code blocks and inline code.\"\n        }\n      }\n    }\n  },\n  \"$defs\": {\n    \"ThemeColors\": {\n      \"type\": \"object\",\n      \"description\": \"Color palette for a theme mode.\",\n      \"properties\": {\n        \"primary\": {\n          \"type\": \"string\",\n          \"description\": \"Primary brand color in CSS format.\"\n        },\n        \"background\": {\n          \"type\": \"string\",\n          \"description\": \"Background color in CSS format.\"\n        },\n        \"border\": {\n          \"type\": \"string\",\n          \"description\": \"Border color in CSS format.\"\n        },\n        \"primaryForeground\": {\n          \"type\": \"string\",\n          \"description\": \"Foreground color used on primary backgrounds.\"\n        },\n        \"secondaryForeground\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Foreground color used on secondary backgrounds.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zudoku/refs/heads/main/json-schema/theme.json
tags:
- Developer Tools
- Documentation
title: Zudoku Theme Configuration
---
