---
description: The location in Amazon S3 where build or script files are stored for access by Amazon GameLift.
layout: schema
name: S3Location
properties_list:
- description: ''
  name: Bucket
  type: object
- description: ''
  name: Key
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: ObjectVersion
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-s3-location-schema.json
slug: gamelift-s3-location
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-s3-location-schema.json\",\n  \"title\": \"S3Location\",\n  \"description\": \"The location in Amazon S3 where build or script files are stored for access by Amazon GameLift.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Bucket\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"<p>An Amazon S3 bucket identifier. Thename of the S3 bucket.</p> <note> <p>Amazon GameLift doesn't support uploading from Amazon S3 buckets with names that contain a dot (.).</p> </note>\"\n        }\n      ]\n    },\n    \"Key\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The name of the zip file that contains\
  \ the build files or script files. \"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) for an IAM role that allows Amazon GameLift to access the S3 bucket.\"\n        }\n      ]\n    },\n    \"ObjectVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NonEmptyString\"\n        },\n        {\n          \"description\": \"The version of the file, if object versioning is turned on for the bucket. Amazon GameLift uses this information when retrieving files from an S3 bucket that you own. Use this parameter to specify a specific version of the file. If not set, the latest version of the file is retrieved. \"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-s3-location-schema.json
tags:
- AWS
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: S3Location
---
