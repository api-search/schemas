---
description: ResolveAliasInput schema from Amazon GameLift API
layout: schema
name: ResolveAliasInput
properties_list:
- description: ''
  name: AliasId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-resolve-alias-input-schema.json
slug: gamelift-resolve-alias-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-resolve-alias-input-schema.json\",\n  \"title\": \"ResolveAliasInput\",\n  \"description\": \"ResolveAliasInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasIdOrArn\"\n        },\n        {\n          \"description\": \"The unique identifier of the alias that you want to retrieve a fleet ID for. You can use either the alias ID or ARN value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AliasId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-resolve-alias-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: ResolveAliasInput
---
