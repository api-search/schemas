---
description: DeleteApplicationInputProcessingConfigurationResponse schema from Amazon Managed Service for Apache Flink API
layout: schema
name: DeleteApplicationInputProcessingConfigurationResponse
properties_list:
- description: ''
  name: ApplicationARN
  type: object
- description: ''
  name: ApplicationVersionId
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-delete-application-input-processing-configuration-response-schema.json
slug: amazon-managed-apache-flink-delete-application-input-processing-configuration-response
source_filename: amazon-managed-apache-flink-delete-application-input-processing-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-input-processing-configuration-response-schema.json\",\n  \"title\": \"DeleteApplicationInputProcessingConfigurationResponse\",\n  \"description\": \"DeleteApplicationInputProcessingConfigurationResponse schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The Amazon Resource Name (ARN) of the application.\"\n        }\n      ]\n    },\n    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The current\
  \ application version ID.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-delete-application-input-processing-configuration-response-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: DeleteApplicationInputProcessingConfigurationResponse
---
