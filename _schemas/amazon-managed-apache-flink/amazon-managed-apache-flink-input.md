---
description: When you configure the application input for a SQL-based Kinesis Data Analytics application, you specify the streaming source, the in-application stream name that is created, and the mapping between the two.
layout: schema
name: Input
properties_list:
- description: ''
  name: NamePrefix
  type: object
- description: ''
  name: InputProcessingConfiguration
  type: object
- description: ''
  name: KinesisStreamsInput
  type: object
- description: ''
  name: KinesisFirehoseInput
  type: object
- description: ''
  name: InputParallelism
  type: object
- description: ''
  name: InputSchema
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-schema.json
slug: amazon-managed-apache-flink-input
source_filename: amazon-managed-apache-flink-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-schema.json\",\n  \"title\": \"Input\",\n  \"description\": \"When you configure the application input for a SQL-based Kinesis Data Analytics application, you specify the streaming source, the in-application stream name that is created, and the mapping between the two. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NamePrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppStreamName\"\n        },\n        {\n          \"description\": \"The name prefix to use when creating an in-application stream. Suppose that you specify a prefix \\\"<code>MyInApplicationStream</code>.\\\" Kinesis Data Analytics then creates one or more (as per the <code>InputParallelism</code> count you specified) in-application streams with\
  \ the names \\\"<code>MyInApplicationStream_001</code>,\\\" \\\"<code>MyInApplicationStream_002</code>,\\\" and so on. \"\n        }\n      ]\n    },\n    \"InputProcessingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputProcessingConfiguration\"\n        },\n        {\n          \"description\": \"The <a>InputProcessingConfiguration</a> for the input. An input processor transforms records as they are received from the stream, before the application's SQL code executes. Currently, the only input processing configuration available is <a>InputLambdaProcessor</a>. \"\n        }\n      ]\n    },\n    \"KinesisStreamsInput\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisStreamsInput\"\n        },\n        {\n          \"description\": \"If the streaming source is an Amazon Kinesis data stream, identifies the stream's Amazon Resource Name (ARN). \"\n        }\n      ]\n    },\n    \"KinesisFirehoseInput\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisFirehoseInput\"\n        },\n        {\n          \"description\": \"If the streaming source is an Amazon Kinesis Data Firehose delivery stream, identifies the delivery stream's ARN.\"\n        }\n      ]\n    },\n    \"InputParallelism\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputParallelism\"\n        },\n        {\n          \"description\": \"Describes the number of in-application streams to create. \"\n        }\n      ]\n    },\n    \"InputSchema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceSchema\"\n        },\n        {\n          \"description\": \"<p>Describes the format of the data in the streaming source, and how each data element maps to corresponding columns in the in-application stream that is being created.</p> <p>Also used to describe the format of the reference data source.</p>\"\n        }\n      ]\n  \
  \  }\n  },\n  \"required\": [\n    \"NamePrefix\",\n    \"InputSchema\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: Input
---
