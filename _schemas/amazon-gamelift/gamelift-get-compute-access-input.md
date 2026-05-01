---
description: GetComputeAccessInput schema from Amazon GameLift API
layout: schema
name: GetComputeAccessInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: ComputeName
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-get-compute-access-input-schema.json
slug: gamelift-get-compute-access-input
source_filename: gamelift-get-compute-access-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-compute-access-input-schema.json\",\n  \"title\": \"GetComputeAccessInput\",\n  \"description\": \"GetComputeAccessInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet that the compute resource is registered to.\"\n        }\n      ]\n    },\n    \"ComputeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeNameOrArn\"\n        },\n        {\n          \"description\": \"The name of the compute resource you are requesting credentials for.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"ComputeName\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-compute-access-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GetComputeAccessInput
---
