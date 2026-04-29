---
description: Output details listed for an action execution, such as the action execution result.
layout: schema
name: ActionExecutionOutput
properties_list:
- description: ''
  name: outputArtifacts
  type: object
- description: ''
  name: executionResult
  type: object
- description: ''
  name: outputVariables
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-execution-output-schema.json
slug: amazon-codepipeline-action-execution-output
source_filename: amazon-codepipeline-action-execution-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-output-schema.json\",\n  \"title\": \"ActionExecutionOutput\",\n  \"description\": \"Output details listed for an action execution, such as the action execution result.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"outputArtifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactDetailList\"\n        },\n        {\n          \"description\": \"Details of output artifacts of the action that correspond to the action execution.\"\n        }\n      ]\n    },\n    \"executionResult\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionResult\"\n        },\n        {\n          \"description\": \"Execution result information listed in the output details for an action execution.\"\
  \n        }\n      ]\n    },\n    \"outputVariables\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OutputVariablesMap\"\n        },\n        {\n          \"description\": \"The outputVariables field shows the key-value pairs that were output as part of that execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionExecutionOutput
---
