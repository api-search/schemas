---
description: Represents the status of a logging configuration.
layout: schema
name: LoggingConfigurationStatus
properties_list:
- description: ''
  name: statusCode
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-logging-configuration-status-schema.json
slug: amazon-managed-prometheus-logging-configuration-status
source_filename: amazon-managed-prometheus-logging-configuration-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-logging-configuration-status-schema.json\",\n  \"title\": \"LoggingConfigurationStatus\",\n  \"description\": \"Represents the status of a logging configuration.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfigurationStatusCode\"\n        },\n        {\n          \"description\": \"Status code of the logging configuration.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason for failure if any.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"statusCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-logging-configuration-status-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: LoggingConfigurationStatus
---
