---
description: Schema for a PI System time-series data point containing a timestamp, value, and quality information.
layout: schema
name: OSIsoft PI Timed Value
properties_list:
- description: UTC timestamp of the value
  name: Timestamp
  type: string
- description: The data value; numeric for analog points, string or object for digital/string points
  name: Value
  type: object
- description: True if the value quality is Good (not a system digital state)
  name: Good
  type: boolean
- description: True if the value is flagged as questionable by the data source
  name: Questionable
  type: boolean
- description: True if the value has been manually substituted
  name: Substituted
  type: boolean
- description: True if the value has an annotation
  name: Annotated
  type: boolean
- description: Unit of measure abbreviation
  name: UnitsAbbreviation
  type: string
provider_name: osisoft-pi
provider_slug: osisoft-pi
schema_file: json-schema/osisoft-pi-timed-value-schema.json
slug: osisoft-pi-timed-value
source_filename: osisoft-pi-timed-value-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/osisoft-pi/json-schema/osisoft-pi-timed-value-schema.json\",\n  \"title\": \"OSIsoft PI Timed Value\",\n  \"description\": \"Schema for a PI System time-series data point containing a timestamp, value, and quality information.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"UTC timestamp of the value\"\n    },\n    \"Value\": {\n      \"description\": \"The data value; numeric for analog points, string or object for digital/string points\",\n      \"oneOf\": [\n        {\n          \"type\": \"number\",\n          \"description\": \"Numeric value for Float or Int point types\"\n        },\n        {\n          \"type\": \"string\",\n          \"description\": \"String value for String point types\"\n        },\n        {\n          \"type\": \"object\"\
  ,\n          \"description\": \"Digital state object for Digital point types\",\n          \"properties\": {\n            \"Name\": {\n              \"type\": \"string\",\n              \"description\": \"Digital state name (e.g. Shutdown, Running, Fault)\"\n            },\n            \"Value\": {\n              \"type\": \"integer\",\n              \"description\": \"Digital state numeric code\"\n            }\n          },\n          \"required\": [\"Name\", \"Value\"]\n        }\n      ]\n    },\n    \"Good\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the value quality is Good (not a system digital state)\"\n    },\n    \"Questionable\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the value is flagged as questionable by the data source\"\n    },\n    \"Substituted\": {\n      \"type\": \"boolean\",\n      \"description\": \"True if the value has been manually substituted\"\n    },\n    \"Annotated\": {\n      \"type\": \"boolean\",\n  \
  \    \"description\": \"True if the value has an annotation\"\n    },\n    \"UnitsAbbreviation\": {\n      \"type\": \"string\",\n      \"description\": \"Unit of measure abbreviation\"\n    }\n  },\n  \"required\": [\"Timestamp\"],\n  \"examples\": [\n    {\n      \"Timestamp\": \"2026-03-18T14:30:00Z\",\n      \"Value\": 87.3,\n      \"Good\": true,\n      \"Questionable\": false,\n      \"Substituted\": false,\n      \"Annotated\": false,\n      \"UnitsAbbreviation\": \"°C\"\n    },\n    {\n      \"Timestamp\": \"2026-03-18T14:25:00Z\",\n      \"Value\": {\n        \"Name\": \"Running\",\n        \"Value\": 2\n      },\n      \"Good\": true,\n      \"Questionable\": false,\n      \"Substituted\": false,\n      \"Annotated\": false,\n      \"UnitsAbbreviation\": \"\"\n    }\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/json-schema/osisoft-pi-timed-value-schema.json
tags: []
title: OSIsoft PI Timed Value
---
