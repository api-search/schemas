---
description: CreateBuildInput schema from Amazon GameLift API
layout: schema
name: CreateBuildInput
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Version
  type: object
- description: ''
  name: StorageLocation
  type: object
- description: ''
  name: OperatingSystem
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: ServerSdkVersion
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-create-build-input-schema.json
slug: gamelift-create-build-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-build-input-schema.json\",\n  \"title\": \"CreateBuildInput\",\n  \"description\": \"CreateBuildInput schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"A descriptive label associated with a build. Build names don't need to be unique. You can change this value later. \"\n        }\n      ]\n    },\n    \"Version\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonZeroAndMaxString\"\n        },\n        {\n          \"description\": \"Version information associated with a build or script. Version strings don't need to be unique. You can change this value later. \"\
  \n        }\n      ]\n    },\n    \"StorageLocation\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Location\"\n        },\n        {\n          \"description\": \"<p>Information indicating where your game build files are stored. Use this parameter only when creating a build with files stored in an Amazon S3 bucket that you own. The storage location must specify an Amazon S3 bucket name and key. The location must also specify a role ARN that you set up to allow Amazon GameLift to access your Amazon S3 bucket. The S3 bucket and your new build must be in the same Region.</p> <p>If a <code>StorageLocation</code> is specified, the size of your file can be found in your Amazon S3 bucket. Amazon GameLift will report a <code>SizeOnDisk</code> of 0. </p>\"\n        }\n      ]\n    },\n    \"OperatingSystem\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OperatingSystem\"\n        },\n        {\n          \"description\": \"The operating\
  \ system that you built the game server binaries to run on. This value determines the type of fleet resources that you can use for this build. If your game build contains multiple executables, they all must run on the same operating system. If an operating system isn't specified when creating a build, Amazon GameLift uses the default value (WINDOWS_2012). This value can't be changed later.\"\n        }\n      ]\n    },\n    \"Tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"A list of labels to assign to the new build resource. Tags are developer defined key-value pairs. Tagging Amazon Web Services resources are useful for resource management, access management and cost allocation. For more information, see <a href=\\\"https://docs.aws.amazon.com/general/latest/gr/aws_tagging.html\\\"> Tagging Amazon Web Services Resources</a> in the <i>Amazon Web Services General Reference</i>. Once the resource\
  \ is created, you can use <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_TagResource.html\\\">TagResource</a>, <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_UntagResource.html\\\">UntagResource</a>, and <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/apireference/API_ListTagsForResource.html\\\">ListTagsForResource</a> to add, remove, and view tags. The maximum tag limit may be lower than stated. See the Amazon Web Services General Reference for actual tagging limits.\"\n        }\n      ]\n    },\n    \"ServerSdkVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ServerSdkVersion\"\n        },\n        {\n          \"description\": \"A server SDK version you used when integrating your game server build with Amazon GameLift. For more information see <a href=\\\"https://docs.aws.amazon.com/gamelift/latest/developerguide/integration-custom-intro.html\\\">Integrate games with custom game servers</a>.\
  \ By default Amazon GameLift sets this value to <code>4.0.2</code>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-create-build-input-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: CreateBuildInput
---
