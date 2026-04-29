---
description: The parameters for using a Kinesis stream as a source.
layout: schema
name: UpdatePipeSourceKinesisStreamParameters
properties_list:
- description: ''
  name: BatchSize
  type: object
- description: ''
  name: DeadLetterConfig
  type: object
- description: ''
  name: MaximumBatchingWindowInSeconds
  type: object
- description: ''
  name: MaximumRecordAgeInSeconds
  type: object
- description: ''
  name: MaximumRetryAttempts
  type: object
- description: ''
  name: OnPartialBatchItemFailure
  type: object
- description: ''
  name: ParallelizationFactor
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-update-pipe-source-kinesis-stream-parameters-schema.json
slug: amazon-eventbridge-pipes-update-pipe-source-kinesis-stream-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-update-pipe-source-kinesis-stream-parameters-schema.json\",\n  \"title\": \"UpdatePipeSourceKinesisStreamParameters\",\n  \"description\": \"The parameters for using a Kinesis stream as a source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BatchSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitMax10000\"\n        },\n        {\n          \"description\": \"The maximum number of records to include in each batch.\"\n        }\n      ]\n    },\n    \"DeadLetterConfig\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DeadLetterConfig\"\n        },\n        {\n          \"description\": \"Define the target queue to send dead-letter queue events to.\"\n        }\n      ]\n    },\n    \"MaximumBatchingWindowInSeconds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumBatchingWindowInSeconds\"\n        },\n        {\n          \"description\": \"The maximum length of a time to wait for events.\"\n        }\n      ]\n    },\n    \"MaximumRecordAgeInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumRecordAgeInSeconds\"\n        },\n        {\n          \"description\": \"(Streams only) Discard records older than the specified age. The default value is -1, which sets the maximum age to infinite. When the value is set to infinite, EventBridge never discards old records. \"\n        }\n      ]\n    },\n    \"MaximumRetryAttempts\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumRetryAttemptsESM\"\n        },\n        {\n          \"description\": \"(Streams only) Discard records after the specified number of retries. The default value is -1, which sets the maximum number of retries to infinite.\
  \ When MaximumRetryAttempts is infinite, EventBridge retries failed records until the record expires in the event source.\"\n        }\n      ]\n    },\n    \"OnPartialBatchItemFailure\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/OnPartialBatchItemFailureStreams\"\n        },\n        {\n          \"description\": \"(Streams only) Define how to handle item process failures. <code>AUTOMATIC_BISECT</code> halves each batch and retry each half until all the records are processed or there is one failed message left in the batch.\"\n        }\n      ]\n    },\n    \"ParallelizationFactor\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitMax10\"\n        },\n        {\n          \"description\": \"(Streams only) The number of batches to process concurrently from each shard. The default value is 1.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-update-pipe-source-kinesis-stream-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: UpdatePipeSourceKinesisStreamParameters
---
