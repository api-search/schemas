---
description: The parameters for using a Kinesis stream as a source.
layout: schema
name: PipeTargetKinesisStreamParameters
properties_list:
- description: ''
  name: PartitionKey
  type: object
provider_name: Amazon EventBridge Pipes
provider_slug: amazon-eventbridge-pipes
schema_file: json-schema/amazon-eventbridge-pipes-pipe-target-kinesis-stream-parameters-schema.json
slug: amazon-eventbridge-pipes-pipe-target-kinesis-stream-parameters
source_filename: amazon-eventbridge-pipes-pipe-target-kinesis-stream-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-kinesis-stream-parameters-schema.json\",\n  \"title\": \"PipeTargetKinesisStreamParameters\",\n  \"description\": \"The parameters for using a Kinesis stream as a source.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PartitionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisPartitionKey\"\n        },\n        {\n          \"description\": \"Determines which shard in the stream the data record is assigned to. Partition keys are Unicode strings with a maximum length limit of 256 characters for each key. Amazon Kinesis Data Streams uses the partition key as input to a hash function that maps the partition key and associated data to a specific shard. Specifically, an MD5 hash function is used to map partition\
  \ keys to 128-bit integer values and to map associated data records to shards. As a result of this hashing mechanism, all data records with the same partition key map to the same shard within the stream.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"PartitionKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-pipes/refs/heads/main/json-schema/amazon-eventbridge-pipes-pipe-target-kinesis-stream-parameters-schema.json
tags:
- Amazon Web Services
- Event-Driven
- Integration
- Messaging
- Serverless
title: PipeTargetKinesisStreamParameters
---
