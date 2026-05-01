---
description: DescribeFleetLocationUtilizationOutput schema from Amazon GameLift API
layout: schema
name: DescribeFleetLocationUtilizationOutput
properties_list:
- description: ''
  name: FleetUtilization
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-fleet-location-utilization-output-schema.json
slug: gamelift-describe-fleet-location-utilization-output
source_filename: gamelift-describe-fleet-location-utilization-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-fleet-location-utilization-output-schema.json\",\n  \"title\": \"DescribeFleetLocationUtilizationOutput\",\n  \"description\": \"DescribeFleetLocationUtilizationOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetUtilization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetUtilization\"\n        },\n        {\n          \"description\": \"Utilization information for the requested fleet location. Utilization objects are returned only for fleets and locations that currently exist.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-fleet-location-utilization-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeFleetLocationUtilizationOutput
---
