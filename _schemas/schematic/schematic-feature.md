---
description: A product feature in Schematic that can be included in plans, targeted by flags, and tracked via events.
layout: schema
name: Schematic Feature
properties_list:
- description: Unique Schematic feature identifier.
  name: id
  type: string
- description: Display name of the feature.
  name: name
  type: string
- description: 'Type of feature: boolean (on/off), trait-based, or event-metered.'
  name: featureType
  type: string
- description: Human-readable description of the feature.
  name: description
  type: string
- description: The feature flag associated with this feature.
  name: flag
  type: object
- description: ''
  name: createdAt
  type: string
- description: ''
  name: updatedAt
  type: string
provider_name: Schematic
provider_slug: schematic
schema_file: json-schema/schematic-feature-schema.json
slug: schematic-feature
source_filename: schematic-feature-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.schematichq.com/schemas/feature\",\n  \"title\": \"Schematic Feature\",\n  \"description\": \"A product feature in Schematic that can be included in plans, targeted by flags, and tracked via events.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Schematic feature identifier.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the feature.\"\n    },\n    \"featureType\": {\n      \"type\": \"string\",\n      \"enum\": [\"boolean\", \"trait\", \"event\"],\n      \"description\": \"Type of feature: boolean (on/off), trait-based, or event-metered.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the feature.\"\n    },\n    \"flag\": {\n      \"$ref\": \"#/$defs/FlagRef\",\n      \"description\"\
  : \"The feature flag associated with this feature.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"featureType\"],\n  \"$defs\": {\n    \"FlagRef\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"key\": { \"type\": \"string\" },\n        \"defaultValue\": { \"type\": \"boolean\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/schematic/refs/heads/main/json-schema/schematic-feature-schema.json
tags:
- Billing
- Entitlements
- Feature Flags
- Feature Management
- FinOps
- Metering
- Pricing
- SaaS
title: Schematic Feature
---
