---
description: JSON Schema for an AspenTech Inmation process data item (tag) including current value, quality, and historical data.
layout: schema
name: AspenTech Inmation Data Item
properties_list:
- description: Full hierarchical path to the data item in the Inmation system tree (e.g., /System/Core/Plant1/Temperature)
  name: path
  type: string
- description: Current process value - can be numeric, string, or boolean
  name: value
  type: object
- description: OPC UA/DA quality code (192=Good, 0=Bad, 64=Uncertain)
  name: quality
  type: integer
- description: Timestamp of the current value (ISO 8601 UTC)
  name: timestamp
  type: string
- description: Engineering unit for the value (e.g., degC, bar, m3/h)
  name: engineeringUnit
  type: string
- description: Type of Inmation item
  name: itemType
  type: string
- description: Item display name
  name: name
  type: string
- description: Item description
  name: description
  type: string
- description: High engineering range limit
  name: highLimit
  type: number
- description: Low engineering range limit
  name: lowLimit
  type: number
- description: High alarm threshold
  name: alarmHigh
  type: number
- description: Low alarm threshold
  name: alarmLow
  type: number
- description: Deadband for value change detection
  name: deadband
  type: number
provider_name: AspenTech
provider_slug: aspentech
schema_file: json-schema/aspentech-dataitem-schema.json
slug: aspentech-dataitem
source_filename: aspentech-dataitem-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/json-schema/aspentech-dataitem-schema.json\",\n  \"title\": \"AspenTech Inmation Data Item\",\n  \"description\": \"JSON Schema for an AspenTech Inmation process data item (tag) including current value, quality, and historical data.\",\n  \"type\": \"object\",\n  \"required\": [\"path\"],\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Full hierarchical path to the data item in the Inmation system tree (e.g., /System/Core/Plant1/Temperature)\"\n    },\n    \"value\": {\n      \"description\": \"Current process value - can be numeric, string, or boolean\",\n      \"oneOf\": [\n        {\"type\": \"number\"},\n        {\"type\": \"string\"},\n        {\"type\": \"boolean\"},\n        {\"type\": \"null\"}\n      ]\n    },\n    \"quality\": {\n      \"type\": \"integer\",\n     \
  \ \"description\": \"OPC UA/DA quality code (192=Good, 0=Bad, 64=Uncertain)\",\n      \"minimum\": 0,\n      \"maximum\": 255\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the current value (ISO 8601 UTC)\"\n    },\n    \"engineeringUnit\": {\n      \"type\": \"string\",\n      \"description\": \"Engineering unit for the value (e.g., degC, bar, m3/h)\"\n    },\n    \"itemType\": {\n      \"type\": \"string\",\n      \"description\": \"Type of Inmation item\",\n      \"enum\": [\"GenItem\", \"InmationGenItem\", \"Model\", \"Trend\", \"Calculation\", \"Connector\"]\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Item display name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Item description\"\n    },\n    \"highLimit\": {\n      \"type\": \"number\",\n      \"description\": \"High engineering range limit\"\n    },\n    \"lowLimit\"\
  : {\n      \"type\": \"number\",\n      \"description\": \"Low engineering range limit\"\n    },\n    \"alarmHigh\": {\n      \"type\": \"number\",\n      \"description\": \"High alarm threshold\"\n    },\n    \"alarmLow\": {\n      \"type\": \"number\",\n      \"description\": \"Low alarm threshold\"\n    },\n    \"deadband\": {\n      \"type\": \"number\",\n      \"description\": \"Deadband for value change detection\",\n      \"minimum\": 0\n    }\n  },\n  \"$defs\": {\n    \"HistoricalValue\": {\n      \"type\": \"object\",\n      \"required\": [\"value\", \"timestamp\"],\n      \"properties\": {\n        \"value\": {\n          \"oneOf\": [\n            {\"type\": \"number\"},\n            {\"type\": \"string\"},\n            {\"type\": \"boolean\"},\n            {\"type\": \"null\"}\n          ]\n        },\n        \"quality\": {\n          \"type\": \"integer\",\n          \"minimum\": 0,\n          \"maximum\": 255\n        },\n        \"timestamp\": {\n          \"type\": \"\
  string\",\n          \"format\": \"date-time\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/json-schema/aspentech-dataitem-schema.json
tags:
- Industrial IoT
- Process Optimization
- Manufacturing
- Energy
- Chemicals
- Time Series
title: AspenTech Inmation Data Item
---
