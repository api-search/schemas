---
description: Information about the ground station data.
layout: schema
name: GroundStationData
properties_list:
- description: ''
  name: groundStationId
  type: object
- description: ''
  name: groundStationName
  type: object
- description: ''
  name: region
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-ground-station-data-schema.json
slug: ground-station-ground-station-data
source_filename: ground-station-ground-station-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ground-station-data-schema.json\",\n  \"title\": \"GroundStationData\",\n  \"description\": \"Information about the ground station data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"groundStationId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroundStationName\"\n        },\n        {\n          \"description\": \"UUID of a ground station.\"\n        }\n      ]\n    },\n    \"groundStationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroundStationName\"\n        },\n        {\n          \"description\": \"Name of a ground station.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSRegion\"\n        },\n        {\n         \
  \ \"description\": \"Ground station Region.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-ground-station-data-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: GroundStationData
---
