---
description: Represents the output of a CreateAlertManagerDefinition operation.
layout: schema
name: CreateAlertManagerDefinitionResponse
properties_list:
- description: ''
  name: status
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-create-alert-manager-definition-response-schema.json
slug: amazon-managed-prometheus-create-alert-manager-definition-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-alert-manager-definition-response-schema.json\",\n  \"title\": \"CreateAlertManagerDefinitionResponse\",\n  \"description\": \"Represents the output of a CreateAlertManagerDefinition operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertManagerDefinitionStatus\"\n        },\n        {\n          \"description\": \"The status of alert manager definition.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-create-alert-manager-definition-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: CreateAlertManagerDefinitionResponse
---
