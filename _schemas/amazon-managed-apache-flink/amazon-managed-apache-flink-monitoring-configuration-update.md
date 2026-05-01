---
description: Describes updates to configuration parameters for Amazon CloudWatch logging for an application.
layout: schema
name: MonitoringConfigurationUpdate
properties_list:
- description: ''
  name: ConfigurationTypeUpdate
  type: object
- description: ''
  name: MetricsLevelUpdate
  type: object
- description: ''
  name: LogLevelUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-monitoring-configuration-update-schema.json
slug: amazon-managed-apache-flink-monitoring-configuration-update
source_filename: amazon-managed-apache-flink-monitoring-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-monitoring-configuration-update-schema.json\",\n  \"title\": \"MonitoringConfigurationUpdate\",\n  \"description\": \"Describes updates to configuration parameters for Amazon CloudWatch logging for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationTypeUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationType\"\n        },\n        {\n          \"description\": \"Describes updates to whether to use the default CloudWatch logging configuration for an application. You must set this property to <code>CUSTOM</code> in order to set the <code>LogLevel</code> or <code>MetricsLevel</code> parameters.\"\n        }\n      ]\n    },\n    \"MetricsLevelUpdate\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/MetricsLevel\"\n        },\n        {\n          \"description\": \"Describes updates to the granularity of the CloudWatch Logs for an application. The <code>Parallelism</code> level is not recommended for applications with a Parallelism over 64 due to excessive costs.\"\n        }\n      ]\n    },\n    \"LogLevelUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"Describes updates to the verbosity of the CloudWatch Logs for an application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-monitoring-configuration-update-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: MonitoringConfigurationUpdate
---
