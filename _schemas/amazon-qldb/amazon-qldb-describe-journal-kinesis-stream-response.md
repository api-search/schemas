---
description: DescribeJournalKinesisStreamResponse schema from Amazon QLDB API
layout: schema
name: DescribeJournalKinesisStreamResponse
properties_list:
- description: ''
  name: Stream
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-describe-journal-kinesis-stream-response-schema.json
slug: amazon-qldb-describe-journal-kinesis-stream-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-describe-journal-kinesis-stream-response-schema.json\",\n  \"title\": \"DescribeJournalKinesisStreamResponse\",\n  \"description\": \"DescribeJournalKinesisStreamResponse schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Stream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/JournalKinesisStreamDescription\"\n        },\n        {\n          \"description\": \"Information about the QLDB journal stream returned by a <code>DescribeJournalS3Export</code> request.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-describe-journal-kinesis-stream-response-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: DescribeJournalKinesisStreamResponse
---
