---
description: UpdateActionTypeInput schema from Amazon CodePipeline
layout: schema
name: UpdateActionTypeInput
properties_list:
- description: ''
  name: actionType
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-update-action-type-input-schema.json
slug: amazon-codepipeline-update-action-type-input
source_filename: amazon-codepipeline-update-action-type-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-update-action-type-input-schema.json\",\n  \"title\": \"UpdateActionTypeInput\",\n  \"description\": \"UpdateActionTypeInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionTypeDeclaration\"\n        },\n        {\n          \"description\": \"The action type definition for the action type to be updated.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"actionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-update-action-type-input-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: UpdateActionTypeInput
---
