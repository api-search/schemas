---
description: Represents the properties of an alert manager definition.
layout: schema
name: AlertManagerDefinitionDescription
properties_list:
- description: ''
  name: status
  type: object
- description: ''
  name: data
  type: object
- description: ''
  name: createdAt
  type: object
- description: ''
  name: modifiedAt
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-alert-manager-definition-description-schema.json
slug: amazon-managed-prometheus-alert-manager-definition-description
source_filename: amazon-managed-prometheus-alert-manager-definition-description-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-alert-manager-definition-description-schema.json\",\n  \"title\": \"AlertManagerDefinitionDescription\",\n  \"description\": \"Represents the properties of an alert manager definition.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertManagerDefinitionStatus\"\n        },\n        {\n          \"description\": \"The status of alert manager definition.\"\n        }\n      ]\n    },\n    \"data\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertManagerDefinitionData\"\n        },\n        {\n          \"description\": \"The alert manager definition.\"\n        }\n      ]\n    },\n    \"createdAt\": {\n      \"allOf\": [\n        {\n      \
  \    \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the alert manager definition was created.\"\n        }\n      ]\n    },\n    \"modifiedAt\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Timestamp\"\n        },\n        {\n          \"description\": \"The time when the alert manager definition was modified.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"data\",\n    \"createdAt\",\n    \"modifiedAt\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-alert-manager-definition-description-schema.json
tags:
- Containers
- Monitoring
- Observability
- Prometheus
title: AlertManagerDefinitionDescription
---
