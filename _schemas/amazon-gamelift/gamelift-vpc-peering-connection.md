---
description: <p>Represents a peering connection between a VPC on one of your Amazon Web Services accounts and the VPC for your Amazon GameLift fleets. This record may be for an active peering connection or a pending connection that has not yet been established.</p> <p> <b>Related actions</b> </p> <p> <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets">All APIs by task</a> </p>
layout: schema
name: VpcPeeringConnection
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: IpV4CidrBlock
  type: object
- description: ''
  name: VpcPeeringConnectionId
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: PeerVpcId
  type: object
- description: ''
  name: GameLiftVpcId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-vpc-peering-connection-schema.json
slug: gamelift-vpc-peering-connection
source_filename: gamelift-vpc-peering-connection-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-vpc-peering-connection-schema.json\",\n  \"title\": \"VpcPeeringConnection\",\n  \"description\": \"<p>Represents a peering connection between a VPC on one of your Amazon Web Services accounts and the VPC for your Amazon GameLift fleets. This record may be for an active peering connection or a pending connection that has not yet been established.</p> <p> <b>Related actions</b> </p> <p> <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets\\\">All APIs by task</a> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet. This ID determines\
  \ the ID of the Amazon GameLift VPC for your fleet.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) associated with the GameLift fleet resource for this connection. \"\n        }\n      ]\n    },\n    \"IpV4CidrBlock\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"CIDR block of IPv4 addresses assigned to the VPC peering connection for the GameLift VPC. The peered VPC also has an IPv4 CIDR block associated with it; these blocks cannot overlap or the peering connection cannot be created. \"\n        }\n      ]\n    },\n    \"VpcPeeringConnectionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\
  \n        },\n        {\n          \"description\": \"A unique identifier that is automatically assigned to the connection record. This ID is referenced in VPC peering connection events, and is used when deleting a connection.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcPeeringConnectionStatus\"\n        },\n        {\n          \"description\": \"The status information about the connection. Status indicates if a connection is pending, successful, or failed.\"\n        }\n      ]\n    },\n    \"PeerVpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for a VPC with resources to be accessed by your Amazon GameLift fleet. The VPC must be in the same Region as your fleet. To look up a VPC ID, use the <a href=\\\"https://console.aws.amazon.com/vpc/\\\">VPC Dashboard</a> in the Amazon\
  \ Web Services Management Console. Learn more about VPC peering in <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/vpc-peering.html\\\">VPC Peering with Amazon GameLift Fleets</a>.\"\n        }\n      ]\n    },\n    \"GameLiftVpcId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A unique identifier for the VPC that contains the Amazon GameLift fleet for this connection. This VPC is managed by Amazon GameLift and does not appear in your Amazon Web Services account. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-vpc-peering-connection-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: VpcPeeringConnection
---
