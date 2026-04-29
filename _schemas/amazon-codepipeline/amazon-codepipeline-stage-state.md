---
description: Represents information about the state of the stage.
layout: schema
name: StageState
properties_list:
- description: ''
  name: stageName
  type: object
- description: ''
  name: inboundExecution
  type: object
- description: ''
  name: inboundTransitionState
  type: object
- description: ''
  name: actionStates
  type: object
- description: ''
  name: latestExecution
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-stage-state-schema.json
slug: amazon-codepipeline-stage-state
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stage-state-schema.json\",\n  \"title\": \"StageState\",\n  \"description\": \"Represents information about the state of the stage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageName\"\n        },\n        {\n          \"description\": \"The name of the stage.\"\n        }\n      ]\n    },\n    \"inboundExecution\": {\n      \"$ref\": \"#/components/schemas/StageExecution\"\n    },\n    \"inboundTransitionState\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TransitionState\"\n        },\n        {\n          \"description\": \"The state of the inbound transition, which is either enabled or disabled.\"\n        }\n      ]\n    },\n    \"actionStates\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionStateList\"\n        },\n        {\n          \"description\": \"The state of the stage.\"\n        }\n      ]\n    },\n    \"latestExecution\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageExecution\"\n        },\n        {\n          \"description\": \"Information about the latest execution in the stage, including its ID and status.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stage-state-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StageState
---
