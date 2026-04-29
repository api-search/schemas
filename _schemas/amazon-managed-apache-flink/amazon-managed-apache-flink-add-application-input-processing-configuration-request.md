---
description: AddApplicationInputProcessingConfigurationRequest schema from Amazon Managed Service for Apache Flink API
layout: schema
name: AddApplicationInputProcessingConfigurationRequest
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: CurrentApplicationVersionId
  type: object
- description: ''
  name: InputId
  type: object
- description: ''
  name: InputProcessingConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-add-application-input-processing-configuration-request-schema.json
slug: amazon-managed-apache-flink-add-application-input-processing-configuration-request
source_filename: amazon-managed-apache-flink-add-application-input-processing-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-input-processing-configuration-request-schema.json\",\n  \"title\": \"AddApplicationInputProcessingConfigurationRequest\",\n  \"description\": \"AddApplicationInputProcessingConfigurationRequest schema from Amazon Managed Service for Apache Flink API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application to which you want to add the input processing configuration.\"\n        }\n      ]\n    },\n    \"CurrentApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n \
  \         \"description\": \"The version of the application to which you want to add the input processing configuration. You can use the <a>DescribeApplication</a> operation to get the current application version. If the version specified is not the current version, the <code>ConcurrentModificationException</code> is returned.\"\n        }\n      ]\n    },\n    \"InputId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Id\"\n        },\n        {\n          \"description\": \"The ID of the input configuration to add the input processing configuration to. You can get a list of the input IDs for an application using the <a>DescribeApplication</a> operation.\"\n        }\n      ]\n    },\n    \"InputProcessingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/InputProcessingConfiguration\"\n        },\n        {\n          \"description\": \"The <a>InputProcessingConfiguration</a> to add to the application.\"\n    \
  \    }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"CurrentApplicationVersionId\",\n    \"InputId\",\n    \"InputProcessingConfiguration\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-add-application-input-processing-configuration-request-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: AddApplicationInputProcessingConfigurationRequest
---
