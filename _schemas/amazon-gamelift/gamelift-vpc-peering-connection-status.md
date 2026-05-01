---
description: Represents status information for a VPC peering connection. Status codes and messages are provided from EC2 (see <a href="https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_VpcPeeringConnectionStateReason.html">VpcPeeringConnectionStateReason</a>). Connection status information is also communicated as a fleet event.
layout: schema
name: VpcPeeringConnectionStatus
properties_list:
- description: ''
  name: Code
  type: object
- description: ''
  name: Message
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-vpc-peering-connection-status-schema.json
slug: gamelift-vpc-peering-connection-status
source_filename: gamelift-vpc-peering-connection-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-vpc-peering-connection-status-schema.json\",\n  \"title\": \"VpcPeeringConnectionStatus\",\n  \"description\": \"Represents status information for a VPC peering connection. Status codes and messages are provided from EC2 (see <a href=\\\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_VpcPeeringConnectionStateReason.html\\\">VpcPeeringConnectionStateReason</a>). Connection status information is also communicated as a fleet event.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Code\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Code indicating the status of a VPC peering connection.\"\n        }\n      ]\n    },\n    \"Message\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Additional messaging associated with the connection status. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-vpc-peering-connection-status-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: VpcPeeringConnectionStatus
---
