---
description: CreateVpcPeeringConnectionInput schema from Amazon GameLift API
layout: schema
name: CreateVpcPeeringConnectionInput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: PeerVpcAwsAccountId
  type: object
- description: ''
  name: PeerVpcId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-vpc-peering-connection-input-schema.json
slug: gamelift-create-vpc-peering-connection-input
source_filename: gamelift-create-vpc-peering-connection-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-vpc-peering-connection-input-schema.json\",\n  \"title\": \"CreateVpcPeeringConnectionInput\",\n  \"description\": \"CreateVpcPeeringConnectionInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet. You can use either the fleet ID or ARN value. This tells Amazon GameLift which GameLift VPC to peer with. \"\n        }\n      ]\n    },\n    \"PeerVpcAwsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for the Amazon Web Services account\
  \ with the VPC that you want to peer your Amazon GameLift fleet with. You can find your Account ID in the Amazon Web Services Management Console under account settings.\"\n        }\n      ]\n    },\n    \"PeerVpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a VPC with resources to be accessed by your Amazon GameLift fleet. The VPC must be in the same Region as your fleet. To look up a VPC ID, use the <a href=\\\"https://console.aws.amazon.com/vpc/\\\">VPC Dashboard</a> in the Amazon Web Services Management Console. Learn more about VPC peering in <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/vpc-peering.html\\\">VPC Peering with Amazon GameLift Fleets</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"FleetId\",\n    \"PeerVpcAwsAccountId\",\n    \"PeerVpcId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-vpc-peering-connection-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateVpcPeeringConnectionInput
---
