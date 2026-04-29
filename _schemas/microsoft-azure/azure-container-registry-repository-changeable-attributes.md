---
description: Changeable attributes for a repository.
layout: schema
name: RepositoryChangeableAttributes
properties_list:
- description: Whether delete is enabled.
  name: deleteEnabled
  type: boolean
- description: Whether write is enabled.
  name: writeEnabled
  type: boolean
- description: Whether list is enabled.
  name: listEnabled
  type: boolean
- description: Whether read is enabled.
  name: readEnabled
  type: boolean
- description: Whether teleport is enabled.
  name: teleportEnabled
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-repository-changeable-attributes-schema.json
slug: azure-container-registry-repository-changeable-attributes
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RepositoryChangeableAttributes\",\n  \"type\": \"object\",\n  \"description\": \"Changeable attributes for a repository.\",\n  \"properties\": {\n    \"deleteEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether delete is enabled.\"\n    },\n    \"writeEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether write is enabled.\"\n    },\n    \"listEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether list is enabled.\"\n    },\n    \"readEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether read is enabled.\"\n    },\n    \"teleportEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether teleport is enabled.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-repository-changeable-attributes-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: RepositoryChangeableAttributes
---
