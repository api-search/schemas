---
description: The parameters for using a Rabbit MQ broker as a source.
layout: schema
name: PipeSourceRabbitMQBrokerParameters
properties_list:
- description: ''
  name: BatchSize
  type: object
- description: ''
  name: Credentials
  type: object
- description: ''
  name: MaximumBatchingWindowInSeconds
  type: object
- description: ''
  name: QueueName
  type: object
- description: ''
  name: VirtualHost
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-source-rabbit-mq-broker-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-source-rabbit-mq-broker-parameters
source_filename: amazon-eventbridge-pipes-pipe-source-rabbit-mq-broker-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-source-rabbit-mq-broker-parameters-schema.json\",\n  \"title\": \"PipeSourceRabbitMQBrokerParameters\",\n  \"description\": \"The parameters for using a Rabbit MQ broker as a source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BatchSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitMax10000\"\n        },\n        {\n          \"description\": \"The maximum number of records to include in each batch.\"\n        }\n      ]\n    },\n    \"Credentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MQBrokerAccessCredentials\"\n        },\n        {\n          \"description\": \"The credentials needed to access the resource.\"\n        }\n      ]\n    },\n    \"MaximumBatchingWindowInSeconds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumBatchingWindowInSeconds\"\n        },\n        {\n          \"description\": \"The maximum length of a time to wait for events.\"\n        }\n      ]\n    },\n    \"QueueName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MQBrokerQueueName\"\n        },\n        {\n          \"description\": \"The name of the destination queue to consume.\"\n        }\n      ]\n    },\n    \"VirtualHost\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/URI\"\n        },\n        {\n          \"description\": \"The name of the virtual host associated with the source broker.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Credentials\",\n    \"QueueName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-source-rabbit-mq-broker-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeSourceRabbitMQBrokerParameters
---
