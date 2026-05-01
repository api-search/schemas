---
description: <p>Current resource utilization statistics in a specified fleet or location. The location value might refer to a fleet's remote location or its home Region.</p> <p> <b>Related actions</b> </p>
layout: schema
name: FleetUtilization
properties_list:
- description: ''
  name: FleetId
  type: object
- description: ''
  name: FleetArn
  type: object
- description: ''
  name: ActiveServerProcessCount
  type: object
- description: ''
  name: ActiveGameSessionCount
  type: object
- description: ''
  name: CurrentPlayerSessionCount
  type: object
- description: ''
  name: MaximumPlayerSessionCount
  type: object
- description: ''
  name: Location
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-fleet-utilization-schema.json
slug: gamelift-fleet-utilization
source_filename: gamelift-fleet-utilization-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-fleet-utilization-schema.json\",\n  \"title\": \"FleetUtilization\",\n  \"description\": \"<p>Current resource utilization statistics in a specified fleet or location. The location value might refer to a fleet's remote location or its home Region.</p> <p> <b>Related actions</b> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FleetId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetId\"\n        },\n        {\n          \"description\": \"A unique identifier for the fleet associated with the location.\"\n        }\n      ]\n    },\n    \"FleetArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FleetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\
  \">ARN</a>) that is assigned to a Amazon GameLift fleet resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::fleet/fleet-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>.\"\n        }\n      ]\n    },\n    \"ActiveServerProcessCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The number of server processes in <code>ACTIVE</code> status that are currently running across all instances in the fleet location. \"\n        }\n      ]\n    },\n    \"ActiveGameSessionCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The number of active game sessions that are currently being hosted across all instances in the fleet location.\"\n        }\n      ]\n    },\n    \"CurrentPlayerSessionCount\": {\n      \"allOf\": [\n        {\n    \
  \      \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The number of active player sessions that are currently being hosted across all instances in the fleet location.\"\n        }\n      ]\n    },\n    \"MaximumPlayerSessionCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WholeNumber\"\n        },\n        {\n          \"description\": \"The maximum number of players allowed across all game sessions that are currently being hosted across all instances in the fleet location.\"\n        }\n      ]\n    },\n    \"Location\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LocationStringModel\"\n        },\n        {\n          \"description\": \"The fleet location for the fleet utilization information, expressed as an Amazon Web Services Region code, such as <code>us-west-2</code>. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-fleet-utilization-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: FleetUtilization
---
