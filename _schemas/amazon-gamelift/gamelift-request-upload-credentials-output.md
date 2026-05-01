---
description: RequestUploadCredentialsOutput schema from Amazon GameLift API
layout: schema
name: RequestUploadCredentialsOutput
properties_list:
- description: ''
  name: UploadCredentials
  type: object
- description: ''
  name: StorageLocation
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-request-upload-credentials-output-schema.json
slug: gamelift-request-upload-credentials-output
source_filename: gamelift-request-upload-credentials-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-request-upload-credentials-output-schema.json\",\n  \"title\": \"RequestUploadCredentialsOutput\",\n  \"description\": \"RequestUploadCredentialsOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UploadCredentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCredentials\"\n        },\n        {\n          \"description\": \"Amazon Web Services credentials required when uploading a game build to the storage location. These credentials have a limited lifespan and are valid only for the build they were issued for.\"\n        }\n      ]\n    },\n    \"StorageLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"Amazon\
  \ S3 path and key, identifying where the game build files are stored.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-request-upload-credentials-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: RequestUploadCredentialsOutput
---
