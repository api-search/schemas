---
description: Represents the output of a <code>CreateCustomActionType</code> operation.
layout: schema
name: CreateCustomActionTypeOutput
properties_list:
- description: ''
  name: actionType
  type: object
- description: ''
  name: tags
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-create-custom-action-type-output-schema.json
slug: amazon-codepipeline-create-custom-action-type-output
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-create-custom-action-type-output-schema.json\",\n  \"title\": \"CreateCustomActionTypeOutput\",\n  \"description\": \"Represents the output of a <code>CreateCustomActionType</code> operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionType\"\n        },\n        {\n          \"description\": \"Returns information about the details of an action type.\"\n        }\n      ]\n    },\n    \"tags\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TagList\"\n        },\n        {\n          \"description\": \"Specifies the tags applied to the custom action.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"actionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-create-custom-action-type-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: CreateCustomActionTypeOutput
---
