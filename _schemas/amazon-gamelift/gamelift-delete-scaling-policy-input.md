---
description: DeleteScalingPolicyInput schema from Amazon GameLift API
layout: schema
name: DeleteScalingPolicyInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: FleetId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-scaling-policy-input-schema.json
slug: gamelift-delete-scaling-policy-input
source_filename: gamelift-delete-scaling-policy-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-scaling-policy-input-schema.json\",\n  \"title\": \"DeleteScalingPolicyInput\",\n  \"description\": \"DeleteScalingPolicyInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a fleet's scaling policy. Policy names do not need to be unique.\"\n        }\n      ]\n    },\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet to be deleted. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n \
  \   }\n  },\n  \"required\": [\n    \"Name\",\n    \"FleetId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-scaling-policy-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteScalingPolicyInput
---
