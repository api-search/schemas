---
description: DescribeComputeOutput schema from Amazon GameLift API
layout: schema
name: DescribeComputeOutput
properties_list:
- description: ''
  name: Compute
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-compute-output-schema.json
slug: gamelift-describe-compute-output
source_filename: gamelift-describe-compute-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-compute-output-schema.json\",\n  \"title\": \"DescribeComputeOutput\",\n  \"description\": \"DescribeComputeOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Compute\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Compute\"\n        },\n        {\n          \"description\": \"The details of the compute resource you registered to the specified fleet.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-compute-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeComputeOutput
---
