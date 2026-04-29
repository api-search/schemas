---
description: For a SQL-based Kinesis Data Analytics application, describes updates to a specific input configuration (identified by the <code>InputId</code> of an application).
layout: schema
name: InputUpdate
properties_list:
- description: ''
  name: InputId
  type: object
- description: ''
  name: NamePrefixUpdate
  type: object
- description: ''
  name: InputProcessingConfigurationUpdate
  type: object
- description: ''
  name: KinesisStreamsInputUpdate
  type: object
- description: ''
  name: KinesisFirehoseInputUpdate
  type: object
- description: ''
  name: InputSchemaUpdate
  type: object
- description: ''
  name: InputParallelismUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-input-update-schema.json
slug: amazon-managed-apache-flink-input-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-update-schema.json\",\n  \"title\": \"InputUpdate\",\n  \"description\": \"For a SQL-based Kinesis Data Analytics application, describes updates to a specific input configuration (identified by the <code>InputId</code> of an application). \",\n  \"type\": \"object\",\n  \"properties\": {\n    \"InputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The input ID of the application input to be updated.\"\n        }\n      ]\n    },\n    \"NamePrefixUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InAppStreamName\"\n        },\n        {\n          \"description\": \"The name prefix for in-application streams that Kinesis Data Analytics\
  \ creates for the specific streaming source.\"\n        }\n      ]\n    },\n    \"InputProcessingConfigurationUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputProcessingConfigurationUpdate\"\n        },\n        {\n          \"description\": \"Describes updates to an <a>InputProcessingConfiguration</a>.\"\n        }\n      ]\n    },\n    \"KinesisStreamsInputUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisStreamsInputUpdate\"\n        },\n        {\n          \"description\": \"If a Kinesis data stream is the streaming source to be updated, provides an updated stream Amazon Resource Name (ARN).\"\n        }\n      ]\n    },\n    \"KinesisFirehoseInputUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/KinesisFirehoseInputUpdate\"\n        },\n        {\n          \"description\": \"If a Kinesis Data Firehose delivery stream is the streaming source to be updated, provides\
  \ an updated stream ARN.\"\n        }\n      ]\n    },\n    \"InputSchemaUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputSchemaUpdate\"\n        },\n        {\n          \"description\": \"Describes the data format on the streaming source, and how record elements on the streaming source map to columns of the in-application stream that is created.\"\n        }\n      ]\n    },\n    \"InputParallelismUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputParallelismUpdate\"\n        },\n        {\n          \"description\": \"Describes the parallelism updates (the number of in-application streams Kinesis Data Analytics creates for the specific streaming source).\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"InputId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-input-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: InputUpdate
---
