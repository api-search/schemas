---
description: Flag schema from AB Tasty Decision API
layout: schema
name: Flag
properties_list:
- description: Value of the flag
  name: value
  type: object
- description: ''
  name: metadata
  type: object
provider_name: AB Tasty
provider_slug: ab-tasty
schema_file: json-schema/decision-api-flag-schema.json
slug: decision-api-flag
source_filename: decision-api-flag-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-flag-schema.json\",\n  \"title\": \"Flag\",\n  \"description\": \"Flag schema from AB Tasty Decision API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"value\": {\n      \"oneOf\": [\n        {\n          \"type\": \"object\"\n        },\n        {\n          \"type\": \"string\"\n        },\n        {\n          \"type\": \"number\"\n        },\n        {\n          \"type\": \"boolean\"\n        }\n      ],\n      \"description\": \"Value of the flag\"\n    },\n    \"metadata\": {\n      \"$ref\": \"#/components/schemas/FlagMetadata\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ab-tasty/refs/heads/main/json-schema/decision-api-flag-schema.json
tags:
- Aggregation
- Experimentation
- Feature Flags
- Personalization
- A/B Testing
title: Flag
---
