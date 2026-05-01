---
description: StreamJournalToKinesisRequest schema from Amazon QLDB API
layout: schema
name: StreamJournalToKinesisRequest
properties_list:
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: Tags
  type: object
- description: ''
  name: InclusiveStartTime
  type: object
- description: ''
  name: ExclusiveEndTime
  type: object
- description: ''
  name: KinesisConfiguration
  type: object
- description: ''
  name: StreamName
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-stream-journal-to-kinesis-request-schema.json
slug: amazon-qldb-stream-journal-to-kinesis-request
source_filename: amazon-qldb-stream-journal-to-kinesis-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-stream-journal-to-kinesis-request-schema.json\",\n  \"title\": \"StreamJournalToKinesisRequest\",\n  \"description\": \"StreamJournalToKinesisRequest schema from Amazon QLDB API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"<p>The Amazon Resource Name (ARN) of the IAM role that grants QLDB permissions for a journal stream to write data records to a Kinesis Data Streams resource.</p> <p>To pass a role to QLDB when requesting a journal stream, you must have permissions to perform the <code>iam:PassRole</code> action on the IAM role resource. This is required for all journal stream requests.</p>\"\n        }\n      ]\n    },\n    \"Tags\": {\n\
  \      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Tags\"\n        },\n        {\n          \"description\": \"The key-value pairs to add as tags to the stream that you want to create. Tag keys are case sensitive. Tag values are case sensitive and can be null.\"\n        }\n      ]\n    },\n    \"InclusiveStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The inclusive start date and time from which to start streaming journal data. This parameter must be in <code>ISO 8601</code> date and time format and in Universal Coordinated Time (UTC). For example: <code>2019-06-13T21:36:34Z</code>.</p> <p>The <code>InclusiveStartTime</code> cannot be in the future and must be before <code>ExclusiveEndTime</code>.</p> <p>If you provide an <code>InclusiveStartTime</code> that is before the ledger's <code>CreationDateTime</code>, QLDB effectively defaults it to the ledger's\
  \ <code>CreationDateTime</code>.</p>\"\n        }\n      ]\n    },\n    \"ExclusiveEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"<p>The exclusive date and time that specifies when the stream ends. If you don't define this parameter, the stream runs indefinitely until you cancel it.</p> <p>The <code>ExclusiveEndTime</code> must be in <code>ISO 8601</code> date and time format and in Universal Coordinated Time (UTC). For example: <code>2019-06-13T21:36:34Z</code>.</p>\"\n        }\n      ]\n    },\n    \"KinesisConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisConfiguration\"\n        },\n        {\n          \"description\": \"The configuration settings of the Kinesis Data Streams destination for your stream request.\"\n        }\n      ]\n    },\n    \"StreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamName\"\
  \n        },\n        {\n          \"description\": \"<p>The name that you want to assign to the QLDB journal stream. User-defined names can help identify and indicate the purpose of a stream.</p> <p>Your stream name must be unique among other <i>active</i> streams for a given ledger. Stream names have the same naming constraints as ledger names, as defined in <a href=\\\"https://docs.aws.amazon.com/qldb/latest/developerguide/limits.html#limits.naming\\\">Quotas in Amazon QLDB</a> in the <i>Amazon QLDB Developer Guide</i>.</p>\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"RoleArn\",\n    \"InclusiveStartTime\",\n    \"KinesisConfiguration\",\n    \"StreamName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-stream-journal-to-kinesis-request-schema.json
tags:
- Blockchain
- Database
- Ledger
title: StreamJournalToKinesisRequest
---
