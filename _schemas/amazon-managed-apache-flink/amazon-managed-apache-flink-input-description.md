---
description: Describes the application input configuration for a SQL-based Kinesis Data Analytics application.
layout: schema
name: InputDescription
properties_list:
- description: ''
  name: InputId
  type: object
- description: ''
  name: NamePrefix
  type: object
- description: ''
  name: InAppStreamNames
  type: object
- description: ''
  name: InputProcessingConfigurationDescription
  type: object
- description: ''
  name: KinesisStreamsInputDescription
  type: object
- description: ''
  name: KinesisFirehoseInputDescription
  type: object
- description: ''
  name: InputSchema
  type: object
- description: ''
  name: InputParallelism
  type: object
- description: ''
  name: InputStartingPositionConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-description-schema.json
slug: amazon-managed-apache-flink-input-description
source_filename: amazon-managed-apache-flink-input-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-description-schema.json\",\n  \"title\": \"InputDescription\",\n  \"description\": \"Describes the application input configuration for a SQL-based Kinesis Data Analytics application. \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The input ID that is associated with the application input. This is the ID that Kinesis Data Analytics assigns to each input configuration that you add to your application. \"\n        }\n      ]\n    },\n    \"NamePrefix\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppStreamName\"\n        },\n        {\n          \"description\": \"The in-application\
  \ name prefix.\"\n        }\n      ]\n    },\n    \"InAppStreamNames\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppStreamNames\"\n        },\n        {\n          \"description\": \"Returns the in-application stream names that are mapped to the stream source. \"\n        }\n      ]\n    },\n    \"InputProcessingConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputProcessingConfigurationDescription\"\n        },\n        {\n          \"description\": \"The description of the preprocessor that executes on records in this input before the application's code is run. \"\n        }\n      ]\n    },\n    \"KinesisStreamsInputDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisStreamsInputDescription\"\n        },\n        {\n          \"description\": \"If a Kinesis data stream is configured as a streaming source, provides the Kinesis data stream's Amazon\
  \ Resource Name (ARN). \"\n        }\n      ]\n    },\n    \"KinesisFirehoseInputDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisFirehoseInputDescription\"\n        },\n        {\n          \"description\": \"If a Kinesis Data Firehose delivery stream is configured as a streaming source, provides the delivery stream's ARN. \"\n        }\n      ]\n    },\n    \"InputSchema\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SourceSchema\"\n        },\n        {\n          \"description\": \"Describes the format of the data in the streaming source, and how each data element maps to corresponding columns in the in-application stream that is being created. \"\n        }\n      ]\n    },\n    \"InputParallelism\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputParallelism\"\n        },\n        {\n          \"description\": \"Describes the configured parallelism (number of in-application\
  \ streams mapped to the streaming source). \"\n        }\n      ]\n    },\n    \"InputStartingPositionConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputStartingPositionConfiguration\"\n        },\n        {\n          \"description\": \"The point at which the application is configured to read from the input stream.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputDescription
---
