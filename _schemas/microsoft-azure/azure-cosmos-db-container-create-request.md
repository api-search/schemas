---
description: Request body for creating or replacing a container.
layout: schema
name: ContainerCreateRequest
properties_list:
- description: The unique name that identifies the container.
  name: id
  type: string
- description: Default time-to-live in seconds.
  name: defaultTtl
  type: integer
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-container-create-request-schema.json
slug: azure-cosmos-db-container-create-request
source_filename: azure-cosmos-db-container-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ContainerCreateRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating or replacing a container.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique name that identifies the container.\"\n    },\n    \"defaultTtl\": {\n      \"type\": \"integer\",\n      \"description\": \"Default time-to-live in seconds.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-container-create-request-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ContainerCreateRequest
---
