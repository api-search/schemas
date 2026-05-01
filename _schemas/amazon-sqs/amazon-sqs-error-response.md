---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: ''
  name: Error
  type: object
- description: The unique request identifier
  name: RequestId
  type: string
provider_name: Amazon SQS
provider_slug: amazon-sqs
schema_file: json-schema/amazon-sqs-error-response-schema.json
slug: amazon-sqs-error-response
source_filename: amazon-sqs-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Error\": {\n      \"type\": \"object\"\n    },\n    \"RequestId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique request identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sqs/refs/heads/main/json-schema/amazon-sqs-error-response-schema.json
tags:
- Cloud
- Distributed Systems
- Messaging
- Microservices
- Queue
title: ErrorResponse
---
