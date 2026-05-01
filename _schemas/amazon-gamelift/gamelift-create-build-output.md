---
description: CreateBuildOutput schema from Amazon GameLift API
layout: schema
name: CreateBuildOutput
properties_list:
- description: ''
  name: Build
  type: object
- description: ''
  name: UploadCredentials
  type: object
- description: ''
  name: StorageLocation
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-build-output-schema.json
slug: gamelift-create-build-output
source_filename: gamelift-create-build-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-build-output-schema.json\",\n  \"title\": \"CreateBuildOutput\",\n  \"description\": \"CreateBuildOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Build\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Build\"\n        },\n        {\n          \"description\": \"The newly created build resource, including a unique build IDs and status. \"\n        }\n      ]\n    },\n    \"UploadCredentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCredentials\"\n        },\n        {\n          \"description\": \"This element is returned only when the operation is called without a storage location. It contains credentials to use when you are uploading a build file to an Amazon S3 bucket\
  \ that is owned by Amazon GameLift. Credentials have a limited life span. To refresh these credentials, call <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_RequestUploadCredentials.html\\\">RequestUploadCredentials</a>. \"\n        }\n      ]\n    },\n    \"StorageLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"Amazon S3 location for your game build file, including bucket name and key.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-build-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateBuildOutput
---
