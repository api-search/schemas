---
description: Package dimensions
layout: schema
name: Dimensions
properties_list:
- description: Package length
  name: length
  type: number
- description: Package width
  name: width
  type: number
- description: Package height
  name: height
  type: number
- description: Dimension unit
  name: unit
  type: string
provider_name: Alaska Airlines
provider_slug: alaska-air
schema_file: json-schema/alaska-air-cargo-dimensions-schema.json
slug: alaska-air-cargo-dimensions
source_filename: alaska-air-cargo-dimensions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-dimensions-schema.json\",\n  \"title\": \"Dimensions\",\n  \"description\": \"Package dimensions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"length\": {\n      \"type\": \"number\",\n      \"description\": \"Package length\",\n      \"example\": 60\n    },\n    \"width\": {\n      \"type\": \"number\",\n      \"description\": \"Package width\",\n      \"example\": 40\n    },\n    \"height\": {\n      \"type\": \"number\",\n      \"description\": \"Package height\",\n      \"example\": 30\n    },\n    \"unit\": {\n      \"type\": \"string\",\n      \"description\": \"Dimension unit\",\n      \"enum\": [\n        \"CM\",\n        \"IN\"\n      ],\n      \"example\": \"CM\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alaska-air/refs/heads/main/json-schema/alaska-air-cargo-dimensions-schema.json
tags:
- Airlines
- Aviation
- Travel
- Cargo
- Loyalty
- Flight Status
title: Dimensions
---
