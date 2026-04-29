---
description: The templated target type for the Amazon Kinesis <a href="kinesis/latest/APIReference/API_PutRecord.html"> <code>PutRecord</code> </a> API operation.
layout: schema
name: KinesisParameters
properties_list:
- description: ''
  name: PartitionKey
  type: object
provider_name: Amazon EventBridge Scheduler
provider_slug: amazon-eventbridge-scheduler
schema_file: json-schema/amazon-eventbridge-scheduler-kinesis-parameters-schema.json
slug: amazon-eventbridge-scheduler-kinesis-parameters
source_filename: amazon-eventbridge-scheduler-kinesis-parameters-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-kinesis-parameters-schema.json\",\n  \"title\": \"KinesisParameters\",\n  \"description\": \"The templated target type for the Amazon Kinesis <a href=\\\"kinesis/latest/APIReference/API_PutRecord.html\\\"> <code>PutRecord</code> </a> API operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PartitionKey\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/TargetPartitionKey\"\n        },\n        {\n          \"description\": \"Specifies the shard to which EventBridge Scheduler sends the event. For more information, see <a href=\\\"https://docs.aws.amazon.com/streams/latest/dev/key-concepts.html\\\">Amazon Kinesis Data Streams terminology and concepts</a> in the <i>Amazon Kinesis Streams Developer Guide</i>.\"\n        }\n\
  \      ]\n    }\n  },\n  \"required\": [\n    \"PartitionKey\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge-scheduler/refs/heads/main/json-schema/amazon-eventbridge-scheduler-kinesis-parameters-schema.json
tags:
- Amazon Web Services
- AWS
- Cron
- Event-Driven
- Scheduling
- Serverless
title: KinesisParameters
---
