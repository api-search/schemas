---
description: <p>Properties describing a custom game build.</p> <p> <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets">All APIs by task</a> </p>
layout: schema
name: Build
properties_list:
- description: ''
  name: BuildId
  type: object
- description: ''
  name: BuildArn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: SizeOnDisk
  type: object
- description: ''
  name: OperatingSystem
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: ServerSdkVersion
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-build-schema.json
slug: gamelift-build
source_filename: gamelift-build-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-build-schema.json\",\n  \"title\": \"Build\",\n  \"description\": \"<p>Properties describing a custom game build.</p> <p> <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets\\\">All APIs by task</a> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BuildId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildId\"\n        },\n        {\n          \"description\": \"A unique identifier for the build.\"\n        }\n      ]\n    },\n    \"BuildArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\
  \">ARN</a>) assigned to a Amazon GameLift build resource and uniquely identifies it. ARNs are unique across all Regions. Format is <code>arn:aws:gamelift:&lt;region&gt;::build/build-a1234567-b8c9-0d1e-2fa3-b45c6d7e8912</code>. In a GameLift build ARN, the resource ID matches the <i>BuildId</i> value.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FreeText\"\n        },\n        {\n          \"description\": \"A descriptive label associated with a build. Build names don't need to be unique. It can be set using <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_CreateBuild.html\\\">CreateBuild</a> or <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/UpdateBuild\\\">UpdateBuild</a>.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FreeText\"\n        },\n        {\n          \"description\": \"Version\
  \ information associated with a build or script. Version strings don't need to be unique.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BuildStatus\"\n        },\n        {\n          \"description\": \"<p>Current status of the build.</p> <p>Possible build statuses include the following:</p> <ul> <li> <p> <b>INITIALIZED</b> -- A new build has been defined, but no files have been uploaded. You cannot create fleets for builds that are in this status. When a build is successfully created, the build status is set to this value. </p> </li> <li> <p> <b>READY</b> -- The game build has been successfully uploaded. You can now create new fleets for this build.</p> </li> <li> <p> <b>FAILED</b> -- The game build upload failed. You cannot create new fleets for this build. </p> </li> </ul>\"\n        }\n      ]\n    },\n    \"SizeOnDisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveLong\"\
  \n        },\n        {\n          \"description\": \"File size of the uploaded game build, expressed in bytes. When the build status is <code>INITIALIZED</code> or when using a custom Amazon S3 storage location, this value is 0.\"\n        }\n      ]\n    },\n    \"OperatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperatingSystem\"\n        },\n        {\n          \"description\": \"Operating system that the game server binaries are built to run on. This value determines the type of fleet resources that you can use for this build.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp indicating when this data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"ServerSdkVersion\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerSdkVersion\"\n        },\n        {\n          \"description\": \"The Amazon GameLift Server SDK version used to develop your game server.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-build-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: Build
---
