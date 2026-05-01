---
description: Represents the input of a CreateAlertManagerDefinition operation.
layout: schema
name: CreateAlertManagerDefinitionRequest
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: clientToken
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-create-alert-manager-definition-request-schema.json
slug: amazon-managed-prometheus-create-alert-manager-definition-request
source_filename: amazon-managed-prometheus-create-alert-manager-definition-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-alert-manager-definition-request-schema.json\",\n  \"title\": \"CreateAlertManagerDefinitionRequest\",\n  \"description\": \"Represents the input of a CreateAlertManagerDefinition operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertManagerDefinitionData\"\n        },\n        {\n          \"description\": \"The alert manager definition data.\"\n        }\n      ]\n    },\n    \"clientToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IdempotencyToken\"\n        },\n        {\n          \"description\": \"Optional, unique, case-sensitive, user-provided identifier to ensure the idempotency of the request.\"\n        }\n    \
  \  ]\n    }\n  },\n  \"required\": [\n    \"data\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-alert-manager-definition-request-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: CreateAlertManagerDefinitionRequest
---
