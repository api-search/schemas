---
description: UpdateBuildInput schema from Amazon GameLift API
layout: schema
name: UpdateBuildInput
properties_list:
- description: ''
  name: BuildId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Version
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-update-build-input-schema.json
slug: gamelift-update-build-input
source_filename: gamelift-update-build-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-build-input-schema.json\",\n  \"title\": \"UpdateBuildInput\",\n  \"description\": \"UpdateBuildInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BuildId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the build to update. You can use either the build ID or ARN value. \"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label associated with a build. Build names don't need to be unique. \"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n       \
  \ {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Version information associated with a build or script. Version strings don't need to be unique.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BuildId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-update-build-input-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UpdateBuildInput
---
