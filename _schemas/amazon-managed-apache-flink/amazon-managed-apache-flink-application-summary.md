---
description: Provides application summary information, including the application Amazon Resource Name (ARN), name, and status.
layout: schema
name: ApplicationSummary
properties_list:
- description: ''
  name: ApplicationName
  type: object
- description: ''
  name: ApplicationARN
  type: object
- description: ''
  name: ApplicationStatus
  type: object
- description: ''
  name: ApplicationVersionId
  type: object
- description: ''
  name: RuntimeEnvironment
  type: object
- description: ''
  name: ApplicationMode
  type: object
provider_name: Amazon Managed Service for Apache Flink
provider_slug: amazon-managed-apache-flink
schema_file: json-schema/amazon-managed-apache-flink-application-summary-schema.json
slug: amazon-managed-apache-flink-application-summary
source_filename: amazon-managed-apache-flink-application-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-summary-schema.json\",\n  \"title\": \"ApplicationSummary\",\n  \"description\": \"Provides application summary information, including the application Amazon Resource Name (ARN), name, and status.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ApplicationName\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationName\"\n        },\n        {\n          \"description\": \"The name of the application.\"\n        }\n      ]\n    },\n    \"ApplicationARN\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ResourceARN\"\n        },\n        {\n          \"description\": \"The ARN of the application.\"\n        }\n      ]\n    },\n    \"ApplicationStatus\": {\n      \"allOf\": [\n   \
  \     {\n          \"$ref\": \"#/components/schemas/ApplicationStatus\"\n        },\n        {\n          \"description\": \"The status of the application.\"\n        }\n      ]\n    },\n    \"ApplicationVersionId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationVersionId\"\n        },\n        {\n          \"description\": \"Provides the current application version.\"\n        }\n      ]\n    },\n    \"RuntimeEnvironment\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RuntimeEnvironment\"\n        },\n        {\n          \"description\": \"The runtime environment for the application.\"\n        }\n      ]\n    },\n    \"ApplicationMode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ApplicationMode\"\n        },\n        {\n          \"description\": \"For a Kinesis Data Analytics for Apache Flink application, the mode is <code>STREAMING</code>. For a Kinesis Data Analytics Studio\
  \ notebook, it is <code>INTERACTIVE</code>.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"ApplicationName\",\n    \"ApplicationARN\",\n    \"ApplicationStatus\",\n    \"ApplicationVersionId\",\n    \"RuntimeEnvironment\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-apache-flink/refs/heads/main/json-schema/amazon-managed-apache-flink-application-summary-schema.json
tags:
- Apache Flink
- Big Data
- Real-Time Processing
- Streaming Analytics
title: ApplicationSummary
---
