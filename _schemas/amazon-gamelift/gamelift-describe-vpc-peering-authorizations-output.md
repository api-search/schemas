---
description: DescribeVpcPeeringAuthorizationsOutput schema from Amazon GameLift API
layout: schema
name: DescribeVpcPeeringAuthorizationsOutput
properties_list:
- description: ''
  name: VpcPeeringAuthorizations
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-vpc-peering-authorizations-output-schema.json
slug: gamelift-describe-vpc-peering-authorizations-output
source_filename: gamelift-describe-vpc-peering-authorizations-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-vpc-peering-authorizations-output-schema.json\",\n  \"title\": \"DescribeVpcPeeringAuthorizationsOutput\",\n  \"description\": \"DescribeVpcPeeringAuthorizationsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"VpcPeeringAuthorizations\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/VpcPeeringAuthorizationList\"\n        },\n        {\n          \"description\": \"A collection of objects that describe all valid VPC peering operations for the current Amazon Web Services account.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-vpc-peering-authorizations-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeVpcPeeringAuthorizationsOutput
---
