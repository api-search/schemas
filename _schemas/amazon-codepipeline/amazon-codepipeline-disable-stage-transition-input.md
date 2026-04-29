---
description: Represents the input of a <code>DisableStageTransition</code> action.
layout: schema
name: DisableStageTransitionInput
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
- description: ''
  name: reason
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-disable-stage-transition-input-schema.json
slug: amazon-codepipeline-disable-stage-transition-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-disable-stage-transition-input-schema.json\",\n  \"title\": \"DisableStageTransitionInput\",\n  \"description\": \"Represents the input of a <code>DisableStageTransition</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline in which you want to disable the flow of artifacts from one stage to another.\"\n        }\n      ]\n    },\n    \"stageName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageName\"\n        },\n        {\n          \"description\": \"The name of the stage where you want to disable the inbound or outbound transition of artifacts.\"\
  \n        }\n      ]\n    },\n    \"transitionType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageTransitionType\"\n        },\n        {\n          \"description\": \"Specifies whether artifacts are prevented from transitioning into the stage and being processed by the actions in that stage (inbound), or prevented from transitioning from the stage after they have been processed by the actions in that stage (outbound).\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DisabledReason\"\n        },\n        {\n          \"description\": \"The reason given to the user that a stage is disabled, such as waiting for manual approval or manual tests. This message is displayed in the pipeline console UI.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipelineName\",\n    \"stageName\",\n    \"transitionType\",\n    \"reason\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-disable-stage-transition-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: DisableStageTransitionInput
---
