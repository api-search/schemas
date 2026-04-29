---
description: The parameters required to set up a source for your pipe.
layout: schema
name: PipeSourceParameters
properties_list:
- description: ''
  name: ActiveMQBrokerParameters
  type: object
- description: ''
  name: DynamoDBStreamParameters
  type: object
- description: ''
  name: FilterCriteria
  type: object
- description: ''
  name: KinesisStreamParameters
  type: object
- description: ''
  name: ManagedStreamingKafkaParameters
  type: object
- description: ''
  name: RabbitMQBrokerParameters
  type: object
- description: ''
  name: SelfManagedKafkaParameters
  type: object
- description: ''
  name: SqsQueueParameters
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-source-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-source-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-source-parameters-schema.json\",\n  \"title\": \"PipeSourceParameters\",\n  \"description\": \"The parameters required to set up a source for your pipe.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ActiveMQBrokerParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeSourceActiveMQBrokerParameters\"\n        },\n        {\n          \"description\": \"The parameters for using an Active MQ broker as a source.\"\n        }\n      ]\n    },\n    \"DynamoDBStreamParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeSourceDynamoDBStreamParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a DynamoDB stream as a source.\"\n        }\n      ]\n\
  \    },\n    \"FilterCriteria\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FilterCriteria\"\n        },\n        {\n          \"description\": \"The collection of event patterns used to filter events. For more information, see <a href=\\\"https://docs.aws.amazon.com/eventbridge/latest/userguide/eventbridge-and-event-patterns.html\\\">Events and Event Patterns</a> in the <i>Amazon EventBridge User Guide</i>.\"\n        }\n      ]\n    },\n    \"KinesisStreamParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeSourceKinesisStreamParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a Kinesis stream as a source.\"\n        }\n      ]\n    },\n    \"ManagedStreamingKafkaParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeSourceManagedStreamingKafkaParameters\"\n        },\n        {\n          \"description\": \"The parameters for using\
  \ an MSK stream as a source.\"\n        }\n      ]\n    },\n    \"RabbitMQBrokerParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeSourceRabbitMQBrokerParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a Rabbit MQ broker as a source.\"\n        }\n      ]\n    },\n    \"SelfManagedKafkaParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeSourceSelfManagedKafkaParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a self-managed Apache Kafka stream as a source.\"\n        }\n      ]\n    },\n    \"SqsQueueParameters\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PipeSourceSqsQueueParameters\"\n        },\n        {\n          \"description\": \"The parameters for using a Amazon SQS stream as a source.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-source-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeSourceParameters
---
