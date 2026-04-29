---
description: PlayerIdList schema from Amazon GameLift API
layout: schema
name: PlayerIdList
properties_list: []
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-player-id-list-schema.json
slug: gamelift-player-id-list
source_filename: gamelift-player-id-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-player-id-list-schema.json\",\n  \"title\": \"PlayerIdList\",\n  \"description\": \"PlayerIdList schema from Amazon GameLift API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 25\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-player-id-list-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: PlayerIdList
---
