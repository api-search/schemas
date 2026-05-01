---
description: <p> Describes a SQL-based Kinesis Data Analytics application's output configuration, in which you identify an in-application stream and a destination where you want the in-application stream data to be written. The destination can be a Kinesis data stream or a Kinesis Data Firehose delivery stream. </p> <p/>
layout: schema
name: Output
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: KinesisStreamsOutput
  type: object
- description: ''
  name: KinesisFirehoseOutput
  type: object
- description: ''
  name: LambdaOutput
  type: object
- description: ''
  name: DestinationSchema
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-output-schema.json
slug: amazon-managed-apache-flink-output
source_filename: amazon-managed-apache-flink-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-output-schema.json\",\n  \"title\": \"Output\",\n  \"description\": \"<p> Describes a SQL-based Kinesis Data Analytics application's output configuration, in which you identify an in-application stream and a destination where you want the in-application stream data to be written. The destination can be a Kinesis data stream or a Kinesis Data Firehose delivery stream. </p> <p/>\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppStreamName\"\n        },\n        {\n          \"description\": \"The name of the in-application stream.\"\n        }\n      ]\n    },\n    \"KinesisStreamsOutput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisStreamsOutput\"\
  \n        },\n        {\n          \"description\": \"Identifies a Kinesis data stream as the destination.\"\n        }\n      ]\n    },\n    \"KinesisFirehoseOutput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisFirehoseOutput\"\n        },\n        {\n          \"description\": \"Identifies a Kinesis Data Firehose delivery stream as the destination.\"\n        }\n      ]\n    },\n    \"LambdaOutput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaOutput\"\n        },\n        {\n          \"description\": \"Identifies an Amazon Lambda function as the destination.\"\n        }\n      ]\n    },\n    \"DestinationSchema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationSchema\"\n        },\n        {\n          \"description\": \"Describes the data format when records are written to the destination. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Name\",\n\
  \    \"DestinationSchema\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-output-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: Output
---
