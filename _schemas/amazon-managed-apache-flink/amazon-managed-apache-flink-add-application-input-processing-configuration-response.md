---
description: AddApplicationInputProcessingConfigurationResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: AddApplicationInputProcessingConfigurationResponse
properties_list:
- description: ''
  name: ApplicationARN
  type: object
- description: ''
  name: ApplicationVersionId
  type: object
- description: ''
  name: InputId
  type: object
- description: ''
  name: InputProcessingConfigurationDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-add-application-input-processing-configuration-response-schema.json
slug: amazon-managed-apache-flink-add-application-input-processing-configuration-response
source_filename: amazon-managed-apache-flink-add-application-input-processing-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-input-processing-configuration-response-schema.json\",\n  \"title\": \"AddApplicationInputProcessingConfigurationResponse\",\n  \"description\": \"AddApplicationInputProcessingConfigurationResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the application.\"\n        }\n      ]\n    },\n    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"Provides the current\
  \ application version. \"\n        }\n      ]\n    },\n    \"InputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The input ID that is associated with the application input. This is the ID that Kinesis Data Analytics assigns to each input configuration that you add to your application.\"\n        }\n      ]\n    },\n    \"InputProcessingConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputProcessingConfigurationDescription\"\n        },\n        {\n          \"description\": \"The description of the preprocessor that executes on records in this input before the application's code is run.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-input-processing-configuration-response-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: AddApplicationInputProcessingConfigurationResponse
---
