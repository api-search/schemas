---
description: The parameters for using a self-managed Apache Kafka stream as a source.
layout: schema
name: PipeSourceSelfManagedKafkaParameters
properties_list:
- description: ''
  name: AdditionalBootstrapServers
  type: object
- description: ''
  name: BatchSize
  type: object
- description: ''
  name: ConsumerGroupID
  type: object
- description: ''
  name: Credentials
  type: object
- description: ''
  name: MaximumBatchingWindowInSeconds
  type: object
- description: ''
  name: ServerRootCaCertificate
  type: object
- description: ''
  name: StartingPosition
  type: object
- description: ''
  name: TopicName
  type: object
- description: ''
  name: Vpc
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-source-self-managed-kafka-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-source-self-managed-kafka-parameters
source_filename: amazon-eventbridge-pipes-pipe-source-self-managed-kafka-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-source-self-managed-kafka-parameters-schema.json\",\n  \"title\": \"PipeSourceSelfManagedKafkaParameters\",\n  \"description\": \"The parameters for using a self-managed Apache Kafka stream as a source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AdditionalBootstrapServers\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KafkaBootstrapServers\"\n        },\n        {\n          \"description\": \"An array of server URLs.\"\n        }\n      ]\n    },\n    \"BatchSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitMax10000\"\n        },\n        {\n          \"description\": \"The maximum number of records to include in each batch.\"\n        }\n      ]\n    },\n    \"ConsumerGroupID\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/URI\"\n        },\n        {\n          \"description\": \"The name of the destination queue to consume.\"\n        }\n      ]\n    },\n    \"Credentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelfManagedKafkaAccessConfigurationCredentials\"\n        },\n        {\n          \"description\": \"The credentials needed to access the resource.\"\n        }\n      ]\n    },\n    \"MaximumBatchingWindowInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumBatchingWindowInSeconds\"\n        },\n        {\n          \"description\": \"The maximum length of a time to wait for events.\"\n        }\n      ]\n    },\n    \"ServerRootCaCertificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretManagerArn\"\n        },\n        {\n          \"description\": \"The ARN of the Secrets Manager secret used\
  \ for certification.\"\n        }\n      ]\n    },\n    \"StartingPosition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelfManagedKafkaStartPosition\"\n        },\n        {\n          \"description\": \"(Streams only) The position in a stream from which to start reading.\"\n        }\n      ]\n    },\n    \"TopicName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KafkaTopicName\"\n        },\n        {\n          \"description\": \"The name of the topic that the pipe will read from.\"\n        }\n      ]\n    },\n    \"Vpc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelfManagedKafkaAccessConfigurationVpc\"\n        },\n        {\n          \"description\": \"This structure specifies the VPC subnets and security groups for the stream, and whether a public IP address is to be used.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"TopicName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-source-self-managed-kafka-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeSourceSelfManagedKafkaParameters
---
