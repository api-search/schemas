---
description: An integer range that has a minimum and maximum value.
layout: schema
name: IntegerRange
properties_list:
- description: ''
  name: maximum
  type: object
- description: ''
  name: minimum
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-integer-range-schema.json
slug: ground-station-integer-range
source_filename: ground-station-integer-range-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-integer-range-schema.json\",\n  \"title\": \"IntegerRange\",\n  \"description\": \"An integer range that has a minimum and maximum value.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"maximum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"A maximum value.\"\n        }\n      ]\n    },\n    \"minimum\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Integer\"\n        },\n        {\n          \"description\": \"A minimum value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"maximum\",\n    \"minimum\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-integer-range-schema.json
tags:
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: IntegerRange
---
