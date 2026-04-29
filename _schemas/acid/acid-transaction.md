---
description: Represents an ACID database transaction with its properties, status, and isolation level.
layout: schema
name: AcidTransaction
properties_list:
- description: Unique identifier for the transaction
  name: transactionId
  type: string
- description: Current status of the transaction
  name: status
  type: string
- description: SQL transaction isolation level
  name: isolationLevel
  type: string
- description: Timestamp when the transaction began
  name: startTime
  type: string
- description: Timestamp when the transaction was committed or rolled back
  name: endTime
  type: string
- description: Transaction duration in milliseconds
  name: durationMs
  type: integer
- description: List of database operations within this transaction
  name: operations
  type: array
- description: Reason for rollback if the transaction was not committed
  name: rollbackReason
  type: string
- description: Named savepoints defined within this transaction
  name: savepoints
  type: array
provider_name: ACID
provider_slug: acid
schema_file: json-schema/acid-transaction-schema.json
slug: acid-transaction
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acid/refs/heads/main/json-schema/acid-transaction-schema.json\",\n  \"title\": \"AcidTransaction\",\n  \"description\": \"Represents an ACID database transaction with its properties, status, and isolation level.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"transactionId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"Unique identifier for the transaction\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the transaction\",\n      \"enum\": [\"Active\", \"Committed\", \"Rolled Back\", \"Aborted\", \"Pending\"],\n      \"example\": \"Committed\"\n    },\n    \"isolationLevel\": {\n      \"type\": \"string\",\n      \"description\": \"SQL transaction isolation level\",\n      \"enum\":\
  \ [\"Read Uncommitted\", \"Read Committed\", \"Repeatable Read\", \"Serializable\"],\n      \"example\": \"Serializable\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the transaction began\",\n      \"example\": \"2026-04-19T10:00:00.000Z\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the transaction was committed or rolled back\",\n      \"example\": \"2026-04-19T10:00:00.150Z\"\n    },\n    \"durationMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Transaction duration in milliseconds\",\n      \"example\": 150\n    },\n    \"operations\": {\n      \"type\": \"array\",\n      \"description\": \"List of database operations within this transaction\",\n      \"items\": {\n        \"$ref\": \"#/$defs/DatabaseOperation\"\n      }\n    },\n    \"rollbackReason\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Reason for rollback if the transaction was not committed\",\n      \"example\": \"Serialization failure: concurrent transaction updated the same row\"\n    },\n    \"savepoints\": {\n      \"type\": \"array\",\n      \"description\": \"Named savepoints defined within this transaction\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\"sp1\", \"before_payment\"]\n    }\n  },\n  \"required\": [\"transactionId\", \"status\", \"isolationLevel\", \"startTime\"],\n  \"$defs\": {\n    \"DatabaseOperation\": {\n      \"type\": \"object\",\n      \"description\": \"A single SQL operation within a transaction\",\n      \"properties\": {\n        \"operationId\": {\n          \"type\": \"integer\",\n          \"description\": \"Sequential identifier within the transaction\",\n          \"example\": 1\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"SQL operation type\",\n          \"enum\": [\"SELECT\"\
  , \"INSERT\", \"UPDATE\", \"DELETE\", \"SAVEPOINT\", \"ROLLBACK TO SAVEPOINT\"],\n          \"example\": \"UPDATE\"\n        },\n        \"table\": {\n          \"type\": \"string\",\n          \"description\": \"Database table affected by the operation\",\n          \"example\": \"accounts\"\n        },\n        \"rowsAffected\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of rows affected by the operation\",\n          \"example\": 1\n        },\n        \"executionTimeMs\": {\n          \"type\": \"number\",\n          \"description\": \"Execution time of the operation in milliseconds\",\n          \"example\": 2.5\n        }\n      },\n      \"required\": [\"operationId\", \"type\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acid/refs/heads/main/json-schema/acid-transaction-schema.json
tags:
- ACID
- Database
- Transactions
- Atomicity
- Consistency
- Isolation
- Durability
- Distributed Systems
title: AcidTransaction
---
