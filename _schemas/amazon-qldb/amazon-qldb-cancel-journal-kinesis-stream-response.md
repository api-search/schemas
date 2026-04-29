---
description: CancelJournalKinesisStreamResponse schema from Amazon QLDB API
layout: schema
name: CancelJournalKinesisStreamResponse
properties_list:
- description: ''
  name: StreamId
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-cancel-journal-kinesis-stream-response-schema.json
slug: amazon-qldb-cancel-journal-kinesis-stream-response
source_filename: amazon-qldb-cancel-journal-kinesis-stream-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-cancel-journal-kinesis-stream-response-schema.json\",\n  \"title\": \"CancelJournalKinesisStreamResponse\",\n  \"description\": \"CancelJournalKinesisStreamResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"StreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UniqueId\"\n        },\n        {\n          \"description\": \"The UUID (Base62-encoded text) of the canceled QLDB journal stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-cancel-journal-kinesis-stream-response-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: CancelJournalKinesisStreamResponse
---
