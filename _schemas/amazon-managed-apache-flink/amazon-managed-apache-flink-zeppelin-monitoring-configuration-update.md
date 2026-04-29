---
description: Updates to the monitoring configuration for Apache Zeppelin within a Kinesis Data Analytics Studio notebook.
layout: schema
name: ZeppelinMonitoringConfigurationUpdate
properties_list:
- description: ''
  name: LogLevelUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-update-schema.json
slug: amazon-managed-apache-flink-zeppelin-monitoring-configuration-update
source_filename: amazon-managed-apache-flink-zeppelin-monitoring-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-update-schema.json\",\n  \"title\": \"ZeppelinMonitoringConfigurationUpdate\",\n  \"description\": \"Updates to the monitoring configuration for Apache Zeppelin within a Kinesis Data Analytics Studio notebook.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"LogLevelUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogLevel\"\n        },\n        {\n          \"description\": \"Updates to the logging level for Apache Zeppelin within a Kinesis Data Analytics Studio notebook.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"LogLevelUpdate\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-zeppelin-monitoring-configuration-update-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ZeppelinMonitoringConfigurationUpdate
---
