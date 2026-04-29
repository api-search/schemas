---
description: Library analytics variable usage data broken down by variable.
layout: schema
name: LibraryAnalyticsVariableUsagesByAsset
properties_list:
- description: Unique, stable id of the variable.
  name: variableKey
  type: string
- description: The name of the variable.
  name: variableName
  type: string
- description: The type of the variable.
  name: variableType
  type: string
- description: Unique, stable id of the collection the variable belongs to.
  name: collectionKey
  type: string
- description: The name of the collection the variable belongs to.
  name: collectionName
  type: string
- description: The number of usages of the variable within the organization.
  name: usages
  type: number
- description: The number of teams using the variable within the organization.
  name: teamsUsing
  type: number
- description: The number of files using the variable within the organization.
  name: filesUsing
  type: number
provider_name: Figma
provider_slug: figma
schema_file: json-schema/figma-analytics-library-analytics-variable-usages-by-asset-schema.json
slug: figma-analytics-library-analytics-variable-usages-by-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LibraryAnalyticsVariableUsagesByAsset\",\n  \"type\": \"object\",\n  \"description\": \"Library analytics variable usage data broken down by variable.\",\n  \"properties\": {\n    \"variableKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique, stable id of the variable.\"\n    },\n    \"variableName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the variable.\"\n    },\n    \"variableType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the variable.\"\n    },\n    \"collectionKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique, stable id of the collection the variable belongs to.\"\n    },\n    \"collectionName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the collection the variable belongs to.\"\n    },\n    \"usages\": {\n      \"type\": \"number\",\n      \"description\": \"The\
  \ number of usages of the variable within the organization.\"\n    },\n    \"teamsUsing\": {\n      \"type\": \"number\",\n      \"description\": \"The number of teams using the variable within the organization.\"\n    },\n    \"filesUsing\": {\n      \"type\": \"number\",\n      \"description\": \"The number of files using the variable within the organization.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/figma/refs/heads/main/json-schema/figma-analytics-library-analytics-variable-usages-by-asset-schema.json
tags:
- Collaboration
- Design
- Graphics
- Interfaces
- Prototypes
- Prototyping
- UI/UX
title: LibraryAnalyticsVariableUsagesByAsset
---
