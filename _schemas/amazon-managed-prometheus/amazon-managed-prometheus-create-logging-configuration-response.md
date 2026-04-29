---
description: Represents the output of a CreateLoggingConfiguration operation.
layout: schema
name: CreateLoggingConfigurationResponse
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-create-logging-configuration-response-schema.json
slug: amazon-managed-prometheus-create-logging-configuration-response
source_filename: amazon-managed-prometheus-create-logging-configuration-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-logging-configuration-response-schema.json\",\n  \"title\": \"CreateLoggingConfigurationResponse\",\n  \"description\": \"Represents the output of a CreateLoggingConfiguration operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LoggingConfigurationStatus\"\n        },\n        {\n          \"description\": \"The status of the logging configuration.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-logging-configuration-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: CreateLoggingConfigurationResponse
---
