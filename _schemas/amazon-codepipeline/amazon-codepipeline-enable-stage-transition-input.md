---
description: Represents the input of an <code>EnableStageTransition</code> action.
layout: schema
name: EnableStageTransitionInput
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: stageName
  type: object
- description: ''
  name: transitionType
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-enable-stage-transition-input-schema.json
slug: amazon-codepipeline-enable-stage-transition-input
source_filename: amazon-codepipeline-enable-stage-transition-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-enable-stage-transition-input-schema.json\",\n  \"title\": \"EnableStageTransitionInput\",\n  \"description\": \"Represents the input of an <code>EnableStageTransition</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline in which you want to enable the flow of artifacts from one stage to another.\"\n        }\n      ]\n    },\n    \"stageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageName\"\n        },\n        {\n          \"description\": \"The name of the stage where you want to enable the transition of artifacts, either into the stage\
  \ (inbound) or from that stage to the next stage (outbound).\"\n        }\n      ]\n    },\n    \"transitionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageTransitionType\"\n        },\n        {\n          \"description\": \"Specifies whether artifacts are allowed to enter the stage and be processed by the actions in that stage (inbound) or whether already processed artifacts are allowed to transition to the next stage (outbound).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipelineName\",\n    \"stageName\",\n    \"transitionType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-enable-stage-transition-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: EnableStageTransitionInput
---
