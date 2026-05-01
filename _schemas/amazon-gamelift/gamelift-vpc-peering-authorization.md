---
description: <p>Represents an authorization for a VPC peering connection between the VPC for an Amazon GameLift fleet and another VPC on an account you have access to. This authorization must exist and be valid for the peering connection to be established. Authorizations are valid for 24 hours after they are issued.</p> <p> <b>Related actions</b> </p> <p> <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets">All APIs by task</a> </p>
layout: schema
name: VpcPeeringAuthorization
properties_list:
- description: ''
  name: GameLiftAwsAccountId
  type: object
- description: ''
  name: PeerVpcAwsAccountId
  type: object
- description: ''
  name: PeerVpcId
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: ExpirationTime
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-vpc-peering-authorization-schema.json
slug: gamelift-vpc-peering-authorization
source_filename: gamelift-vpc-peering-authorization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-vpc-peering-authorization-schema.json\",\n  \"title\": \"VpcPeeringAuthorization\",\n  \"description\": \"<p>Represents an authorization for a VPC peering connection between the VPC for an Amazon GameLift fleet and another VPC on an account you have access to. This authorization must exist and be valid for the peering connection to be established. Authorizations are valid for 24 hours after they are issued.</p> <p> <b>Related actions</b> </p> <p> <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets\\\">All APIs by task</a> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"GameLiftAwsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n   \
  \     {\n          \"description\": \"A unique identifier for the Amazon Web Services account that you use to manage your Amazon GameLift fleet. You can find your Account ID in the Amazon Web Services Management Console under account settings.\"\n        }\n      ]\n    },\n    \"PeerVpcAwsAccountId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"The authorization's peer VPC Amazon Web Services account ID.\"\n        }\n      ]\n    },\n    \"PeerVpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a VPC with resources to be accessed by your Amazon GameLift fleet. The VPC must be in the same Region as your fleet. To look up a VPC ID, use the <a href=\\\"https://console.aws.amazon.com/vpc/\\\">VPC Dashboard</a> in the Amazon Web Services Management Console.\
  \ Learn more about VPC peering in <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/vpc-peering.html\\\">VPC Peering with Amazon GameLift Fleets</a>.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Time stamp indicating when this authorization was issued. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"ExpirationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"Time stamp indicating when this authorization expires (24 hours after issuance). Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-vpc-peering-authorization-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: VpcPeeringAuthorization
---
