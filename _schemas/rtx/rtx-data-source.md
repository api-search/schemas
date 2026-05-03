---
description: A configured intelligence or logistics data source in the RTX EAGLE platform
layout: schema
name: RTX EAGLE Data Source
properties_list:
- description: Unique identifier for the data source
  name: id
  type: string
- description: Human-readable name of the data source
  name: name
  type: string
- description: Type of data source (e.g., LogisticsDB, IntelligenceDB, AnalyticsDB)
  name: type
  type: string
- description: Current operational status
  name: status
  type: string
- description: Description of data contained in this source
  name: description
  type: string
- description: Defense program this data source is associated with
  name: program
  type: string
- description: Data classification level
  name: classification
  type: string
provider_name: RTX
provider_slug: rtx
schema_file: json-schema/rtx-data-source-schema.json
slug: rtx-data-source
source_filename: rtx-data-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.rtx.com/eagle/schemas/data-source\",\n  \"title\": \"RTX EAGLE Data Source\",\n  \"description\": \"A configured intelligence or logistics data source in the RTX EAGLE platform\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the data source\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the data source\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of data source (e.g., LogisticsDB, IntelligenceDB, AnalyticsDB)\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current operational status\",\n      \"enum\": [\"Active\", \"Inactive\", \"Maintenance\", \"Error\"]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of\
  \ data contained in this source\"\n    },\n    \"program\": {\n      \"type\": \"string\",\n      \"description\": \"Defense program this data source is associated with\"\n    },\n    \"classification\": {\n      \"type\": \"string\",\n      \"description\": \"Data classification level\"\n    }\n  },\n  \"required\": [\"id\", \"name\", \"type\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rtx/refs/heads/main/json-schema/rtx-data-source-schema.json
tags:
- Defense
- Aerospace
- Government
- Logistics
- Intelligence
- Military
title: RTX EAGLE Data Source
---
