---
description: An Air Force Reserve unit
layout: schema
name: ReserveUnit
properties_list:
- description: Unit designation
  name: unit_id
  type: string
- description: Full unit name
  name: name
  type: string
- description: Installation/base name
  name: location
  type: string
- description: Primary unit mission
  name: mission
  type: string
- description: Primary aircraft type
  name: aircraft
  type: string
- description: Wing type classification
  name: wing_type
  type: string
provider_name: Air Force Reserve
provider_slug: air-force-reserve
schema_file: json-schema/afrc-reserve-unit-schema.json
slug: afrc-reserve-unit
source_filename: afrc-reserve-unit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/air-force-reserve/refs/heads/main/json-schema/afrc-reserve-unit-schema.json\",\n  \"title\": \"ReserveUnit\",\n  \"description\": \"An Air Force Reserve unit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unit_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unit designation\",\n      \"example\": \"433rd AW\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Full unit name\",\n      \"example\": \"433rd Airlift Wing\"\n    },\n    \"location\": {\n      \"type\": \"string\",\n      \"description\": \"Installation/base name\",\n      \"example\": \"Joint Base San Antonio-Lackland, TX\"\n    },\n    \"mission\": {\n      \"type\": \"string\",\n      \"description\": \"Primary unit mission\",\n      \"example\": \"Strategic airlift using C-5M Super Galaxy\"\n    },\n    \"aircraft\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Primary aircraft type\",\n      \"example\": \"C-5M Super Galaxy\"\n    },\n    \"wing_type\": {\n      \"type\": \"string\",\n      \"description\": \"Wing type classification\",\n      \"example\": \"Airlift\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/air-force-reserve/refs/heads/main/json-schema/afrc-reserve-unit-schema.json
tags:
- Federal Government
- Military
- Defense
- Air Force
- United States Government
title: ReserveUnit
---
