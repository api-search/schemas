---
description: Represents the context of an action in the stage of a pipeline to a job worker.
layout: schema
name: ActionContext
properties_list:
- description: ''
  name: name
  type: object
- description: ''
  name: actionExecutionId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-context-schema.json
slug: amazon-codepipeline-action-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-context-schema.json\",\n  \"title\": \"ActionContext\",\n  \"description\": \"Represents the context of an action in the stage of a pipeline to a job worker.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionName\"\n        },\n        {\n          \"description\": \"The name of the action in the context of a job.\"\n        }\n      ]\n    },\n    \"actionExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionId\"\n        },\n        {\n          \"description\": \"The system-generated unique ID that corresponds to an action's execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-context-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionContext
---
