---
description: The templated target type for the Amazon SageMaker <a href="https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_StartPipelineExecution.html"> <code>StartPipelineExecution</code> </a> API operation.
layout: schema
name: SageMakerPipelineParameters
properties_list:
- description: ''
  name: PipelineParameterList
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-sage-maker-pipeline-parameters-schema.json
slug: amazon-eventbridge-scheduler-sage-maker-pipeline-parameters
source_filename: amazon-eventbridge-scheduler-sage-maker-pipeline-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-sage-maker-pipeline-parameters-schema.json\",\n  \"title\": \"SageMakerPipelineParameters\",\n  \"description\": \"The templated target type for the Amazon SageMaker <a href=\\\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_StartPipelineExecution.html\\\"> <code>StartPipelineExecution</code> </a> API operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PipelineParameterList\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SageMakerPipelineParameterList\"\n        },\n        {\n          \"description\": \"List of parameter names and values to use when executing the SageMaker Model Building Pipeline.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-sage-maker-pipeline-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: SageMakerPipelineParameters
---
