---
description: The summary of the application version.
layout: schema
name: ApplicationVersionSummary
properties_list:
- description: ''
  name: ApplicationVersionId
  type: object
- description: ''
  name: ApplicationStatus
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-version-summary-schema.json
slug: amazon-managed-apache-flink-application-version-summary
source_filename: amazon-managed-apache-flink-application-version-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-version-summary-schema.json\",\n  \"title\": \"ApplicationVersionSummary\",\n  \"description\": \"The summary of the application version.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"The ID of the application version. Kinesis Data Analytics updates the <code>ApplicationVersionId</code> each time you update the application.\"\n        }\n      ]\n    },\n    \"ApplicationStatus\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationStatus\"\n        },\n        {\n          \"description\": \"The status of the application.\"\n     \
  \   }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationVersionId\",\n    \"ApplicationStatus\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-version-summary-schema.json
tags:
- Apache Flink
- AWS
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationVersionSummary
---
