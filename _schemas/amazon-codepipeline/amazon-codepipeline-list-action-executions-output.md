---
description: ListActionExecutionsOutput schema from Amazon CodePipeline
layout: schema
name: ListActionExecutionsOutput
properties_list:
- description: ''
  name: actionExecutionDetails
  type: object
- description: ''
  name: nextToken
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-list-action-executions-output-schema.json
slug: amazon-codepipeline-list-action-executions-output
source_filename: amazon-codepipeline-list-action-executions-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-action-executions-output-schema.json\",\n  \"title\": \"ListActionExecutionsOutput\",\n  \"description\": \"ListActionExecutionsOutput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionExecutionDetails\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionDetailList\"\n        },\n        {\n          \"description\": \"The details for a list of recent executions, such as action execution ID.\"\n        }\n      ]\n    },\n    \"nextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"If the amount of returned information is significantly large, an identifier is also returned and can be used in\
  \ a subsequent <code>ListActionExecutions</code> call to return the next set of action executions in the list.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-list-action-executions-output-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ListActionExecutionsOutput
---
