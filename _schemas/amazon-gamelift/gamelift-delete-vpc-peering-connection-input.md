---
description: DeleteVpcPeeringConnectionInput schema from Amazon GameLift API
layout: schema
name: DeleteVpcPeeringConnectionInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: VpcPeeringConnectionId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-vpc-peering-connection-input-schema.json
slug: gamelift-delete-vpc-peering-connection-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-vpc-peering-connection-input-schema.json\",\n  \"title\": \"DeleteVpcPeeringConnectionInput\",\n  \"description\": \"DeleteVpcPeeringConnectionInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet. This fleet specified must match the fleet referenced in the VPC peering connection record. You can use either the fleet ID or ARN value.\"\n        }\n      ]\n    },\n    \"VpcPeeringConnectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for\
  \ a VPC peering connection.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"VpcPeeringConnectionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-vpc-peering-connection-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteVpcPeeringConnectionInput
---
