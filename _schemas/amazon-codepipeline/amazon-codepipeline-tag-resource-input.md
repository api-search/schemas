---
description: TagResourceInput schema from Amazon CodePipeline
layout: schema
name: TagResourceInput
properties_list:
- description: ''
  name: resourceArn
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-tag-resource-input-schema.json
slug: amazon-codepipeline-tag-resource-input
source_filename: amazon-codepipeline-tag-resource-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-tag-resource-input-schema.json\",\n  \"title\": \"TagResourceInput\",\n  \"description\": \"TagResourceInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resourceArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the resource you want to add tags to.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"The tags you want to modify or add to the resource.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"resourceArn\",\n    \"tags\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-tag-resource-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: TagResourceInput
---
