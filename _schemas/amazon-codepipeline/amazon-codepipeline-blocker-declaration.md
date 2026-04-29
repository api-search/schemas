---
description: Reserved for future use.
layout: schema
name: BlockerDeclaration
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-blocker-declaration-schema.json
slug: amazon-codepipeline-blocker-declaration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-blocker-declaration-schema.json\",\n  \"title\": \"BlockerDeclaration\",\n  \"description\": \"Reserved for future use.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockerName\"\n        },\n        {\n          \"description\": \"Reserved for future use.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BlockerType\"\n        },\n        {\n          \"description\": \"Reserved for future use.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-blocker-declaration-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: BlockerDeclaration
---
