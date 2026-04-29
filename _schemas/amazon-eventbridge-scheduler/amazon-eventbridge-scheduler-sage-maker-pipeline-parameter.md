---
description: The name and value pair of a parameter to use to start execution of a SageMaker Model Building Pipeline.
layout: schema
name: SageMakerPipelineParameter
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Value
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-sage-maker-pipeline-parameter-schema.json
slug: amazon-eventbridge-scheduler-sage-maker-pipeline-parameter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-sage-maker-pipeline-parameter-schema.json\",\n  \"title\": \"SageMakerPipelineParameter\",\n  \"description\": \"The name and value pair of a parameter to use to start execution of a SageMaker Model Building Pipeline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SageMakerPipelineParameterName\"\n        },\n        {\n          \"description\": \"Name of parameter to start execution of a SageMaker Model Building Pipeline.\"\n        }\n      ]\n    },\n    \"Value\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SageMakerPipelineParameterValue\"\n        },\n        {\n          \"description\": \"Value of parameter to start execution of\
  \ a SageMaker Model Building Pipeline.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-sage-maker-pipeline-parameter-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: SageMakerPipelineParameter
---
