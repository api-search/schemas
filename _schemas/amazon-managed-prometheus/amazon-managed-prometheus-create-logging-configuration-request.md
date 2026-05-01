---
description: Represents the input of a CreateLoggingConfiguration operation.
layout: schema
name: CreateLoggingConfigurationRequest
properties_list:
- description: ''
  name: logGroupArn
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-create-logging-configuration-request-schema.json
slug: amazon-managed-prometheus-create-logging-configuration-request
source_filename: amazon-managed-prometheus-create-logging-configuration-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-logging-configuration-request-schema.json\",\n  \"title\": \"CreateLoggingConfigurationRequest\",\n  \"description\": \"Represents the input of a CreateLoggingConfiguration operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"logGroupArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LogGroupArn\"\n        },\n        {\n          \"description\": \"The ARN of the CW log group to which the vended log data will be published.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"Optional, unique, case-sensitive, user-provided identifier to ensure the idempotency of the request.\"\
  \n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"logGroupArn\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-logging-configuration-request-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: CreateLoggingConfigurationRequest
---
