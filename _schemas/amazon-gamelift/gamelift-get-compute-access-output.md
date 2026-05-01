---
description: GetComputeAccessOutput schema from Amazon GameLift API
layout: schema
name: GetComputeAccessOutput
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: ComputeName
  type: object
- description: ''
  name: ComputeArn
  type: object
- description: ''
  name: Credentials
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-get-compute-access-output-schema.json
slug: gamelift-get-compute-access-output
source_filename: gamelift-get-compute-access-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-compute-access-output-schema.json\",\n  \"title\": \"GetComputeAccessOutput\",\n  \"description\": \"GetComputeAccessOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"The fleet ID of compute resource.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift fleet resource and uniquely identifies it. ARNs are\
  \ unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::fleet/fleet-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>.\"\n        }\n      ]\n    },\n    \"ComputeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeNameOrArn\"\n        },\n        {\n          \"description\": \"The name of the compute resource you requested credentials for.\"\n        }\n      ]\n    },\n    \"ComputeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift compute resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::compute/compute-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>.\"\n        }\n      ]\n    },\n    \"Credentials\": {\n   \
  \   \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AwsCredentials\"\n        },\n        {\n          \"description\": \"The access credentials for the compute resource.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-compute-access-output-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GetComputeAccessOutput
---
