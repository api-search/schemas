---
description: The schedule's target. EventBridge Scheduler supports templated target that invoke common API operations, as well as universal targets that you can customize to invoke over 6,000 API operations across more than 270 services. You can only specify one templated or universal target for a schedule.
layout: schema
name: Target
properties_list:
- description: ''
  name: Arn
  type: object
- description: ''
  name: DeadLetterConfig
  type: object
- description: ''
  name: EcsParameters
  type: object
- description: ''
  name: EventBridgeParameters
  type: object
- description: ''
  name: Input
  type: object
- description: ''
  name: KinesisParameters
  type: object
- description: ''
  name: RetryPolicy
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: SageMakerPipelineParameters
  type: object
- description: ''
  name: SqsParameters
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-target-schema.json
slug: amazon-eventbridge-scheduler-target
source_filename: amazon-eventbridge-scheduler-target-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-target-schema.json\",\n  \"title\": \"Target\",\n  \"description\": \"The schedule's target. EventBridge Scheduler supports templated target that invoke common API operations, as well as universal targets that you can customize to invoke over 6,000 API operations across more than 270 services. You can only specify one templated or universal target for a schedule.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the target.\"\n        }\n      ]\n    },\n    \"DeadLetterConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeadLetterConfig\"\n\
  \        },\n        {\n          \"description\": \"An object that contains information about an Amazon SQS queue that EventBridge Scheduler uses as a dead-letter queue for your schedule. If specified, EventBridge Scheduler delivers failed events that could not be successfully delivered to a target to the queue.\"\n        }\n      ]\n    },\n    \"EcsParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EcsParameters\"\n        },\n        {\n          \"description\": \"The templated target type for the Amazon ECS <a href=\\\"https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_RunTask.html\\\"> <code>RunTask</code> </a> API operation.\"\n        }\n      ]\n    },\n    \"EventBridgeParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/EventBridgeParameters\"\n        },\n        {\n          \"description\": \"The templated target type for the EventBridge <a href=\\\"https://docs.aws.amazon.com/eventbridge/latest/APIReference/API_PutEvents.html\\\
  \"> <code>PutEvents</code> </a> API operation.\"\n        }\n      ]\n    },\n    \"Input\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetInput\"\n        },\n        {\n          \"description\": \"The text, or well-formed JSON, passed to the target. If you are configuring a templated Lambda, AWS Step Functions, or Amazon EventBridge target, the input must be a well-formed JSON. For all other target types, a JSON is not required. If you do not specify anything for this field, EventBridge Scheduler delivers a default notification to the target.\"\n        }\n      ]\n    },\n    \"KinesisParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisParameters\"\n        },\n        {\n          \"description\": \"The templated target type for the Amazon Kinesis <a href=\\\"kinesis/latest/APIReference/API_PutRecord.html\\\"> <code>PutRecord</code> </a> API operation.\"\n        }\n      ]\n    },\n    \"RetryPolicy\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RetryPolicy\"\n        },\n        {\n          \"description\": \"A <code>RetryPolicy</code> object that includes information about the retry policy settings, including the maximum age of an event, and the maximum number of times EventBridge Scheduler will try to deliver the event to a target.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleArn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that EventBridge Scheduler will use for this target when the schedule is invoked.\"\n        }\n      ]\n    },\n    \"SageMakerPipelineParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SageMakerPipelineParameters\"\n        },\n        {\n          \"description\": \"The templated target type for the Amazon SageMaker <a href=\\\"https://docs.aws.amazon.com/sagemaker/latest/APIReference/API_StartPipelineExecution.html\\\
  \"> <code>StartPipelineExecution</code> </a> API operation.\"\n        }\n      ]\n    },\n    \"SqsParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SqsParameters\"\n        },\n        {\n          \"description\": \"The templated target type for the Amazon SQS <a href=\\\"https://docs.aws.amazon.com/AWSSimpleQueueService/latest/APIReference/API_SendMessage.html\\\"> <code>SendMessage</code> </a> API operation. Contains the message group ID to use when the target is a FIFO queue. If you specify an Amazon SQS FIFO queue as a target, the queue must have content-based deduplication enabled. For more information, see <a href=\\\"https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/using-messagededuplicationid-property.html\\\">Using the Amazon SQS message deduplication ID</a> in the <i>Amazon SQS Developer Guide</i>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Arn\",\n    \"RoleArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-target-schema.json
tags:
- Amazon Web Services
- Cron
- Event-Driven
- Scheduling
- Serverless
title: Target
---
