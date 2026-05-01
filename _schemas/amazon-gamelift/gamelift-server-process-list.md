---
description: ServerProcessList schema from Amazon GameLift API
layout: schema
name: ServerProcessList
properties_list: []
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-server-process-list-schema.json
slug: gamelift-server-process-list
source_filename: gamelift-server-process-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-server-process-list-schema.json\",\n  \"title\": \"ServerProcessList\",\n  \"description\": \"ServerProcessList schema from Amazon GameLift API\",\n  \"type\": \"array\",\n  \"items\": {\n    \"$ref\": \"#/components/schemas/ServerProcess\"\n  },\n  \"minItems\": 1,\n  \"maxItems\": 50\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-server-process-list-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ServerProcessList
---
