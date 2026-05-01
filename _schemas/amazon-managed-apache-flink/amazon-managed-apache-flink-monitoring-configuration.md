---
description: Describes configuration parameters for Amazon CloudWatch logging for an application. For more information about CloudWatch logging, see <a href="https://docs.aws.amazon.com/kinesisanalytics/latest/java/monitoring-overview.html">Monitoring</a>.
layout: schema
name: MonitoringConfiguration
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
schema_file: json-schema/amazon-managed-apache-flink-monitoring-configuration-schema.json
slug: amazon-managed-apache-flink-monitoring-configuration
source_filename: amazon-managed-apache-flink-monitoring-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-monitoring-configuration-schema.json\",\n  \"title\": \"MonitoringConfiguration\",\n  \"description\": \"Describes configuration parameters for Amazon CloudWatch logging for an application. For more information about CloudWatch logging, see <a href=\\\"https://docs.aws.amazon.com/kinesisanalytics/latest/java/monitoring-overview.html\\\">Monitoring</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ConfigurationType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ConfigurationType\"\n        },\n        {\n          \"description\": \"Describes whether to use the default CloudWatch logging configuration for an application. You must set this property to <code>CUSTOM</code> in order to set the <code>LogLevel</code> or <code>MetricsLevel</code>\
  \ parameters.\"\n        }\n      ]\n    },\n    \"MetricsLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/MetricsLevel\"\n        },\n        {\n          \"description\": \"Describes the granularity of the CloudWatch Logs for an application. The <code>Parallelism</code> level is not recommended for applications with a Parallelism over 64 due to excessive costs.\"\n        }\n      ]\n    },\n    \"LogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"Describes the verbosity of the CloudWatch Logs for an application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ConfigurationType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-monitoring-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: MonitoringConfiguration
---
