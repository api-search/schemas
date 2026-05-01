---
description: Describes configuration parameters for Amazon CloudWatch logging for a Kinesis Data Analytics Studio notebook. For more information about CloudWatch logging, see <a href="https://docs.aws.amazon.com/kinesisanalytics/latest/java/monitoring-overview.html">Monitoring</a>.
layout: schema
name: ZeppelinMonitoringConfiguration
properties_list:
- description: ''
  name: LogLevel
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-schema.json
slug: amazon-managed-apache-flink-zeppelin-monitoring-configuration
source_filename: amazon-managed-apache-flink-zeppelin-monitoring-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-schema.json\",\n  \"title\": \"ZeppelinMonitoringConfiguration\",\n  \"description\": \"Describes configuration parameters for Amazon CloudWatch logging for a Kinesis Data Analytics Studio notebook. For more information about CloudWatch logging, see <a href=\\\"https://docs.aws.amazon.com/kinesisanalytics/latest/java/monitoring-overview.html\\\">Monitoring</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"The verbosity of the CloudWatch Logs for an application.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LogLevel\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ZeppelinMonitoringConfiguration
---
