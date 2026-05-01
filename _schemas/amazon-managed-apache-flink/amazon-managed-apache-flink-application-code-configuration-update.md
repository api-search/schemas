---
description: Describes code configuration updates for an application. This is supported for a Flink-based Kinesis Data Analytics application or a SQL-based Kinesis Data Analytics application.
layout: schema
name: ApplicationCodeConfigurationUpdate
properties_list:
- description: ''
  name: CodeContentTypeUpdate
  type: object
- description: ''
  name: CodeContentUpdate
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-code-configuration-update-schema.json
slug: amazon-managed-apache-flink-application-code-configuration-update
source_filename: amazon-managed-apache-flink-application-code-configuration-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-code-configuration-update-schema.json\",\n  \"title\": \"ApplicationCodeConfigurationUpdate\",\n  \"description\": \"Describes code configuration updates for an application. This is supported for a Flink-based Kinesis Data Analytics application or a SQL-based Kinesis Data Analytics application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeContentTypeUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeContentType\"\n        },\n        {\n          \"description\": \"Describes updates to the code content type.\"\n        }\n      ]\n    },\n    \"CodeContentUpdate\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeContentUpdate\"\n        },\n        {\n          \"\
  description\": \"Describes updates to the code content of an application.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-code-configuration-update-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationCodeConfigurationUpdate
---
