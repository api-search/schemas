---
description: <p>Properties describing a Realtime script.</p> <p> <b>Related actions</b> </p> <p> <a href="https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets">All APIs by task</a> </p>
layout: schema
name: Script
properties_list:
- description: ''
  name: ScriptId
  type: object
- description: ''
  name: ScriptArn
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: SizeOnDisk
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: StorageLocation
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-script-schema.json
slug: gamelift-script
source_filename: gamelift-script-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-script-schema.json\",\n  \"title\": \"Script\",\n  \"description\": \"<p>Properties describing a Realtime script.</p> <p> <b>Related actions</b> </p> <p> <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/reference-awssdk.html#reference-awssdk-resources-fleets\\\">All APIs by task</a> </p>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ScriptId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptId\"\n        },\n        {\n          \"description\": \"A unique identifier for the Realtime script\"\n        }\n      ]\n    },\n    \"ScriptArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ScriptArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\
  \">ARN</a>) that is assigned to a Amazon GameLift script resource and uniquely identifies it. ARNs are unique across all Regions. In a GameLift script ARN, the resource ID matches the <i>ScriptId</i> value.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label that is associated with a script. Script names don't need to be unique.\"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Version information associated with a build or script. Version strings don't need to be unique.\"\n        }\n      ]\n    },\n    \"SizeOnDisk\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PositiveLong\"\n        },\n        {\n          \"description\": \"The file size\
  \ of the uploaded Realtime script, expressed in bytes. When files are uploaded from an S3 location, this value remains at \\\"0\\\".\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"A time stamp indicating when this data object was created. Format is a number expressed in Unix time as milliseconds (for example <code>\\\"1469498468.057\\\"</code>).\"\n        }\n      ]\n    },\n    \"StorageLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"The location of the Amazon S3 bucket where a zipped file containing your Realtime scripts is stored. The storage location must specify the Amazon S3 bucket name, the zip file name (the \\\"key\\\"), and a role ARN that allows Amazon GameLift to access the Amazon S3 storage location. The S3 bucket must be\
  \ in the same Region where you want to create a new script. By default, Amazon GameLift uploads the latest version of the zip file; if you have S3 object versioning turned on, you can use the <code>ObjectVersion</code> parameter to specify an earlier version. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-script-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: Script
---
