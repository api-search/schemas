---
description: The parameters for using an Active MQ broker as a source.
layout: schema
name: UpdatePipeSourceActiveMQBrokerParameters
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
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-update-pipe-source-active-mq-broker-parameters-schema.json
slug: amazon-eventbridge-pipes-update-pipe-source-active-mq-broker-parameters
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-update-pipe-source-active-mq-broker-parameters-schema.json\",\n  \"title\": \"UpdatePipeSourceActiveMQBrokerParameters\",\n  \"description\": \"The parameters for using an Active MQ broker as a source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"BatchSize\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LimitMax10000\"\n        },\n        {\n          \"description\": \"The maximum number of records to include in each batch.\"\n        }\n      ]\n    },\n    \"Credentials\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MQBrokerAccessCredentials\"\n        },\n        {\n          \"description\": \"The credentials needed to access the resource.\"\n        }\n      ]\n    },\n    \"MaximumBatchingWindowInSeconds\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MaximumBatchingWindowInSeconds\"\n        },\n        {\n          \"description\": \"The maximum length of a time to wait for events.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Credentials\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-update-pipe-source-active-mq-broker-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Event-Driven
- Integration
- Messaging
- Serverless
title: UpdatePipeSourceActiveMQBrokerParameters
---
