---
description: The parameters required to set up a target for your pipe.
layout: schema
name: PipeTargetParameters
properties_list:
- description: ''
  name: BatchJobParameters
  type: object
- description: ''
  name: CloudWatchLogsParameters
  type: object
- description: ''
  name: EcsTaskParameters
  type: object
- description: ''
  name: EventBridgeEventBusParameters
  type: object
- description: ''
  name: HttpParameters
  type: object
- description: ''
  name: InputTemplate
  type: object
- description: ''
  name: KinesisStreamParameters
  type: object
- description: ''
  name: LambdaFunctionParameters
  type: object
- description: ''
  name: RedshiftDataParameters
  type: object
- description: ''
  name: SageMakerPipelineParameters
  type: object
- description: ''
  name: SqsQueueParameters
  type: object
- description: ''
  name: StepFunctionStateMachineParameters
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-parameters-schema.json\",\n  \"title\": \"PipeTargetParameters\",\n  \"description\": \"The parameters required to set up a target for your pipe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BatchJobParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetBatchJobParameters\"\n        },\n        {\n          \"description\": \"The parameters for using an Batch job as a target.\"\n        }\n      ]\n    },\n    \"CloudWatchLogsParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetCloudWatchLogsParameters\"\n        },\n        {\n          \"description\": \"The parameters for using an CloudWatch Logs log stream as a target.\"\n        }\n      ]\n    },\n\
  \    \"EcsTaskParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetEcsTaskParameters\"\n        },\n        {\n          \"description\": \"The parameters for using an Amazon ECS task as a target.\"\n        }\n      ]\n    },\n    \"EventBridgeEventBusParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetEventBridgeEventBusParameters\"\n        },\n        {\n          \"description\": \"The parameters for using an EventBridge event bus as a target.\"\n        }\n      ]\n    },\n    \"HttpParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetHttpParameters\"\n        },\n        {\n          \"description\": \"These are custom parameter to be used when the target is an API Gateway REST APIs or EventBridge ApiDestinations.\"\n        }\n      ]\n    },\n    \"InputTemplate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputTemplate\"\
  \n        },\n        {\n          \"description\": \"Valid JSON text passed to the target. In this case, nothing from the event itself is passed to the target. For more information, see <a href=\\\"http://www.rfc-editor.org/rfc/rfc7159.txt\\\">The JavaScript Object Notation (JSON) Data Interchange Format</a>.\"\n        }\n      ]\n    },\n    \"KinesisStreamParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetKinesisStreamParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a Kinesis stream as a source.\"\n        }\n      ]\n    },\n    \"LambdaFunctionParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetLambdaFunctionParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a Lambda function as a target.\"\n        }\n      ]\n    },\n    \"RedshiftDataParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\"\
  : \"#/components/schemas/PipeTargetRedshiftDataParameters\"\n        },\n        {\n          \"description\": \"These are custom parameters to be used when the target is a Amazon Redshift cluster to invoke the Amazon Redshift Data API ExecuteStatement.\"\n        }\n      ]\n    },\n    \"SageMakerPipelineParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetSageMakerPipelineParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a SageMaker pipeline as a target.\"\n        }\n      ]\n    },\n    \"SqsQueueParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetSqsQueueParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a Amazon SQS stream as a source.\"\n        }\n      ]\n    },\n    \"StepFunctionStateMachineParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeTargetStateMachineParameters\"\
  \n        },\n        {\n          \"description\": \"The parameters for using a Step Functions state machine as a target.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetParameters
---
