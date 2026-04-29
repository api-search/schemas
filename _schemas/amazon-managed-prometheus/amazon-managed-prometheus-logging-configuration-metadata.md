---
description: Represents the properties of a logging configuration metadata.
layout: schema
name: LoggingConfigurationMetadata
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: workspace
  type: object
- description: ''
  name: logGroupArn
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: modifiedAt
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-logging-configuration-metadata-schema.json
slug: amazon-managed-prometheus-logging-configuration-metadata
source_filename: amazon-managed-prometheus-logging-configuration-metadata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-logging-configuration-metadata-schema.json\",\n  \"title\": \"LoggingConfigurationMetadata\",\n  \"description\": \"Represents the properties of a logging configuration metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfigurationStatus\"\n        },\n        {\n          \"description\": \"The status of the logging configuration.\"\n        }\n      ]\n    },\n    \"workspace\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/WorkspaceId\"\n        },\n        {\n          \"description\": \"The workspace where the logging configuration exists.\"\n        }\n      ]\n    },\n    \"logGroupArn\": {\n      \"allOf\": [\n        {\n\
  \          \"$ref\": \"#/components/schemas/LogGroupArn\"\n        },\n        {\n          \"description\": \"The ARN of the CW log group to which the vended log data will be published.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the logging configuration was created.\"\n        }\n      ]\n    },\n    \"modifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the logging configuration was modified.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"workspace\",\n    \"logGroupArn\",\n    \"createdAt\",\n    \"modifiedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-logging-configuration-metadata-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: LoggingConfigurationMetadata
---
