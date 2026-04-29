---
description: CreateFleetOutput schema from Amazon GameLift API
layout: schema
name: CreateFleetOutput
properties_list:
- description: ''
  name: FleetAttributes
  type: object
- description: ''
  name: LocationStates
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-fleet-output-schema.json
slug: gamelift-create-fleet-output
source_filename: gamelift-create-fleet-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-fleet-output-schema.json\",\n  \"title\": \"CreateFleetOutput\",\n  \"description\": \"CreateFleetOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetAttributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetAttributes\"\n        },\n        {\n          \"description\": \"The properties for the new fleet, including the current status. All fleets are placed in <code>NEW</code> status on creation. \"\n        }\n      ]\n    },\n    \"LocationStates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStateList\"\n        },\n        {\n          \"description\": \"The fleet's locations and life-cycle status of each location. For new fleets, the status of all locations\
  \ is set to <code>NEW</code>. During fleet creation, Amazon GameLift updates each location status as instances are deployed there and prepared for game hosting. This list includes an entry for the fleet's home Region. For fleets with no remote locations, only one entry, representing the home Region, is returned.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-fleet-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateFleetOutput
---
