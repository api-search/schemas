---
description: Execution result information, such as the external execution ID.
layout: schema
name: ActionExecutionResult
properties_list:
- description: ''
  name: externalExecutionId
  type: object
- description: ''
  name: externalExecutionSummary
  type: object
- description: ''
  name: externalExecutionUrl
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-execution-result-schema.json
slug: amazon-codepipeline-action-execution-result
source_filename: amazon-codepipeline-action-execution-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-result-schema.json\",\n  \"title\": \"ActionExecutionResult\",\n  \"description\": \"Execution result information, such as the external execution ID.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalExecutionId\"\n        },\n        {\n          \"description\": \"The action provider's external ID for the action execution.\"\n        }\n      ]\n    },\n    \"externalExecutionSummary\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ExternalExecutionSummary\"\n        },\n        {\n          \"description\": \"The action provider's summary for the action execution.\"\n        }\n      ]\n    },\n    \"externalExecutionUrl\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Url\"\n        },\n        {\n          \"description\": \"The deepest external link to the external resource (for example, a repository URL or deployment endpoint) that is used when running the action.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-result-schema.json
tags:
- Amazon
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionExecutionResult
---
