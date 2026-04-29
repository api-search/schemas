---
description: A step in a distributed Saga pattern transaction, representing a local transaction with a compensating action for rollback.
layout: schema
name: AcidSagaStep
properties_list:
- description: Unique identifier for this saga step
  name: stepId
  type: string
- description: Identifier of the parent saga workflow
  name: sagaId
  type: string
- description: Human-readable name for this saga step
  name: stepName
  type: string
- description: Execution order within the saga (1-based)
  name: sequence
  type: integer
- description: Current status of this saga step
  name: status
  type: string
- description: URL of the service responsible for this step
  name: serviceEndpoint
  type: string
- description: URL to call to undo this step if a later step fails
  name: compensationEndpoint
  type: string
- description: When this step began executing
  name: startTime
  type: string
- description: When this step completed or was compensated
  name: endTime
  type: string
- description: Number of retry attempts for this step
  name: retryCount
  type: integer
- description: Error message if the step failed
  name: errorMessage
  type: string
provider_name: ACID
provider_slug: acid
schema_file: json-schema/acid-saga-step-schema.json
slug: acid-saga-step
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acid/refs/heads/main/json-schema/acid-saga-step-schema.json\",\n  \"title\": \"AcidSagaStep\",\n  \"description\": \"A step in a distributed Saga pattern transaction, representing a local transaction with a compensating action for rollback.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stepId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for this saga step\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"sagaId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Identifier of the parent saga workflow\",\n      \"example\": \"b2c3d4e5-f6a7-8901-bcde-fa2345678901\"\n    },\n    \"stepName\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name for this saga step\",\n      \"example\": \"\
  Debit Customer Account\"\n    },\n    \"sequence\": {\n      \"type\": \"integer\",\n      \"description\": \"Execution order within the saga (1-based)\",\n      \"example\": 1\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of this saga step\",\n      \"enum\": [\"Pending\", \"Executing\", \"Completed\", \"Compensating\", \"Compensated\", \"Failed\"],\n      \"example\": \"Completed\"\n    },\n    \"serviceEndpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the service responsible for this step\",\n      \"example\": \"https://payments.example.com/api/debit\"\n    },\n    \"compensationEndpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to call to undo this step if a later step fails\",\n      \"example\": \"https://payments.example.com/api/refund\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"When this step began executing\",\n      \"example\": \"2026-04-19T10:00:00.000Z\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When this step completed or was compensated\",\n      \"example\": \"2026-04-19T10:00:00.200Z\"\n    },\n    \"retryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of retry attempts for this step\",\n      \"example\": 0\n    },\n    \"errorMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Error message if the step failed\",\n      \"example\": \"Insufficient funds in account\"\n    }\n  },\n  \"required\": [\"stepId\", \"sagaId\", \"stepName\", \"sequence\", \"status\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acid/refs/heads/main/json-schema/acid-saga-step-schema.json
tags:
- ACID
- Database
- Transactions
- Atomicity
- Consistency
- Isolation
- Durability
- Distributed Systems
title: AcidSagaStep
---
