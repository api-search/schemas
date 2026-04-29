---
description: StopPipelineExecutionInput schema from Amazon CodePipeline
layout: schema
name: StopPipelineExecutionInput
properties_list:
- description: ''
  name: pipelineName
  type: object
- description: ''
  name: pipelineExecutionId
  type: object
- description: ''
  name: abandon
  type: object
- description: ''
  name: reason
  type: object
provider_name: Amazon CodePipeline
provider_slug: amazon-codepipeline
schema_file: json-schema/amazon-codepipeline-stop-pipeline-execution-input-schema.json
slug: amazon-codepipeline-stop-pipeline-execution-input
source_filename: amazon-codepipeline-stop-pipeline-execution-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stop-pipeline-execution-input-schema.json\",\n  \"title\": \"StopPipelineExecutionInput\",\n  \"description\": \"StopPipelineExecutionInput schema from Amazon CodePipeline\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"pipelineName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineName\"\n        },\n        {\n          \"description\": \"The name of the pipeline to stop.\"\n        }\n      ]\n    },\n    \"pipelineExecutionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipelineExecutionId\"\n        },\n        {\n          \"description\": \"The ID of the pipeline execution to be stopped in the current stage. Use the <code>GetPipelineState</code> action to retrieve the current pipelineExecutionId.\"\
  \n        }\n      ]\n    },\n    \"abandon\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"<p>Use this option to stop the pipeline execution by abandoning, rather than finishing, in-progress actions.</p> <note> <p>This option can lead to failed or out-of-sequence tasks.</p> </note>\"\n        }\n      ]\n    },\n    \"reason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StopPipelineExecutionReason\"\n        },\n        {\n          \"description\": \"Use this option to enter comments, such as the reason the pipeline was stopped.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"pipelineName\",\n    \"pipelineExecutionId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-codepipeline/refs/heads/main/json-schema/amazon-codepipeline-stop-pipeline-execution-input-schema.json
tags:
- Amazon
- AWS
- CI/CD
- Continuous Delivery
- DevOps
- Pipeline
- Release Automation
title: StopPipelineExecutionInput
---
