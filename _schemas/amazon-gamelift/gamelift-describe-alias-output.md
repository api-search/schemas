---
description: DescribeAliasOutput schema from Amazon GameLift API
layout: schema
name: DescribeAliasOutput
properties_list:
- description: ''
  name: Alias
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-describe-alias-output-schema.json
slug: gamelift-describe-alias-output
source_filename: gamelift-describe-alias-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-alias-output-schema.json\",\n  \"title\": \"DescribeAliasOutput\",\n  \"description\": \"DescribeAliasOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Alias\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Alias\"\n        },\n        {\n          \"description\": \"The requested alias resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-describe-alias-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: DescribeAliasOutput
---
