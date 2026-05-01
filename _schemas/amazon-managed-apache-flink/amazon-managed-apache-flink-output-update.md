---
description: For a SQL-based Kinesis Data Analytics application, describes updates to the output configuration identified by the <code>OutputId</code>.
layout: schema
name: OutputUpdate
properties_list:
- description: ''
  name: OutputId
  type: object
- description: ''
  name: NameUpdate
  type: object
- description: ''
  name: KinesisStreamsOutputUpdate
  type: object
- description: ''
  name: KinesisFirehoseOutputUpdate
  type: object
- description: ''
  name: LambdaOutputUpdate
  type: object
- description: ''
  name: DestinationSchemaUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-output-update-schema.json
slug: amazon-managed-apache-flink-output-update
source_filename: amazon-managed-apache-flink-output-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-output-update-schema.json\",\n  \"title\": \"OutputUpdate\",\n  \"description\": \" For a SQL-based Kinesis Data Analytics application, describes updates to the output configuration identified by the <code>OutputId</code>. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"OutputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"Identifies the specific output configuration that you want to update.\"\n        }\n      ]\n    },\n    \"NameUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppStreamName\"\n        },\n        {\n          \"description\": \"If you want to specify a different in-application stream for this output configuration,\
  \ use this field to specify the new in-application stream name.\"\n        }\n      ]\n    },\n    \"KinesisStreamsOutputUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisStreamsOutputUpdate\"\n        },\n        {\n          \"description\": \"Describes a Kinesis data stream as the destination for the output.\"\n        }\n      ]\n    },\n    \"KinesisFirehoseOutputUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisFirehoseOutputUpdate\"\n        },\n        {\n          \"description\": \"Describes a Kinesis Data Firehose delivery stream as the destination for the output.\"\n        }\n      ]\n    },\n    \"LambdaOutputUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LambdaOutputUpdate\"\n        },\n        {\n          \"description\": \"Describes an Amazon Lambda function as the destination for the output.\"\n        }\n      ]\n    },\n    \"DestinationSchemaUpdate\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/DestinationSchema\"\n        },\n        {\n          \"description\": \"Describes the data format when records are written to the destination. \"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"OutputId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-output-update-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: OutputUpdate
---
