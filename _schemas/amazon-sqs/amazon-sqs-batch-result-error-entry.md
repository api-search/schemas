---
description: A batch result error entry
layout: schema
name: BatchResultErrorEntry
properties_list:
- description: The Id of the entry that caused the error
  name: Id
  type: string
- description: An error code representing the type of error
  name: Code
  type: string
- description: A message explaining the error
  name: Message
  type: string
- description: Specifies whether the error happened due to the caller of the batch API action
  name: SenderFault
  type: boolean
provider_name: Amazon SQS
provider_slug: amazon-sqs
schema_file: json-schema/amazon-sqs-batch-result-error-entry-schema.json
slug: amazon-sqs-batch-result-error-entry
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchResultErrorEntry\",\n  \"type\": \"object\",\n  \"description\": \"A batch result error entry\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The Id of the entry that caused the error\"\n    },\n    \"Code\": {\n      \"type\": \"string\",\n      \"description\": \"An error code representing the type of error\"\n    },\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"A message explaining the error\"\n    },\n    \"SenderFault\": {\n      \"type\": \"boolean\",\n      \"description\": \"Specifies whether the error happened due to the caller of the batch API action\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-sqs/refs/heads/main/json-schema/amazon-sqs-batch-result-error-entry-schema.json
tags:
- AWS
- Cloud
- Distributed Systems
- Messaging
- Microservices
- Queue
title: BatchResultErrorEntry
---
