---
description: A data record in an Amazon Kinesis data stream.
layout: schema
name: Record
properties_list:
- description: The unique identifier of the record in the shard.
  name: SequenceNumber
  type: string
- description: The approximate time the record was inserted.
  name: ApproximateArrivalTimestamp
  type: string
- description: The data blob (base64-encoded).
  name: Data
  type: string
- description: Identifies which shard the data record belongs to.
  name: PartitionKey
  type: string
provider_name: Amazon Kinesis
provider_slug: amazon-kinesis
schema_file: json-schema/amazon-kinesis-record-schema.json
slug: amazon-kinesis-record
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/json-schema/amazon-kinesis-record-schema.json\",\n  \"title\": \"Record\",\n  \"description\": \"A data record in an Amazon Kinesis data stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SequenceNumber\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the record in the shard.\",\n      \"example\": \"seq-000000000000\"\n    },\n    \"ApproximateArrivalTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The approximate time the record was inserted.\",\n      \"format\": \"date-time\"\n    },\n    \"Data\": {\n      \"type\": \"string\",\n      \"description\": \"The data blob (base64-encoded).\"\n    },\n    \"PartitionKey\": {\n      \"type\": \"string\",\n      \"description\": \"Identifies which shard the data record belongs to.\",\n      \"example\"\
  : \"partition-1\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis/refs/heads/main/json-schema/amazon-kinesis-record-schema.json
tags:
- Analytics
- Big Data
- Data Processing
- Real-Time
- Streaming
title: Record
---
