---
description: Elevation angle of the satellite in the sky during a contact.
layout: schema
name: Elevation
properties_list:
- description: ''
  name: unit
  type: object
- description: ''
  name: value
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-elevation-schema.json
slug: ground-station-elevation
source_filename: ground-station-elevation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-elevation-schema.json\",\n  \"title\": \"Elevation\",\n  \"description\": \"Elevation angle of the satellite in the sky during a contact.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"unit\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AngleUnits\"\n        },\n        {\n          \"description\": \"Elevation angle units.\"\n        }\n      ]\n    },\n    \"value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Double\"\n        },\n        {\n          \"description\": \"Elevation angle value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"unit\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-elevation-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: Elevation
---
