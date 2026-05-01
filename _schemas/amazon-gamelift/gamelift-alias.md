---
description: <p>Properties that describe an alias resource.</p> <p> <b>Related actions</b> </p> <p> <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets">All APIs by task</a> </p>
layout: schema
name: Alias
properties_list:
- description: ''
  name: AliasId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: AliasArn
  type: object
- description: ''
  name: Description
  type: object
- description: ''
  name: RoutingStrategy
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: LastUpdatedTime
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-alias-schema.json
slug: gamelift-alias
source_filename: gamelift-alias-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-alias-schema.json\",\n  \"title\": \"Alias\",\n  \"description\": \"<p>Properties that describe an alias resource.</p> <p> <b>Related actions</b> </p> <p> <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets\\\">All APIs by task</a> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AliasId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasId\"\n        },\n        {\n          \"description\": \"A unique identifier for the alias. Alias IDs are unique within a Region.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonBlankAndLengthConstraintString\"\n        },\n        {\n          \"description\": \"\
  A descriptive label that is associated with an alias. Alias names do not need to be unique.\"\n        }\n      ]\n    },\n    \"AliasArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AliasArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that is assigned to a Amazon GameLift alias resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::alias/alias-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>. In a GameLift alias ARN, the resource ID matches the alias ID value.\"\n        }\n      ]\n    },\n    \"Description\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FreeText\"\n        },\n        {\n          \"description\": \"A human-readable description of an alias.\"\n        }\n      ]\n    },\n    \"RoutingStrategy\": {\n      \"allOf\"\
  : [\n        {\n          \"$ref\": \"#/components/schemas/RoutingStrategy\"\n        },\n        {\n          \"description\": \"The routing configuration, including routing type and fleet target, for the alias. \"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp indicating when this data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"LastUpdatedTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time that this data object was last modified. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-alias-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: Alias
---
