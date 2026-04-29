---
description: CreateVpcPeeringAuthorizationOutput schema from Amazon GameLift API
layout: schema
name: CreateVpcPeeringAuthorizationOutput
properties_list:
- description: ''
  name: VpcPeeringAuthorization
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-vpc-peering-authorization-output-schema.json
slug: gamelift-create-vpc-peering-authorization-output
source_filename: gamelift-create-vpc-peering-authorization-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-vpc-peering-authorization-output-schema.json\",\n  \"title\": \"CreateVpcPeeringAuthorizationOutput\",\n  \"description\": \"CreateVpcPeeringAuthorizationOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcPeeringAuthorization\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcPeeringAuthorization\"\n        },\n        {\n          \"description\": \"Details on the requested VPC peering authorization, including expiration.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-vpc-peering-authorization-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateVpcPeeringAuthorizationOutput
---
