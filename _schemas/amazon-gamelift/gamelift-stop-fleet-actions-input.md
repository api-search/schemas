---
description: StopFleetActionsInput schema from Amazon GameLift API
layout: schema
name: StopFleetActionsInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: Actions
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-stop-fleet-actions-input-schema.json
slug: gamelift-stop-fleet-actions-input
source_filename: gamelift-stop-fleet-actions-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-stop-fleet-actions-input-schema.json\",\n  \"title\": \"StopFleetActionsInput\",\n  \"description\": \"StopFleetActionsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to stop actions on. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"Actions\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetActionList\"\n        },\n        {\n          \"description\": \"List of actions to suspend on the fleet. \"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The fleet location to stop fleet actions for. Specify a location in the form of an Amazon Web Services Region code, such as <code>us-west-2</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"Actions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-stop-fleet-actions-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: StopFleetActionsInput
---
