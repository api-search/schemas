---
description: CreateFleetLocationsInput schema from Amazon GameLift API
layout: schema
name: CreateFleetLocationsInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: Locations
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-fleet-locations-input-schema.json
slug: gamelift-create-fleet-locations-input
source_filename: gamelift-create-fleet-locations-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-fleet-locations-input-schema.json\",\n  \"title\": \"CreateFleetLocationsInput\",\n  \"description\": \"CreateFleetLocationsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to add locations to. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"Locations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationConfigurationList\"\n        },\n        {\n          \"description\": \"A list of locations to deploy additional instances to and manage as part of the fleet. You can add any Amazon GameLift-supported\
  \ Amazon Web Services Region as a remote location, in the form of an Amazon Web Services Region code such as <code>us-west-2</code>. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"Locations\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-fleet-locations-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateFleetLocationsInput
---
