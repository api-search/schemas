---
description: An Async Agent defines a consumer that subscribes to a queue or event stream (such as RabbitMQ, Kafka, or AWS SNS/SQS) and processes messages independently of HTTP request/response cycles.
layout: schema
name: KrakenD Async Agent
properties_list:
- description: A unique name for the async agent.
  name: name
  type: string
- description: The encoding of the consumed messages.
  name: encoding
  type: string
- description: Backend definitions to process the consumed messages.
  name: backend
  type: array
- description: Consumer configuration including topic, subscription, and connection details.
  name: consumer
  type: object
- description: Connection settings for the message broker.
  name: connection
  type: object
- description: Additional component configurations keyed by namespace.
  name: extra_config
  type: object
provider_name: KrakenD
provider_slug: krakend
schema_file: json-schema/async-agent.json
slug: async-agent
source_filename: async-agent.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/krakend/blob/main/json-schema/async-agent.json\",\n  \"title\": \"KrakenD Async Agent\",\n  \"description\": \"An Async Agent defines a consumer that subscribes to a queue or event stream (such as RabbitMQ, Kafka, or AWS SNS/SQS) and processes messages independently of HTTP request/response cycles.\",\n  \"type\": \"object\",\n  \"required\": [\"name\", \"backend\", \"consumer\"],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A unique name for the async agent.\"\n    },\n    \"encoding\": {\n      \"type\": \"string\",\n      \"description\": \"The encoding of the consumed messages.\"\n    },\n    \"backend\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"backend.json\"\n      },\n      \"description\": \"Backend definitions to process the consumed messages.\"\n    },\n    \"consumer\": {\n\
  \      \"type\": \"object\",\n      \"description\": \"Consumer configuration including topic, subscription, and connection details.\",\n      \"properties\": {\n        \"topic\": {\n          \"type\": \"string\",\n          \"description\": \"The topic or queue name to consume from.\"\n        },\n        \"workers\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of concurrent consumer workers.\"\n        },\n        \"timeout\": {\n          \"type\": \"string\",\n          \"description\": \"Timeout for consuming a message.\"\n        },\n        \"max_rate\": {\n          \"type\": \"number\",\n          \"description\": \"Maximum rate of messages consumed per second.\"\n        }\n      }\n    },\n    \"connection\": {\n      \"type\": \"object\",\n      \"description\": \"Connection settings for the message broker.\",\n      \"properties\": {\n        \"max_retries\": {\n          \"type\": \"integer\",\n          \"description\": \"Maximum number of\
  \ connection retry attempts.\"\n        },\n        \"backoff_strategy\": {\n          \"type\": \"string\",\n          \"description\": \"Backoff strategy for reconnection attempts.\"\n        },\n        \"health_interval\": {\n          \"type\": \"string\",\n          \"description\": \"Interval between health checks on the connection.\"\n        }\n      }\n    },\n    \"extra_config\": {\n      \"type\": \"object\",\n      \"description\": \"Additional component configurations keyed by namespace.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/krakend/refs/heads/main/json-schema/async-agent.json
tags:
- Aggregation
- API Gateway
- Go
- Open Source
title: KrakenD Async Agent
---
