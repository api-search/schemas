---
description: Object that represents EIRP.
layout: schema
name: Eirp
properties_list:
- description: ''
  name: units
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-eirp-schema.json
slug: ground-station-eirp
source_filename: ground-station-eirp-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-eirp-schema.json\",\n  \"title\": \"Eirp\",\n  \"description\": \"Object that represents EIRP.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"units\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EirpUnits\"\n        },\n        {\n          \"description\": \"Units of an EIRP.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"Value of an EIRP. Valid values are between 20.0 to 50.0 dBW.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"units\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-eirp-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: Eirp
---
