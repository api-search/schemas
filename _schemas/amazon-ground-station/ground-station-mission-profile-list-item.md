---
description: Item in a list of mission profiles.
layout: schema
name: MissionProfileListItem
properties_list:
- description: ''
  name: missionProfileArn
  type: object
- description: ''
  name: missionProfileId
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: region
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-mission-profile-list-item-schema.json
slug: ground-station-mission-profile-list-item
source_filename: ground-station-mission-profile-list-item-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-mission-profile-list-item-schema.json\",\n  \"title\": \"MissionProfileListItem\",\n  \"description\": \"Item in a list of mission profiles.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"missionProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MissionProfileArn\"\n        },\n        {\n          \"description\": \"ARN of a mission profile.\"\n        }\n      ]\n    },\n    \"missionProfileId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of a mission profile.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SafeName\"\n        },\n        {\n          \"description\"\
  : \"Name of a mission profile.\"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSRegion\"\n        },\n        {\n          \"description\": \"Region of a mission profile.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-mission-profile-list-item-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: MissionProfileListItem
---
