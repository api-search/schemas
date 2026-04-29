---
description: Represents the output of a DescribeAlertManagerDefinition operation.
layout: schema
name: DescribeAlertManagerDefinitionResponse
properties_list:
- description: ''
  name: alertManagerDefinition
  type: object
provider_name: Amazon Managed Service for Prometheus
provider_slug: amazon-managed-prometheus
schema_file: json-schema/amazon-managed-prometheus-describe-alert-manager-definition-response-schema.json
slug: amazon-managed-prometheus-describe-alert-manager-definition-response
source_filename: amazon-managed-prometheus-describe-alert-manager-definition-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-describe-alert-manager-definition-response-schema.json\",\n  \"title\": \"DescribeAlertManagerDefinitionResponse\",\n  \"description\": \"Represents the output of a DescribeAlertManagerDefinition operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"alertManagerDefinition\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AlertManagerDefinitionDescription\"\n        },\n        {\n          \"description\": \"The properties of the selected workspace's alert manager definition.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"alertManagerDefinition\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-managed-prometheus/refs/heads/main/json-schema/amazon-managed-prometheus-describe-alert-manager-definition-response-schema.json
tags:
- AWS
- Containers
- Monitoring
- Observability
- Prometheus
title: DescribeAlertManagerDefinitionResponse
---
