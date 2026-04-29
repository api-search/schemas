---
description: Library analytics style usage data broken down by asset.
layout: schema
name: LibraryAnalyticsStyleUsagesByAsset
properties_list:
- description: Unique, stable id of the style.
  name: styleKey
  type: string
- description: The name of the style.
  name: styleName
  type: string
- description: The type of the style.
  name: styleType
  type: string
- description: The number of usages of the style within the organization.
  name: usages
  type: number
- description: The number of teams using the style within the organization.
  name: teamsUsing
  type: number
- description: The number of files using the style within the organization.
  name: filesUsing
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-analytics-library-analytics-style-usages-by-asset-schema.json
slug: figma-analytics-library-analytics-style-usages-by-asset
source_filename: figma-analytics-library-analytics-style-usages-by-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryAnalyticsStyleUsagesByAsset\",\n  \"type\": \"object\",\n  \"description\": \"Library analytics style usage data broken down by asset.\",\n  \"properties\": {\n    \"styleKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique, stable id of the style.\"\n    },\n    \"styleName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the style.\"\n    },\n    \"styleType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the style.\"\n    },\n    \"usages\": {\n      \"type\": \"number\",\n      \"description\": \"The number of usages of the style within the organization.\"\n    },\n    \"teamsUsing\": {\n      \"type\": \"number\",\n      \"description\": \"The number of teams using the style within the organization.\"\n    },\n    \"filesUsing\": {\n      \"type\": \"number\",\n      \"description\": \"The number of files using the\
  \ style within the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-analytics-library-analytics-style-usages-by-asset-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: LibraryAnalyticsStyleUsagesByAsset
---
