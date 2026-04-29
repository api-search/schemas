---
description: Information about an Amazon QLDB journal stream, including the Amazon Resource Name (ARN), stream name, creation time, current status, and the parameters of the original stream creation request.
layout: schema
name: JournalKinesisStreamDescription
properties_list:
- description: ''
  name: LedgerName
  type: object
- description: ''
  name: CreationTime
  type: object
- description: ''
  name: InclusiveStartTime
  type: object
- description: ''
  name: ExclusiveEndTime
  type: object
- description: ''
  name: RoleArn
  type: object
- description: ''
  name: StreamId
  type: object
- description: ''
  name: Arn
  type: object
- description: ''
  name: Status
  type: object
- description: ''
  name: KinesisConfiguration
  type: object
- description: ''
  name: ErrorCause
  type: object
- description: ''
  name: StreamName
  type: object
provider_name: Amazon QLDB
provider_slug: amazon-qldb
schema_file: json-schema/amazon-qldb-journal-kinesis-stream-description-schema.json
slug: amazon-qldb-journal-kinesis-stream-description
source_filename: amazon-qldb-journal-kinesis-stream-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-journal-kinesis-stream-description-schema.json\",\n  \"title\": \"JournalKinesisStreamDescription\",\n  \"description\": \"Information about an Amazon QLDB journal stream, including the Amazon Resource Name (ARN), stream name, creation time, current status, and the parameters of the original stream creation request.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LedgerName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LedgerName\"\n        },\n        {\n          \"description\": \"The name of the ledger.\"\n        }\n      ]\n    },\n    \"CreationTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The date and time, in epoch time format, when the QLDB\
  \ journal stream was created. (Epoch time format is the number of seconds elapsed since 12:00:00 AM January 1, 1970 UTC.)\"\n        }\n      ]\n    },\n    \"InclusiveStartTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The inclusive start date and time from which to start streaming journal data.\"\n        }\n      ]\n    },\n    \"ExclusiveEndTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The exclusive date and time that specifies when the stream ends. If this parameter is undefined, the stream runs indefinitely until you cancel it.\"\n        }\n      ]\n    },\n    \"RoleArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the IAM role that grants QLDB permissions\
  \ for a journal stream to write data records to a Kinesis Data Streams resource.\"\n        }\n      ]\n    },\n    \"StreamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/UniqueId\"\n        },\n        {\n          \"description\": \"The UUID (represented in Base62-encoded text) of the QLDB journal stream.\"\n        }\n      ]\n    },\n    \"Arn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Arn\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the QLDB journal stream.\"\n        }\n      ]\n    },\n    \"Status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamStatus\"\n        },\n        {\n          \"description\": \"The current state of the QLDB journal stream.\"\n        }\n      ]\n    },\n    \"KinesisConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisConfiguration\"\n        },\n   \
  \     {\n          \"description\": \"The configuration settings of the Amazon Kinesis Data Streams destination for a QLDB journal stream.\"\n        }\n      ]\n    },\n    \"ErrorCause\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ErrorCause\"\n        },\n        {\n          \"description\": \"The error message that describes the reason that a stream has a status of <code>IMPAIRED</code> or <code>FAILED</code>. This is not applicable to streams that have other status values.\"\n        }\n      ]\n    },\n    \"StreamName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamName\"\n        },\n        {\n          \"description\": \"The user-defined name of the QLDB journal stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LedgerName\",\n    \"RoleArn\",\n    \"StreamId\",\n    \"Status\",\n    \"KinesisConfiguration\",\n    \"StreamName\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-qldb/refs/heads/main/json-schema/amazon-qldb-journal-kinesis-stream-description-schema.json
tags:
- AWS
- Blockchain
- Database
- Ledger
title: JournalKinesisStreamDescription
---
