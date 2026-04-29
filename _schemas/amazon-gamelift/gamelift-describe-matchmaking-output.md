---
description: DescribeMatchmakingOutput schema from Amazon GameLift API
layout: schema
name: DescribeMatchmakingOutput
properties_list:
- description: ''
  name: TicketList
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-matchmaking-output-schema.json
slug: gamelift-describe-matchmaking-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-output-schema.json\",\n  \"title\": \"DescribeMatchmakingOutput\",\n  \"description\": \"DescribeMatchmakingOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TicketList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingTicketList\"\n        },\n        {\n          \"description\": \"A collection of existing matchmaking ticket objects matching the request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeMatchmakingOutput
---
