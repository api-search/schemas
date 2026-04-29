---
description: DescribeComputeInput schema from Amazon GameLift API
layout: schema
name: DescribeComputeInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: ComputeName
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-compute-input-schema.json
slug: gamelift-describe-compute-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-compute-input-schema.json\",\n  \"title\": \"DescribeComputeInput\",\n  \"description\": \"DescribeComputeInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet the compute is registered to.\"\n        }\n      ]\n    },\n    \"ComputeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeNameOrArn\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with the compute resource registered to your fleet.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"ComputeName\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-compute-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeComputeInput
---
