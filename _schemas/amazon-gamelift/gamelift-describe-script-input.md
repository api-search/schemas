---
description: DescribeScriptInput schema from Amazon GameLift API
layout: schema
name: DescribeScriptInput
properties_list:
- description: ''
  name: ScriptId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-script-input-schema.json
slug: gamelift-describe-script-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-script-input-schema.json\",\n  \"title\": \"DescribeScriptInput\",\n  \"description\": \"DescribeScriptInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScriptId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the Realtime script to retrieve properties for. You can use either the script ID or ARN value.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ScriptId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-script-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeScriptInput
---
