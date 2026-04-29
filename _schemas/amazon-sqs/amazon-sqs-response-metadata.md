---
description: ''
layout: schema
name: ResponseMetadata
properties_list:
- description: A unique identifier for the request
  name: RequestId
  type: string
provider_name: Amazon SQS
provider_slug: amazon-sqs
schema_file: json-schema/amazon-sqs-response-metadata-schema.json
slug: amazon-sqs-response-metadata
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResponseMetadata\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RequestId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the request\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sqs/refs/heads/main/json-schema/amazon-sqs-response-metadata-schema.json
tags:
- AWS
- Cloud
- Distributed Systems
- Messaging
- Microservices
- Queue
title: ResponseMetadata
---
