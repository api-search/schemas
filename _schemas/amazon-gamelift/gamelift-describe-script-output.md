---
description: DescribeScriptOutput schema from Amazon GameLift API
layout: schema
name: DescribeScriptOutput
properties_list:
- description: ''
  name: Script
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-script-output-schema.json
slug: gamelift-describe-script-output
source_filename: gamelift-describe-script-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-script-output-schema.json\",\n  \"title\": \"DescribeScriptOutput\",\n  \"description\": \"DescribeScriptOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Script\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Script\"\n        },\n        {\n          \"description\": \"A set of properties describing the requested script.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-script-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeScriptOutput
---
