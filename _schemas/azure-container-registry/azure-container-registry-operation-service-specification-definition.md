---
description: The definition of Azure Monitoring list.
layout: schema
name: OperationServiceSpecificationDefinition
properties_list:
- description: A list of Azure Monitoring metrics definition.
  name: metricSpecifications
  type: array
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-operation-service-specification-definition-schema.json
slug: azure-container-registry-operation-service-specification-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-service-specification-definition-schema.json\",\n  \"title\": \"OperationServiceSpecificationDefinition\",\n  \"description\": \"The definition of Azure Monitoring list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metricSpecifications\": {\n      \"description\": \"A list of Azure Monitoring metrics definition.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/OperationMetricSpecificationDefinition\"\n      },\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-service-specification-definition-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: OperationServiceSpecificationDefinition
---
