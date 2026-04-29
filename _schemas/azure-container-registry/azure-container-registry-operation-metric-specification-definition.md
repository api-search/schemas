---
description: The definition of Azure Monitoring metric.
layout: schema
name: OperationMetricSpecificationDefinition
properties_list:
- description: Metric aggregation type.
  name: aggregationType
  type: string
- description: Metric description.
  name: displayDescription
  type: string
- description: Metric display name.
  name: displayName
  type: string
- description: Internal metric name.
  name: internalMetricName
  type: string
- description: Metric name.
  name: name
  type: string
- description: Metric unit.
  name: unit
  type: string
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-operation-metric-specification-definition-schema.json
slug: azure-container-registry-operation-metric-specification-definition
source_filename: azure-container-registry-operation-metric-specification-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-metric-specification-definition-schema.json\",\n  \"title\": \"OperationMetricSpecificationDefinition\",\n  \"description\": \"The definition of Azure Monitoring metric.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"aggregationType\": {\n      \"description\": \"Metric aggregation type.\",\n      \"type\": \"string\"\n    },\n    \"displayDescription\": {\n      \"description\": \"Metric description.\",\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"description\": \"Metric display name.\",\n      \"type\": \"string\"\n    },\n    \"internalMetricName\": {\n      \"description\": \"Internal metric name.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"Metric name.\",\n      \"type\": \"string\"\n\
  \    },\n    \"unit\": {\n      \"description\": \"Metric unit.\",\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-metric-specification-definition-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: OperationMetricSpecificationDefinition
---
