---
description: DescribeVpcPeeringConnectionsInput schema from Amazon GameLift API
layout: schema
name: DescribeVpcPeeringConnectionsInput
properties_list:
- description: ''
  name: FleetId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-vpc-peering-connections-input-schema.json
slug: gamelift-describe-vpc-peering-connections-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-vpc-peering-connections-input-schema.json\",\n  \"title\": \"DescribeVpcPeeringConnectionsInput\",\n  \"description\": \"DescribeVpcPeeringConnectionsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-vpc-peering-connections-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeVpcPeeringConnectionsInput
---
