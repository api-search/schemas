---
description: GetInstanceAccessInput schema from Amazon GameLift API
layout: schema
name: GetInstanceAccessInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: InstanceId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-get-instance-access-input-schema.json
slug: gamelift-get-instance-access-input
source_filename: gamelift-get-instance-access-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-instance-access-input-schema.json\",\n  \"title\": \"GetInstanceAccessInput\",\n  \"description\": \"GetInstanceAccessInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet that contains the instance you want access to. You can use either the fleet ID or ARN value. The fleet can be in any of the following statuses: <code>ACTIVATING</code>, <code>ACTIVE</code>, or <code>ERROR</code>. Fleets with an <code>ERROR</code> status may be accessible for a short time before they are deleted.\"\n        }\n      ]\n    },\n    \"InstanceId\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/InstanceId\"\n        },\n        {\n          \"description\": \"A unique identifier for the instance you want to get access to. You can access an instance in any status.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"InstanceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-instance-access-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GetInstanceAccessInput
---
