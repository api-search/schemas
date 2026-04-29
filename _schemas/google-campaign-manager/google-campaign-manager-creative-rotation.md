---
description: Creative rotation configuration controlling how creatives are served within an ad.
layout: schema
name: CreativeRotation
properties_list:
- description: Type of creative rotation.
  name: type
  type: string
- description: Strategy for calculating creative weights.
  name: weightCalculationStrategy
  type: string
- description: Creative assignments in this creative rotation.
  name: creativeAssignments
  type: array
- description: Creative optimization configuration used for this creative rotation.
  name: creativeOptimizationConfigurationId
  type: string
provider_name: Google Campaign Manager
provider_slug: google-campaign-manager
schema_file: json-schema/google-campaign-manager-creative-rotation-schema.json
slug: google-campaign-manager-creative-rotation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreativeRotation\",\n  \"type\": \"object\",\n  \"description\": \"Creative rotation configuration controlling how creatives are served within an ad.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of creative rotation.\"\n    },\n    \"weightCalculationStrategy\": {\n      \"type\": \"string\",\n      \"description\": \"Strategy for calculating creative weights.\"\n    },\n    \"creativeAssignments\": {\n      \"type\": \"array\",\n      \"description\": \"Creative assignments in this creative rotation.\"\n    },\n    \"creativeOptimizationConfigurationId\": {\n      \"type\": \"string\",\n      \"description\": \"Creative optimization configuration used for this creative rotation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-campaign-manager/refs/heads/main/json-schema/google-campaign-manager-creative-rotation-schema.json
tags:
- Advertising
- Analytics
- Campaign Management
- Digital Marketing
- Reporting
title: CreativeRotation
---
