---
description: The parameters for using a self-managed Apache Kafka stream as a source.
layout: schema
name: UpdatePipeSourceSelfManagedKafkaParameters
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
  name: ServerRootCaCertificate
  type: object
- description: ''
  name: Vpc
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-update-pipe-source-self-managed-kafka-parameters-schema.json
slug: amazon-eventbridge-pipes-update-pipe-source-self-managed-kafka-parameters
source_filename: amazon-eventbridge-pipes-update-pipe-source-self-managed-kafka-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-update-pipe-source-self-managed-kafka-parameters-schema.json\",\n  \"title\": \"UpdatePipeSourceSelfManagedKafkaParameters\",\n  \"description\": \"The parameters for using a self-managed Apache Kafka stream as a source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BatchSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitMax10000\"\n        },\n        {\n          \"description\": \"The maximum number of records to include in each batch.\"\n        }\n      ]\n    },\n    \"Credentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelfManagedKafkaAccessConfigurationCredentials\"\n        },\n        {\n          \"description\": \"The credentials needed to access the resource.\"\n     \
  \   }\n      ]\n    },\n    \"MaximumBatchingWindowInSeconds\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumBatchingWindowInSeconds\"\n        },\n        {\n          \"description\": \"The maximum length of a time to wait for events.\"\n        }\n      ]\n    },\n    \"ServerRootCaCertificate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SecretManagerArn\"\n        },\n        {\n          \"description\": \"The ARN of the Secrets Manager secret used for certification.\"\n        }\n      ]\n    },\n    \"Vpc\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SelfManagedKafkaAccessConfigurationVpc\"\n        },\n        {\n          \"description\": \"This structure specifies the VPC subnets and security groups for the stream, and whether a public IP address is to be used.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-update-pipe-source-self-managed-kafka-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: UpdatePipeSourceSelfManagedKafkaParameters
---
