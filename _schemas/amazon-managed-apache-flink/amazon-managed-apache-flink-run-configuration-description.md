---
description: Describes the starting properties for a Kinesis Data Analytics application.
layout: schema
name: RunConfigurationDescription
properties_list:
- description: ''
  name: ApplicationRestoreConfigurationDescription
  type: object
- description: ''
  name: FlinkRunConfigurationDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-run-configuration-description-schema.json
slug: amazon-managed-apache-flink-run-configuration-description
source_filename: amazon-managed-apache-flink-run-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-run-configuration-description-schema.json\",\n  \"title\": \"RunConfigurationDescription\",\n  \"description\": \"Describes the starting properties for a Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationRestoreConfigurationDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationRestoreConfiguration\"\n        },\n        {\n          \"description\": \"Describes the restore behavior of a restarting application.\"\n        }\n      ]\n    },\n    \"FlinkRunConfigurationDescription\": {\n      \"$ref\": \"#/components/schemas/FlinkRunConfiguration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-run-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: RunConfigurationDescription
---
