---
description: UntagResourceRequest schema from Amazon GameLift API
layout: schema
name: UntagResourceRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: TagKeys
  type: object
provider_name: Amazon GameLift
provider_slug: amazon-gamelift
schema_file: json-schema/gamelift-untag-resource-request-schema.json
slug: gamelift-untag-resource-request
source_filename: gamelift-untag-resource-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-untag-resource-request-schema.json\",\n  \"title\": \"UntagResourceRequest\",\n  \"description\": \"UntagResourceRequest schema from Amazon GameLift API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AmazonResourceName\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (<a href=\\\"https://docs.aws.amazon.com/AmazonS3/latest/dev/s3-arn-format.html\\\">ARN</a>) that uniquely identifies the Amazon GameLift resource that you want to remove tags from. Amazon GameLift includes resource ARNs in the data object for the resource. You can retrieve the ARN by calling a <code>List</code> or <code>Describe</code> operation for the resource type. \"\n        }\n      ]\n    },\n\
  \    \"TagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"A list of one or more tag keys to remove from the specified Amazon GameLift resource. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ResourceARN\",\n    \"TagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-gamelift/refs/heads/main/json-schema/gamelift-untag-resource-request-schema.json
tags:
- Cloud Computing
- Game Servers
- Gaming
- Multiplayer
- Matchmaking
- FlexMatch
- FleetIQ
title: UntagResourceRequest
---
