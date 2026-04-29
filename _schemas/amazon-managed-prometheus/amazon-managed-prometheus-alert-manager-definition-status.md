---
description: Represents the status of a definition.
layout: schema
name: AlertManagerDefinitionStatus
properties_list:
- description: ''
  name: statusCode
  type: object
- description: ''
  name: statusReason
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-alert-manager-definition-status-schema.json
slug: amazon-managed-prometheus-alert-manager-definition-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-alert-manager-definition-status-schema.json\",\n  \"title\": \"AlertManagerDefinitionStatus\",\n  \"description\": \"Represents the status of a definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertManagerDefinitionStatusCode\"\n        },\n        {\n          \"description\": \"Status code of this definition.\"\n        }\n      ]\n    },\n    \"statusReason\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"The reason for failure if any.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"statusCode\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-alert-manager-definition-status-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: AlertManagerDefinitionStatus
---
