---
description: DescribeMatchmakingInput schema from Amazon GameLift API
layout: schema
name: DescribeMatchmakingInput
properties_list:
- description: ''
  name: TicketIds
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-matchmaking-input-schema.json
slug: gamelift-describe-matchmaking-input
source_filename: gamelift-describe-matchmaking-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-input-schema.json\",\n  \"title\": \"DescribeMatchmakingInput\",\n  \"description\": \"DescribeMatchmakingInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TicketIds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MatchmakingIdList\"\n        },\n        {\n          \"description\": \"A unique identifier for a matchmaking ticket. You can include up to 10 ID values. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TicketIds\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-matchmaking-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeMatchmakingInput
---
