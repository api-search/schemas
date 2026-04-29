---
description: Capacity consumption information for an environment.
layout: schema
name: CapacityInfo
properties_list:
- description: The type of capacity.
  name: capacityType
  type: string
- description: The actual capacity consumption.
  name: actualConsumption
  type: number
- description: The rated capacity consumption.
  name: ratedConsumption
  type: number
- description: The unit of measurement for capacity.
  name: capacityUnit
  type: string
- description: The timestamp when the capacity data was last updated.
  name: updatedOn
  type: string
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-capacity-info-schema.json
slug: power-platform-capacity-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CapacityInfo\",\n  \"type\": \"object\",\n  \"description\": \"Capacity consumption information for an environment.\",\n  \"properties\": {\n    \"capacityType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of capacity.\"\n    },\n    \"actualConsumption\": {\n      \"type\": \"number\",\n      \"description\": \"The actual capacity consumption.\"\n    },\n    \"ratedConsumption\": {\n      \"type\": \"number\",\n      \"description\": \"The rated capacity consumption.\"\n    },\n    \"capacityUnit\": {\n      \"type\": \"string\",\n      \"description\": \"The unit of measurement for capacity.\"\n    },\n    \"updatedOn\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the capacity data was last updated.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-capacity-info-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: CapacityInfo
---
