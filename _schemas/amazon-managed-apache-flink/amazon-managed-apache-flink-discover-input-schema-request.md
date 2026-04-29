---
description: DiscoverInputSchemaRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DiscoverInputSchemaRequest
properties_list:
- description: ''
  name: ResourceARN
  type: object
- description: ''
  name: ServiceExecutionRole
  type: object
- description: ''
  name: InputStartingPositionConfiguration
  type: object
- description: ''
  name: S3Configuration
  type: object
- description: ''
  name: InputProcessingConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-discover-input-schema-request-schema.json
slug: amazon-managed-apache-flink-discover-input-schema-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-discover-input-schema-request-schema.json\",\n  \"title\": \"DiscoverInputSchemaRequest\",\n  \"description\": \"DiscoverInputSchemaRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ResourceARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the streaming source.\"\n        }\n      ]\n    },\n    \"ServiceExecutionRole\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RoleARN\"\n        },\n        {\n          \"description\": \"The ARN of the role that is used to access the streaming source.\"\n        }\n      ]\n    },\n    \"InputStartingPositionConfiguration\"\
  : {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputStartingPositionConfiguration\"\n        },\n        {\n          \"description\": \"The point at which you want Kinesis Data Analytics to start reading records from the specified streaming source discovery purposes.\"\n        }\n      ]\n    },\n    \"S3Configuration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/S3Configuration\"\n        },\n        {\n          \"description\": \"Specify this parameter to discover a schema from data in an Amazon S3 object.\"\n        }\n      ]\n    },\n    \"InputProcessingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputProcessingConfiguration\"\n        },\n        {\n          \"description\": \"The <a>InputProcessingConfiguration</a> to use to preprocess the records before discovering the schema of the records.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ServiceExecutionRole\"\
  \n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-discover-input-schema-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DiscoverInputSchemaRequest
---
