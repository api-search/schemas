---
description: StageDeclaration schema from Amazon CodePipeline
layout: schema
name: StageDeclaration
properties_list:
- description: The name of the stage.
  name: name
  type: string
- description: ''
  name: actions
  type: array
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-stage-declaration-schema.json
slug: amazon-codepipeline-stage-declaration
source_filename: amazon-codepipeline-stage-declaration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stage-declaration-schema.json\",\n  \"title\": \"StageDeclaration\",\n  \"description\": \"StageDeclaration schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the stage.\"\n    },\n    \"actions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ActionDeclaration\"\n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"actions\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stage-declaration-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StageDeclaration
---
