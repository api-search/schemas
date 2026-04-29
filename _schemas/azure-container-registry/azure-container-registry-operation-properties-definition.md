---
description: The definition of Azure Monitoring properties.
layout: schema
name: OperationPropertiesDefinition
properties_list:
- description: The definition of Azure Monitoring service.
  name: serviceSpecification
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-operation-properties-definition-schema.json
slug: azure-container-registry-operation-properties-definition
source_filename: azure-container-registry-operation-properties-definition-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-properties-definition-schema.json\",\n  \"title\": \"OperationPropertiesDefinition\",\n  \"description\": \"The definition of Azure Monitoring properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceSpecification\": {\n      \"$ref\": \"#/definitions/OperationServiceSpecificationDefinition\",\n      \"description\": \"The definition of Azure Monitoring service.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-container-registry/refs/heads/main/json-schema/azure-container-registry-operation-properties-definition-schema.json
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: OperationPropertiesDefinition
---
