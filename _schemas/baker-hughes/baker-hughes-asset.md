---
description: An industrial asset monitored by Baker Hughes Cordant platform.
layout: schema
name: Asset
properties_list:
- description: Unique identifier for the asset.
  name: assetId
  type: string
- description: Human-readable name for the asset.
  name: assetName
  type: string
- description: Classification of the asset (e.g., compressor, pump, turbine).
  name: assetType
  type: string
- description: Identifier of the facility where the asset is located.
  name: facilityId
  type: string
- description: Geographic or plant location of the asset.
  name: location
  type: string
- description: Current operational status of the asset.
  name: status
  type: string
- description: AI-computed health score from 0 (critical) to 100 (healthy).
  name: healthScore
  type: number
- description: Timestamp of the last data update for this asset.
  name: lastUpdated
  type: string
- description: User-defined tags for organizing and filtering assets.
  name: tags
  type: array
provider_name: Baker Hughes
provider_slug: baker-hughes
schema_file: json-schema/baker-hughes-asset-schema.json
slug: baker-hughes-asset
source_filename: baker-hughes-asset-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/baker-hughes/json-schema/baker-hughes-asset-schema.json\",\n  \"title\": \"Asset\",\n  \"description\": \"An industrial asset monitored by Baker Hughes Cordant platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"assetId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the asset.\"\n    },\n    \"assetName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for the asset.\"\n    },\n    \"assetType\": {\n      \"type\": \"string\",\n      \"description\": \"Classification of the asset (e.g., compressor, pump, turbine).\",\n      \"enum\": [\"compressor\", \"pump\", \"turbine\", \"heat-exchanger\", \"separator\", \"valve\", \"other\"]\n    },\n    \"facilityId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the facility where the asset is located.\"\n    },\n    \"\
  location\": {\n      \"type\": \"string\",\n      \"description\": \"Geographic or plant location of the asset.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status of the asset.\",\n      \"enum\": [\"running\", \"idle\", \"maintenance\", \"fault\", \"offline\"]\n    },\n    \"healthScore\": {\n      \"type\": \"number\",\n      \"description\": \"AI-computed health score from 0 (critical) to 100 (healthy).\",\n      \"minimum\": 0,\n      \"maximum\": 100\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last data update for this asset.\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"User-defined tags for organizing and filtering assets.\"\n    }\n  },\n  \"required\": [\"assetId\", \"assetName\", \"assetType\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/baker-hughes/refs/heads/main/json-schema/baker-hughes-asset-schema.json
tags:
- Energy Technology
- Industrial IoT
- Oil And Gas
- Asset Performance Management
- Digital Energy
title: Asset
---
