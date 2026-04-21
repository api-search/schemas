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
