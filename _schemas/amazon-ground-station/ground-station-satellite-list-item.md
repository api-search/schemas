---
description: Item in a list of satellites.
layout: schema
name: SatelliteListItem
properties_list:
- description: ''
  name: currentEphemeris
  type: object
- description: ''
  name: groundStations
  type: object
- description: ''
  name: noradSatelliteID
  type: object
- description: ''
  name: satelliteArn
  type: object
- description: ''
  name: satelliteId
  type: object
provider_name: Amazon Ground Station
provider_slug: amazon-ground-station
schema_file: json-schema/ground-station-satellite-list-item-schema.json
slug: ground-station-satellite-list-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-satellite-list-item-schema.json\",\n  \"title\": \"SatelliteListItem\",\n  \"description\": \"Item in a list of satellites.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentEphemeris\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EphemerisMetaData\"\n        },\n        {\n          \"description\": \"The current ephemeris being used to compute the trajectory of the satellite.\"\n        }\n      ]\n    },\n    \"groundStations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/GroundStationIdList\"\n        },\n        {\n          \"description\": \"A list of ground stations to which the satellite is on-boarded.\"\n        }\n      ]\n    },\n    \"noradSatelliteID\": {\n      \"allOf\": [\n        {\n  \
  \        \"$ref\": \"#/components/schemas/noradSatelliteID\"\n        },\n        {\n          \"description\": \"NORAD satellite ID number.\"\n        }\n      ]\n    },\n    \"satelliteArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/satelliteArn\"\n        },\n        {\n          \"description\": \"ARN of a satellite.\"\n        }\n      ]\n    },\n    \"satelliteId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Uuid\"\n        },\n        {\n          \"description\": \"UUID of a satellite.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-ground-station/refs/heads/main/json-schema/ground-station-satellite-list-item-schema.json
tags:
- AWS
- Data Processing
- IoT
- Satellite Communications
- Space Technology
title: SatelliteListItem
---
