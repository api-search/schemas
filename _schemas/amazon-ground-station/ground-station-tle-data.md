---
description: Two-line element set (TLE) data.
layout: schema
name: TLEData
properties_list:
- description: ''
  name: tleLine1
  type: object
- description: ''
  name: tleLine2
  type: object
- description: ''
  name: validTimeRange
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-tle-data-schema.json
slug: ground-station-tle-data
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-tle-data-schema.json\",\n  \"title\": \"TLEData\",\n  \"description\": \"Two-line element set (TLE) data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"tleLine1\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TleLineOne\"\n        },\n        {\n          \"description\": \"First line of two-line element set (TLE) data.\"\n        }\n      ]\n    },\n    \"tleLine2\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TleLineTwo\"\n        },\n        {\n          \"description\": \"Second line of two-line element set (TLE) data.\"\n        }\n      ]\n    },\n    \"validTimeRange\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TimeRange\"\n        },\n        {\n          \"description\"\
  : \"The valid time range for the TLE. Gaps or overlap are not permitted.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"tleLine1\",\n    \"tleLine2\",\n    \"validTimeRange\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-tle-data-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: TLEData
---
