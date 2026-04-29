---
description: Represents the output of a <code>GetPipelineState</code> action.
layout: schema
name: GetPipelineStateOutput
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: pipelineVersion
  type: object
- description: ''
  name: stageStates
  type: object
- description: ''
  name: created
  type: object
- description: ''
  name: updated
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-get-pipeline-state-output-schema.json
slug: amazon-codepipeline-get-pipeline-state-output
source_filename: amazon-codepipeline-get-pipeline-state-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-state-output-schema.json\",\n  \"title\": \"GetPipelineStateOutput\",\n  \"description\": \"Represents the output of a <code>GetPipelineState</code> action.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline for which you want to get the state.\"\n        }\n      ]\n    },\n    \"pipelineVersion\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineVersion\"\n        },\n        {\n          \"description\": \"<p>The version number of the pipeline.</p> <note> <p>A newly created pipeline is always assigned a version number of <code>1</code>.</p>\
  \ </note>\"\n        }\n      ]\n    },\n    \"stageStates\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageStateList\"\n        },\n        {\n          \"description\": \"A list of the pipeline stage output information, including stage name, state, most recent run details, whether the stage is disabled, and other data.\"\n        }\n      ]\n    },\n    \"created\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the pipeline was created, in timestamp format.\"\n        }\n      ]\n    },\n    \"updated\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time the pipeline was last updated, in timestamp format.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-get-pipeline-state-output-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: GetPipelineStateOutput
---
