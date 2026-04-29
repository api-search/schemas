---
description: Response returned by the Apache Doris Stream Load HTTP API after a data loading operation.
layout: schema
name: StreamLoadResponse
properties_list:
- description: Transaction ID assigned to this load job.
  name: TxnId
  type: integer
- description: Label for idempotent load tracking.
  name: Label
  type: string
- description: Overall status of the load operation.
  name: Status
  type: string
- description: Status of existing job with same label if label already exists.
  name: ExistingJobStatus
  type: string
- description: Status message or error description.
  name: Message
  type: string
- description: Total number of rows processed.
  name: NumberTotalRows
  type: integer
- description: Number of rows successfully loaded.
  name: NumberLoadedRows
  type: integer
- description: Number of rows filtered due to quality issues.
  name: NumberFilteredRows
  type: integer
- description: Number of rows filtered by WHERE clause.
  name: NumberUnselectedRows
  type: integer
- description: Total data size loaded in bytes.
  name: LoadBytes
  type: integer
- description: Time spent loading data in milliseconds.
  name: LoadTimeMs
  type: integer
- description: Time to begin transaction in milliseconds.
  name: BeginTxnTimeMs
  type: integer
- description: Time to plan the load in milliseconds.
  name: StreamLoadPutTimeMs
  type: integer
- description: Time to read data in milliseconds.
  name: ReadDataTimeMs
  type: integer
- description: Time to write data in milliseconds.
  name: WriteDataTimeMs
  type: integer
- description: Time to commit and publish in milliseconds.
  name: CommitAndPublishTimeMs
  type: integer
- description: URL to retrieve error details when rows are filtered.
  name: ErrorURL
  type: string
provider_name: Apache Doris
provider_slug: apache-doris
schema_file: json-schema/apache-doris-stream-load-response-schema.json
slug: apache-doris-stream-load-response
source_filename: apache-doris-stream-load-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-doris/refs/heads/main/json-schema/apache-doris-stream-load-response-schema.json\",\n  \"title\": \"StreamLoadResponse\",\n  \"description\": \"Response returned by the Apache Doris Stream Load HTTP API after a data loading operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"TxnId\": {\n      \"type\": \"integer\",\n      \"description\": \"Transaction ID assigned to this load job.\",\n      \"example\": 1001\n    },\n    \"Label\": {\n      \"type\": \"string\",\n      \"description\": \"Label for idempotent load tracking.\",\n      \"example\": \"load-20250315-001\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"Overall status of the load operation.\",\n      \"enum\": [\n        \"Success\",\n        \"Publish Timeout\",\n        \"Label Already Exists\",\n        \"Fail\"\n      ],\n  \
  \    \"example\": \"Success\"\n    },\n    \"ExistingJobStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Status of existing job with same label if label already exists.\",\n      \"example\": \"FINISHED\"\n    },\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"Status message or error description.\",\n      \"example\": \"OK\"\n    },\n    \"NumberTotalRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of rows processed.\",\n      \"example\": 10000\n    },\n    \"NumberLoadedRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows successfully loaded.\",\n      \"example\": 9998\n    },\n    \"NumberFilteredRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows filtered due to quality issues.\",\n      \"example\": 2\n    },\n    \"NumberUnselectedRows\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of rows filtered by WHERE clause.\",\n      \"\
  example\": 0\n    },\n    \"LoadBytes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total data size loaded in bytes.\",\n      \"example\": 1024000\n    },\n    \"LoadTimeMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Time spent loading data in milliseconds.\",\n      \"example\": 350\n    },\n    \"BeginTxnTimeMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to begin transaction in milliseconds.\",\n      \"example\": 5\n    },\n    \"StreamLoadPutTimeMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to plan the load in milliseconds.\",\n      \"example\": 20\n    },\n    \"ReadDataTimeMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to read data in milliseconds.\",\n      \"example\": 120\n    },\n    \"WriteDataTimeMs\": {\n      \"type\": \"integer\",\n      \"description\": \"Time to write data in milliseconds.\",\n      \"example\": 200\n    },\n    \"CommitAndPublishTimeMs\": {\n      \"type\"\
  : \"integer\",\n      \"description\": \"Time to commit and publish in milliseconds.\",\n      \"example\": 5\n    },\n    \"ErrorURL\": {\n      \"type\": \"string\",\n      \"description\": \"URL to retrieve error details when rows are filtered.\",\n      \"example\": \"http://doris-fe:8030/api/_load_error_log?file=error_log_abc\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-doris/refs/heads/main/json-schema/apache-doris-stream-load-response-schema.json
tags:
- Analytics
- Apache
- Database
- Lakehouse
- MPP
- OLAP
- Open Source
- Real-Time
- SQL
title: StreamLoadResponse
---
