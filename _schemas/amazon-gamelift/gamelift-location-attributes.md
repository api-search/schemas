---
description: Details about a location in a multi-location fleet.
layout: schema
name: LocationAttributes
properties_list:
- description: ''
  name: LocationState
  type: object
- description: ''
  name: StoppedActions
  type: object
- description: ''
  name: UpdateStatus
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-location-attributes-schema.json
slug: gamelift-location-attributes
source_filename: gamelift-location-attributes-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-location-attributes-schema.json\",\n  \"title\": \"LocationAttributes\",\n  \"description\": \"Details about a location in a multi-location fleet.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LocationState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationState\"\n        },\n        {\n          \"description\": \"A fleet location and its current life-cycle state.\"\n        }\n      ]\n    },\n    \"StoppedActions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetActionList\"\n        },\n        {\n          \"description\": \"A list of fleet actions that have been suspended in the fleet location.\"\n        }\n      ]\n    },\n    \"UpdateStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationUpdateStatus\"\
  \n        },\n        {\n          \"description\": \"The status of fleet activity updates to the location. The status <code>PENDING_UPDATE</code> indicates that <code>StopFleetActions</code> or <code>StartFleetActions</code> has been requested but the update has not yet been completed for the location.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-location-attributes-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: LocationAttributes
---
