---
description: An Amazon Kinesis Data Firehose delivery stream.
layout: schema
name: DeliveryStream
properties_list:
- description: The name of the delivery stream.
  name: DeliveryStreamName
  type: string
- description: The ARN of the delivery stream.
  name: DeliveryStreamARN
  type: string
- description: The status of the delivery stream.
  name: DeliveryStreamStatus
  type: string
- description: The type of the delivery stream.
  name: DeliveryStreamType
  type: string
- description: The date and time the delivery stream was created.
  name: CreateTimestamp
  type: string
- description: The date and time the delivery stream was last updated.
  name: LastUpdateTimestamp
  type: string
provider_name: Amazon Kinesis Data Firehose
provider_slug: amazon-kinesis-firehose
schema_file: json-schema/amazon-kinesis-firehose-delivery-stream-schema.json
slug: amazon-kinesis-firehose-delivery-stream
source_filename: amazon-kinesis-firehose-delivery-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-firehose/refs/heads/main/json-schema/amazon-kinesis-firehose-delivery-stream-schema.json\",\n  \"title\": \"DeliveryStream\",\n  \"description\": \"An Amazon Kinesis Data Firehose delivery stream.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"DeliveryStreamName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the delivery stream.\",\n      \"example\": \"my-firehose-stream\"\n    },\n    \"DeliveryStreamARN\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the delivery stream.\"\n    },\n    \"DeliveryStreamStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the delivery stream.\",\n      \"example\": \"ACTIVE\",\n      \"enum\": [\n        \"CREATING\",\n        \"CREATING_FAILED\",\n        \"DELETING\",\n        \"DELETING_FAILED\",\n        \"ACTIVE\"\
  \n      ]\n    },\n    \"DeliveryStreamType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the delivery stream.\",\n      \"example\": \"DirectPut\",\n      \"enum\": [\n        \"DirectPut\",\n        \"KinesisStreamAsSource\",\n        \"MSKAsSource\"\n      ]\n    },\n    \"CreateTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the delivery stream was created.\",\n      \"format\": \"date-time\"\n    },\n    \"LastUpdateTimestamp\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the delivery stream was last updated.\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-kinesis-firehose/refs/heads/main/json-schema/amazon-kinesis-firehose-delivery-stream-schema.json
tags:
- Analytics
- AWS
- Data Delivery
- Streaming
title: DeliveryStream
---
