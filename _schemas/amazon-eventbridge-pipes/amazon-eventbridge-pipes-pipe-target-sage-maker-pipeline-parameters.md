---
description: The parameters for using a SageMaker pipeline as a target.
layout: schema
name: PipeTargetSageMakerPipelineParameters
properties_list:
- description: ''
  name: PipelineParameterList
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-sage-maker-pipeline-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-sage-maker-pipeline-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-sage-maker-pipeline-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-sage-maker-pipeline-parameters-schema.json\",\n  \"title\": \"PipeTargetSageMakerPipelineParameters\",\n  \"description\": \"The parameters for using a SageMaker pipeline as a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PipelineParameterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SageMakerPipelineParameterList\"\n        },\n        {\n          \"description\": \"List of Parameter names and values for SageMaker Model Building Pipeline execution.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-sage-maker-pipeline-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetSageMakerPipelineParameters
---
