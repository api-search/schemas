---
description: GetComputeAuthTokenOutput schema from Amazon GameLift API
layout: schema
name: GetComputeAuthTokenOutput
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
  name: AuthToken
  type: object
- description: ''
  name: ExpirationTimestamp
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-get-compute-auth-token-output-schema.json
slug: gamelift-get-compute-auth-token-output
source_filename: gamelift-get-compute-auth-token-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-compute-auth-token-output-schema.json\",\n  \"title\": \"GetComputeAuthTokenOutput\",\n  \"description\": \"GetComputeAuthTokenOutput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetIdOrArn\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet that the compute is registered to.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift fleet resource\
  \ and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::fleet/fleet-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>.\"\n        }\n      ]\n    },\n    \"ComputeName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeNameOrArn\"\n        },\n        {\n          \"description\": \"The name of the compute resource you are requesting the authentication token for.\"\n        }\n      ]\n    },\n    \"ComputeArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift compute resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::compute/compute-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code> \"\n\
  \        }\n      ]\n    },\n    \"AuthToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ComputeAuthToken\"\n        },\n        {\n          \"description\": \"The authentication token that your game server uses to authenticate with Amazon GameLift.\"\n        }\n      ]\n    },\n    \"ExpirationTimestamp\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The amount of time until the authentication token is no longer valid. To continue using the compute resource for game server hosting, renew the authentication token by using this operation again.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-get-compute-auth-token-output-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: GetComputeAuthTokenOutput
---
