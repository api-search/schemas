---
description: The parameters for using an Batch job as a target.
layout: schema
name: PipeTargetBatchJobParameters
properties_list:
- description: ''
  name: ArrayProperties
  type: object
- description: ''
  name: ContainerOverrides
  type: object
- description: ''
  name: DependsOn
  type: object
- description: ''
  name: JobDefinition
  type: object
- description: ''
  name: JobName
  type: object
- description: ''
  name: Parameters
  type: object
- description: ''
  name: RetryStrategy
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-batch-job-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-batch-job-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-batch-job-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-batch-job-parameters-schema.json\",\n  \"title\": \"PipeTargetBatchJobParameters\",\n  \"description\": \"The parameters for using an Batch job as a target.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ArrayProperties\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchArrayProperties\"\n        },\n        {\n          \"description\": \"The array properties for the submitted job, such as the size of the array. The array size can be between 2 and 10,000. If you specify array properties for a job, it becomes an array job. This parameter is used only if the target is an Batch job.\"\n        }\n      ]\n    },\n    \"ContainerOverrides\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchContainerOverrides\"\
  \n        },\n        {\n          \"description\": \"The overrides that are sent to a container.\"\n        }\n      ]\n    },\n    \"DependsOn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchDependsOn\"\n        },\n        {\n          \"description\": \"A list of dependencies for the job. A job can depend upon a maximum of 20 jobs. You can specify a <code>SEQUENTIAL</code> type dependency without specifying a job ID for array jobs so that each child array job completes sequentially, starting at index 0. You can also specify an <code>N_TO_N</code> type dependency with a job ID for array jobs. In that case, each index child of this job must wait for the corresponding index child of each dependency to complete before it can begin.\"\n        }\n      ]\n    },\n    \"JobDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The job definition used by this\
  \ job. This value can be one of <code>name</code>, <code>name:revision</code>, or the Amazon Resource Name (ARN) for the job definition. If name is specified without a revision then the latest active revision is used.\"\n        }\n      ]\n    },\n    \"JobName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The name of the job. It can be up to 128 letters long. The first character must be alphanumeric, can contain uppercase and lowercase letters, numbers, hyphens (-), and underscores (_).\"\n        }\n      ]\n    },\n    \"Parameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchParametersMap\"\n        },\n        {\n          \"description\": \"Additional parameters passed to the job that replace parameter substitution placeholders that are set in the job definition. Parameters are specified as a key and value pair mapping. Parameters included here\
  \ override any corresponding parameter defaults from the job definition.\"\n        }\n      ]\n    },\n    \"RetryStrategy\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/BatchRetryStrategy\"\n        },\n        {\n          \"description\": \"The retry strategy to use for failed jobs. When a retry strategy is specified here, it overrides the retry strategy defined in the job definition.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"JobDefinition\",\n    \"JobName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-batch-job-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetBatchJobParameters
---
