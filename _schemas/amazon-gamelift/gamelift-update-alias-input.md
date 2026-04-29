---
description: UpdateAliasInput schema from Amazon GameLift API
layout: schema
name: UpdateAliasInput
properties_list:
- description: ''
  name: AliasId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: RoutingStrategy
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-alias-input-schema.json
slug: gamelift-update-alias-input
source_filename: gamelift-update-alias-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-alias-input-schema.json\",\n  \"title\": \"UpdateAliasInput\",\n  \"description\": \"UpdateAliasInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the alias that you want to update. You can use either the alias ID or ARN value.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonBlankAndLengthConstraintString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with an alias. Alias names do not need to be unique.\"\n        }\n      ]\n    },\n    \"Description\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A human-readable description of the alias.\"\n        }\n      ]\n    },\n    \"RoutingStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoutingStrategy\"\n        },\n        {\n          \"description\": \"The routing configuration, including routing type and fleet target, for the alias.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"AliasId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-alias-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateAliasInput
---
