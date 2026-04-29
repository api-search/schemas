---
description: Describes configuration parameters for CloudWatch logging for an application.
layout: schema
name: MonitoringConfigurationDescription
properties_list:
- description: ''
  name: ConfigurationType
  type: object
- description: ''
  name: MetricsLevel
  type: object
- description: ''
  name: LogLevel
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-monitoring-configuration-description-schema.json
slug: amazon-managed-apache-flink-monitoring-configuration-description
source_filename: amazon-managed-apache-flink-monitoring-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-monitoring-configuration-description-schema.json\",\n  \"title\": \"MonitoringConfigurationDescription\",\n  \"description\": \"Describes configuration parameters for CloudWatch logging for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationType\"\n        },\n        {\n          \"description\": \"Describes whether to use the default CloudWatch logging configuration for an application.\"\n        }\n      ]\n    },\n    \"MetricsLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricsLevel\"\n        },\n        {\n          \"description\": \"Describes the granularity of the CloudWatch Logs for\
  \ an application.\"\n        }\n      ]\n    },\n    \"LogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"Describes the verbosity of the CloudWatch Logs for an application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-monitoring-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: MonitoringConfigurationDescription
---
