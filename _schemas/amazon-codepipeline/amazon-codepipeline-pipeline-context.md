---
description: <p>Represents information about a pipeline to a job worker.</p> <note> <p>PipelineContext contains <code>pipelineArn</code> and <code>pipelineExecutionId</code> for custom action jobs. The <code>pipelineArn</code> and <code>pipelineExecutionId</code> fields are not populated for ThirdParty action jobs.</p> </note>
layout: schema
name: PipelineContext
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: stage
  type: object
- description: ''
  name: action
  type: object
- description: ''
  name: pipelineArn
  type: object
- description: ''
  name: pipelineExecutionId
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-pipeline-context-schema.json
slug: amazon-codepipeline-pipeline-context
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-context-schema.json\",\n  \"title\": \"PipelineContext\",\n  \"description\": \"<p>Represents information about a pipeline to a job worker.</p> <note> <p>PipelineContext contains <code>pipelineArn</code> and <code>pipelineExecutionId</code> for custom action jobs. The <code>pipelineArn</code> and <code>pipelineExecutionId</code> fields are not populated for ThirdParty action jobs.</p> </note>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline. This is a user-specified value. Pipeline names must be unique across all pipeline names under an Amazon Web Services account.\"\n        }\n\
  \      ]\n    },\n    \"stage\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StageContext\"\n        },\n        {\n          \"description\": \"The stage of the pipeline.\"\n        }\n      ]\n    },\n    \"action\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ActionContext\"\n        },\n        {\n          \"description\": \"The context of an action to a job worker in the stage of a pipeline.\"\n        }\n      ]\n    },\n    \"pipelineArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the pipeline.\"\n        }\n      ]\n    },\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The execution ID of the pipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-pipeline-context-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: PipelineContext
---
