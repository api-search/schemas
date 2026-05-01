---
description: Describes the updates to the starting parameters for a Kinesis Data Analytics application.
layout: schema
name: RunConfigurationUpdate
properties_list:
- description: ''
  name: FlinkRunConfiguration
  type: object
- description: ''
  name: ApplicationRestoreConfiguration
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-run-configuration-update-schema.json
slug: amazon-managed-apache-flink-run-configuration-update
source_filename: amazon-managed-apache-flink-run-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-run-configuration-update-schema.json\",\n  \"title\": \"RunConfigurationUpdate\",\n  \"description\": \"Describes the updates to the starting parameters for a Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FlinkRunConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/FlinkRunConfiguration\"\n        },\n        {\n          \"description\": \"Describes the starting parameters for a Flink-based Kinesis Data Analytics application.\"\n        }\n      ]\n    },\n    \"ApplicationRestoreConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationRestoreConfiguration\"\n        },\n        {\n          \"description\": \"Describes updates to\
  \ the restore behavior of a restarting application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-run-configuration-update-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: RunConfigurationUpdate
---
