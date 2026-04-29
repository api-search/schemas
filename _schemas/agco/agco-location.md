---
description: Historical location data point for an AGCO machine.
layout: schema
name: MachineLocation
properties_list:
- description: Machine identifier.
  name: machine_id
  type: string
- description: Latitude in decimal degrees.
  name: latitude
  type: number
- description: Longitude in decimal degrees.
  name: longitude
  type: number
- description: Altitude in meters.
  name: altitude
  type: number
- description: Direction of travel in degrees (0-360).
  name: heading
  type: number
- description: Ground speed in km/h at this location.
  name: ground_speed
  type: number
- description: Location timestamp.
  name: timestamp
  type: string
provider_name: agco
provider_slug: agco
schema_file: json-schema/agco-location-schema.json
slug: agco-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/json-schema/agco-location-schema.json\",\n  \"title\": \"MachineLocation\",\n  \"description\": \"Historical location data point for an AGCO machine.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"machine_id\": {\n      \"type\": \"string\",\n      \"description\": \"Machine identifier.\",\n      \"example\": \"mach-500123\"\n    },\n    \"latitude\": {\n      \"type\": \"number\",\n      \"description\": \"Latitude in decimal degrees.\",\n      \"example\": 41.8781\n    },\n    \"longitude\": {\n      \"type\": \"number\",\n      \"description\": \"Longitude in decimal degrees.\",\n      \"example\": -87.6298\n    },\n    \"altitude\": {\n      \"type\": \"number\",\n      \"description\": \"Altitude in meters.\",\n      \"example\": 215.0\n    },\n    \"heading\": {\n      \"type\": \"number\",\n      \"description\"\
  : \"Direction of travel in degrees (0-360).\",\n      \"example\": 45.0\n    },\n    \"ground_speed\": {\n      \"type\": \"number\",\n      \"description\": \"Ground speed in km/h at this location.\",\n      \"example\": 8.5\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Location timestamp.\",\n      \"example\": \"2025-04-01T10:30:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/agco/refs/heads/main/json-schema/agco-location-schema.json
tags: []
title: MachineLocation
---
