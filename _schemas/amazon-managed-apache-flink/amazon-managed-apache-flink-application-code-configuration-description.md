---
description: Describes code configuration for an application.
layout: schema
name: ApplicationCodeConfigurationDescription
properties_list:
- description: ''
  name: CodeContentType
  type: object
- description: ''
  name: CodeContentDescription
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-code-configuration-description-schema.json
slug: amazon-managed-apache-flink-application-code-configuration-description
source_filename: amazon-managed-apache-flink-application-code-configuration-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-code-configuration-description-schema.json\",\n  \"title\": \"ApplicationCodeConfigurationDescription\",\n  \"description\": \"Describes code configuration for an application.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CodeContentType\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeContentType\"\n        },\n        {\n          \"description\": \"Specifies whether the code content is in text or zip format.\"\n        }\n      ]\n    },\n    \"CodeContentDescription\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/CodeContentDescription\"\n        },\n        {\n          \"description\": \"Describes details about the location and format of the application code.\"\n      \
  \  }\n      ]\n    }\n  },\n  \"required\": [\n    \"CodeContentType\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-code-configuration-description-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationCodeConfigurationDescription
---
