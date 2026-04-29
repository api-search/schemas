---
description: <p/>
layout: schema
name: ReserveContactRequest
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: groundStation
  type: object
- description: ''
  name: missionProfileArn
  type: object
- description: ''
  name: satelliteArn
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-reserve-contact-request-schema.json
slug: ground-station-reserve-contact-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-reserve-contact-request-schema.json\",\n  \"title\": \"ReserveContactRequest\",\n  \"description\": \"<p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"End time of a contact in UTC.\"\n        }\n      ]\n    },\n    \"groundStation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroundStationName\"\n        },\n        {\n          \"description\": \"Name of a ground station.\"\n        }\n      ]\n    },\n    \"missionProfileArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MissionProfileArn\"\n        },\n        {\n          \"description\": \"ARN of a\
  \ mission profile.\"\n        }\n      ]\n    },\n    \"satelliteArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/satelliteArn\"\n        },\n        {\n          \"description\": \"ARN of a satellite\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Start time of a contact in UTC.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagsMap\"\n        },\n        {\n          \"description\": \"Tags assigned to a contact.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"endTime\",\n    \"groundStation\",\n    \"missionProfileArn\",\n    \"satelliteArn\",\n    \"startTime\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-reserve-contact-request-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: ReserveContactRequest
---
