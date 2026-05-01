---
description: A Lambda event source mapping that connects an event source to a Lambda function.
layout: schema
name: EventSourceMapping
properties_list:
- description: The identifier of the event source mapping.
  name: UUID
  type: string
- description: The ARN of the event source.
  name: EventSourceArn
  type: string
- description: The ARN of the Lambda function.
  name: FunctionArn
  type: string
- description: The state of the event source mapping.
  name: State
  type: string
- description: The maximum number of records in each batch.
  name: BatchSize
  type: integer
provider_name: Amazon Lambda
provider_slug: amazon-lambda
schema_file: json-schema/amazon-lambda-event-source-mapping-schema.json
slug: amazon-lambda-event-source-mapping
source_filename: amazon-lambda-event-source-mapping-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-lambda/refs/heads/main/json-schema/amazon-lambda-event-source-mapping-schema.json\",\n  \"title\": \"EventSourceMapping\",\n  \"description\": \"A Lambda event source mapping that connects an event source to a Lambda function.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"UUID\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the event source mapping.\",\n      \"example\": \"abc12345-6789-def0-1234-abcdef012345\"\n    },\n    \"EventSourceArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the event source.\"\n    },\n    \"FunctionArn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the Lambda function.\"\n    },\n    \"State\": {\n      \"type\": \"string\",\n      \"description\": \"The state of the event source mapping.\",\n      \"example\": \"Enabled\"\
  ,\n      \"enum\": [\n        \"Creating\",\n        \"Enabling\",\n        \"Enabled\",\n        \"Disabling\",\n        \"Disabled\",\n        \"Updating\",\n        \"Deleting\"\n      ]\n    },\n    \"BatchSize\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of records in each batch.\",\n      \"example\": 10\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-lambda/refs/heads/main/json-schema/amazon-lambda-event-source-mapping-schema.json
tags:
- Compute
- Event-Driven
- FaaS
- Functions
- Serverless
title: EventSourceMapping
---
