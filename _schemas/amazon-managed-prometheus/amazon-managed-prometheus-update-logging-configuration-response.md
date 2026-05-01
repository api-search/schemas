---
description: Represents the output of an UpdateLoggingConfiguration operation.
layout: schema
name: UpdateLoggingConfigurationResponse
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-update-logging-configuration-response-schema.json
slug: amazon-managed-prometheus-update-logging-configuration-response
source_filename: amazon-managed-prometheus-update-logging-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-update-logging-configuration-response-schema.json\",\n  \"title\": \"UpdateLoggingConfigurationResponse\",\n  \"description\": \"Represents the output of an UpdateLoggingConfiguration operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfigurationStatus\"\n        },\n        {\n          \"description\": \"The status of the logging configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-update-logging-configuration-response-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: UpdateLoggingConfigurationResponse
---
