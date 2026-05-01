---
description: GetActionTypeOutput schema from Amazon CodePipeline
layout: schema
name: GetActionTypeOutput
properties_list:
- description: ''
  name: actionType
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-action-type-output-schema.json
slug: amazon-codepipeline-get-action-type-output
source_filename: amazon-codepipeline-get-action-type-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-action-type-output-schema.json\",\n  \"title\": \"GetActionTypeOutput\",\n  \"description\": \"GetActionTypeOutput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeDeclaration\"\n        },\n        {\n          \"description\": \"The action type information for the requested action type, such as the action type ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-action-type-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetActionTypeOutput
---
