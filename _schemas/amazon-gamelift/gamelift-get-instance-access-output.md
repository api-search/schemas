---
description: GetInstanceAccessOutput schema from Amazon GameLift API
layout: schema
name: GetInstanceAccessOutput
properties_list:
- description: ''
  name: InstanceAccess
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-get-instance-access-output-schema.json
slug: gamelift-get-instance-access-output
source_filename: gamelift-get-instance-access-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-instance-access-output-schema.json\",\n  \"title\": \"GetInstanceAccessOutput\",\n  \"description\": \"GetInstanceAccessOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InstanceAccess\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InstanceAccess\"\n        },\n        {\n          \"description\": \"The connection information for a fleet instance, including IP address and access credentials.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-instance-access-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GetInstanceAccessOutput
---
