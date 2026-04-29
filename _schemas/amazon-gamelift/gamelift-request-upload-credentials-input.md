---
description: RequestUploadCredentialsInput schema from Amazon GameLift API
layout: schema
name: RequestUploadCredentialsInput
properties_list:
- description: ''
  name: BuildId
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-request-upload-credentials-input-schema.json
slug: gamelift-request-upload-credentials-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-request-upload-credentials-input-schema.json\",\n  \"title\": \"RequestUploadCredentialsInput\",\n  \"description\": \"RequestUploadCredentialsInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BuildId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the build to get credentials for. You can use either the build ID or ARN value. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"BuildId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-request-upload-credentials-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: RequestUploadCredentialsInput
---
