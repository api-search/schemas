---
description: UntagResourceInput schema from Amazon CodePipeline
layout: schema
name: UntagResourceInput
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: tagKeys
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-untag-resource-input-schema.json
slug: amazon-codepipeline-untag-resource-input
source_filename: amazon-codepipeline-untag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-untag-resource-input-schema.json\",\n  \"title\": \"UntagResourceInput\",\n  \"description\": \"UntagResourceInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \" The Amazon Resource Name (ARN) of the resource to remove tags from.\"\n        }\n      ]\n    },\n    \"tagKeys\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagKeyList\"\n        },\n        {\n          \"description\": \"The list of keys for the tags to be removed from the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\",\n    \"tagKeys\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-untag-resource-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: UntagResourceInput
---
