---
description: Input information used for an action execution.
layout: schema
name: ActionExecutionInput
properties_list:
- description: ''
  name: actionTypeId
  type: object
- description: ''
  name: configuration
  type: object
- description: ''
  name: resolvedConfiguration
  type: object
- description: ''
  name: roleArn
  type: object
- description: ''
  name: region
  type: object
- description: ''
  name: inputArtifacts
  type: object
- description: ''
  name: namespace
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-action-execution-input-schema.json
slug: amazon-codepipeline-action-execution-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-input-schema.json\",\n  \"title\": \"ActionExecutionInput\",\n  \"description\": \"Input information used for an action execution.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"actionTypeId\": {\n      \"$ref\": \"#/components/schemas/ActionTypeId\"\n    },\n    \"configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionConfigurationMap\"\n        },\n        {\n          \"description\": \"Configuration data for an action execution.\"\n        }\n      ]\n    },\n    \"resolvedConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResolvedActionConfigurationMap\"\n        },\n        {\n          \"description\": \"Configuration data for an action execution with all variable\
  \ references replaced with their real values for the execution.\"\n        }\n      ]\n    },\n    \"roleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The ARN of the IAM service role that performs the declared action. This is assumed through the roleArn for the pipeline. \"\n        }\n      ]\n    },\n    \"region\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AWSRegionName\"\n        },\n        {\n          \"description\": \"The Amazon Web Services Region for the action, such as us-east-1.\"\n        }\n      ]\n    },\n    \"inputArtifacts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ArtifactDetailList\"\n        },\n        {\n          \"description\": \"Details of input artifacts of the action that correspond to the action execution.\"\n        }\n      ]\n    },\n    \"namespace\": {\n      \"allOf\": [\n     \
  \   {\n          \"$ref\": \"#/components/schemas/ActionNamespace\"\n        },\n        {\n          \"description\": \"The variable namespace associated with the action. All variables produced as output by this action fall under this namespace.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-action-execution-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: ActionExecutionInput
---
