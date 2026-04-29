---
description: Returns information about an execution of an action, including the action execution ID, and the name, version, and timing of the action.
layout: schema
name: ActionExecutionDetail
properties_list:
- description: ''
  name: pipelineExecutionId
  type: object
- description: ''
  name: actionExecutionId
  type: object
- description: ''
  name: pipelineVersion
  type: object
- description: ''
  name: stageName
  type: object
- description: ''
  name: actionName
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: lastUpdateTime
  type: object
- description: ''
  name: status
  type: object
- description: ''
  name: input
  type: object
- description: ''
  name: output
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-execution-detail-schema.json
slug: amazon-codepipeline-action-execution-detail
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-detail-schema.json\",\n  \"title\": \"ActionExecutionDetail\",\n  \"description\": \"Returns information about an execution of an action, including the action execution ID, and the name, version, and timing of the action. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The pipeline execution ID for the action execution.\"\n        }\n      ]\n    },\n    \"actionExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionId\"\n        },\n        {\n          \"description\": \"The action execution ID.\"\n        }\n      ]\n    },\n \
  \   \"pipelineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineVersion\"\n        },\n        {\n          \"description\": \"The version of the pipeline where the action was run.\"\n        }\n      ]\n    },\n    \"stageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageName\"\n        },\n        {\n          \"description\": \"The name of the stage that contains the action.\"\n        }\n      ]\n    },\n    \"actionName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionName\"\n        },\n        {\n          \"description\": \"The name of the action.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The start time of the action execution.\"\n        }\n      ]\n    },\n    \"lastUpdateTime\": {\n      \"allOf\": [\n    \
  \    {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The last update time of the action execution.\"\n        }\n      ]\n    },\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionStatus\"\n        },\n        {\n          \"description\": \" The status of the action execution. Status categories are <code>InProgress</code>, <code>Succeeded</code>, and <code>Failed</code>.\"\n        }\n      ]\n    },\n    \"input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionInput\"\n        },\n        {\n          \"description\": \"Input details for the action execution, such as role ARN, Region, and input artifacts.\"\n        }\n      ]\n    },\n    \"output\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionExecutionOutput\"\n        },\n        {\n          \"description\": \"Output details for\
  \ the action execution, such as the action execution result.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-detail-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionExecutionDetail
---
