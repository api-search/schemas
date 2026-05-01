---
description: DeleteVpcPeeringAuthorizationInput schema from Amazon GameLift API
layout: schema
name: DeleteVpcPeeringAuthorizationInput
properties_list:
- description: ''
  name: GameLiftAwsAccountId
  type: object
- description: ''
  name: PeerVpcId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-delete-vpc-peering-authorization-input-schema.json
slug: gamelift-delete-vpc-peering-authorization-input
source_filename: gamelift-delete-vpc-peering-authorization-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-vpc-peering-authorization-input-schema.json\",\n  \"title\": \"DeleteVpcPeeringAuthorizationInput\",\n  \"description\": \"DeleteVpcPeeringAuthorizationInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameLiftAwsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for the Amazon Web Services account that you use to manage your Amazon GameLift fleet. You can find your Account ID in the Amazon Web Services Management Console under account settings.\"\n        }\n      ]\n    },\n    \"PeerVpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n      \
  \  {\n          \"description\": \"A unique identifier for a VPC with resources to be accessed by your Amazon GameLift fleet. The VPC must be in the same Region as your fleet. To look up a VPC ID, use the <a href=\\\"https://console.aws.amazon.com/vpc/\\\">VPC Dashboard</a> in the Amazon Web Services Management Console. Learn more about VPC peering in <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/vpc-peering.html\\\">VPC Peering with Amazon GameLift Fleets</a>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"GameLiftAwsAccountId\",\n    \"PeerVpcId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-delete-vpc-peering-authorization-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DeleteVpcPeeringAuthorizationInput
---
