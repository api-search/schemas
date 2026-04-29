---
description: VpcSubnets schema from Amazon GameLift API
layout: schema
name: VpcSubnets
properties_list: []
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-vpc-subnets-schema.json
slug: gamelift-vpc-subnets
source_filename: gamelift-vpc-subnets-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-vpc-subnets-schema.json\",\n  \"title\": \"VpcSubnets\",\n  \"description\": \"VpcSubnets schema from Amazon GameLift API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/VpcSubnet\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 20\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-vpc-subnets-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: VpcSubnets
---
