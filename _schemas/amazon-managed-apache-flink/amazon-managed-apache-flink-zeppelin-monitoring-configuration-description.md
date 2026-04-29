---
description: The monitoring configuration for Apache Zeppelin within a Kinesis Data Analytics Studio notebook.
layout: schema
name: ZeppelinMonitoringConfigurationDescription
properties_list:
- description: ''
  name: LogLevel
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-description-schema.json
slug: amazon-managed-apache-flink-zeppelin-monitoring-configuration-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-description-schema.json\",\n  \"title\": \"ZeppelinMonitoringConfigurationDescription\",\n  \"description\": \"The monitoring configuration for Apache Zeppelin within a Kinesis Data Analytics Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogLevel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"Describes the verbosity of the CloudWatch Logs for an application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ZeppelinMonitoringConfigurationDescription
---
