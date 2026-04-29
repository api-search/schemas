---
description: Add-on allocation information for an environment.
layout: schema
name: AddonInfo
properties_list:
- description: The type of add-on.
  name: addonType
  type: string
- description: The number of allocated add-on units.
  name: allocated
  type: number
- description: The unit of measurement for the add-on.
  name: addonUnit
  type: string
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-addon-info-schema.json
slug: power-platform-addon-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AddonInfo\",\n  \"type\": \"object\",\n  \"description\": \"Add-on allocation information for an environment.\",\n  \"properties\": {\n    \"addonType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of add-on.\"\n    },\n    \"allocated\": {\n      \"type\": \"number\",\n      \"description\": \"The number of allocated add-on units.\"\n    },\n    \"addonUnit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of measurement for the add-on.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-addon-info-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: AddonInfo
---
