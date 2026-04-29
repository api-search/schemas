---
description: Object that describes the frequency.
layout: schema
name: Frequency
properties_list:
- description: ''
  name: units
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-frequency-schema.json
slug: ground-station-frequency
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-frequency-schema.json\",\n  \"title\": \"Frequency\",\n  \"description\": \"Object that describes the frequency.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"units\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FrequencyUnits\"\n        },\n        {\n          \"description\": \"Frequency units.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"Frequency value. Valid values are between 2200 to 2300 MHz and 7750 to 8400 MHz for downlink and 2025 to 2120 MHz for uplink.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"units\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-frequency-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: Frequency
---
