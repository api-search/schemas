---
description: For a SQL-based Kinesis Data Analytics application, describes the application output configuration, which includes the in-application stream name and the destination where the stream data is written. The destination can be a Kinesis data stream or a Kinesis Data Firehose delivery stream.
layout: schema
name: OutputDescription
properties_list:
- description: ''
  name: OutputId
  type: object
- description: ''
  name: Name
  type: object
- description: ''
  name: KinesisStreamsOutputDescription
  type: object
- description: ''
  name: KinesisFirehoseOutputDescription
  type: object
- description: ''
  name: LambdaOutputDescription
  type: object
- description: ''
  name: DestinationSchema
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-output-description-schema.json
slug: amazon-managed-apache-flink-output-description
source_filename: amazon-managed-apache-flink-output-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-output-description-schema.json\",\n  \"title\": \"OutputDescription\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, describes the application output configuration, which includes the in-application stream name and the destination where the stream data is written. The destination can be a Kinesis data stream or a Kinesis Data Firehose delivery stream. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"A unique identifier for the output configuration.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppStreamName\"\
  \n        },\n        {\n          \"description\": \"The name of the in-application stream that is configured as output.\"\n        }\n      ]\n    },\n    \"KinesisStreamsOutputDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisStreamsOutputDescription\"\n        },\n        {\n          \"description\": \"Describes the Kinesis data stream that is configured as the destination where output is written.\"\n        }\n      ]\n    },\n    \"KinesisFirehoseOutputDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisFirehoseOutputDescription\"\n        },\n        {\n          \"description\": \"Describes the Kinesis Data Firehose delivery stream that is configured as the destination where output is written.\"\n        }\n      ]\n    },\n    \"LambdaOutputDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaOutputDescription\"\n        },\n        {\n\
  \          \"description\": \"Describes the Lambda function that is configured as the destination where output is written.\"\n        }\n      ]\n    },\n    \"DestinationSchema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationSchema\"\n        },\n        {\n          \"description\": \"The data format used for writing data to the destination.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-output-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: OutputDescription
---
