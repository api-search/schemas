---
description: A time range with a start and end time.
layout: schema
name: TimeRange
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: startTime
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-time-range-schema.json
slug: ground-station-time-range
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-time-range-schema.json\",\n  \"title\": \"TimeRange\",\n  \"description\": \"A time range with a start and end time.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Time in UTC at which the time range ends.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Time in UTC at which the time range starts.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"endTime\",\n    \"startTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-time-range-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: TimeRange
---
