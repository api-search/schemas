---
description: Temporary access credentials used for uploading game build files to Amazon GameLift. They are valid for a limited time. If they expire before you upload your game build, get a new set by calling <a href="https://docs.aws.amazon.com/gamelift/latest/apireference/API_RequestUploadCredentials.html">RequestUploadCredentials</a>.
layout: schema
name: AwsCredentials
properties_list:
- description: ''
  name: AccessKeyId
  type: object
- description: ''
  name: SecretAccessKey
  type: object
- description: ''
  name: SessionToken
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-aws-credentials-schema.json
slug: gamelift-aws-credentials
source_filename: gamelift-aws-credentials-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-aws-credentials-schema.json\",\n  \"title\": \"AwsCredentials\",\n  \"description\": \"Temporary access credentials used for uploading game build files to Amazon GameLift. They are valid for a limited time. If they expire before you upload your game build, get a new set by calling <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_RequestUploadCredentials.html\\\">RequestUploadCredentials</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AccessKeyId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Temporary key allowing access to the Amazon GameLift S3 account.\"\n        }\n      ]\n    },\n    \"SecretAccessKey\": {\n      \"allOf\": [\n        {\n          \"\
  $ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Temporary secret key allowing access to the Amazon GameLift S3 account.\"\n        }\n      ]\n    },\n    \"SessionToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"Token used to associate a specific build ID with the files uploaded using these credentials.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-aws-credentials-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: AwsCredentials
---
