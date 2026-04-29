---
description: The indexing policy for a container.
layout: schema
name: IndexingPolicy
properties_list:
- description: Whether indexing is automatic.
  name: automatic
  type: boolean
- description: The indexing mode.
  name: indexingMode
  type: string
- description: Paths to include in indexing.
  name: includedPaths
  type: array
- description: Paths to exclude from indexing.
  name: excludedPaths
  type: array
- description: Composite indexes for the container.
  name: compositeIndexes
  type: array
- description: Spatial indexes for the container.
  name: spatialIndexes
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-cosmos-db-indexing-policy-schema.json
slug: azure-cosmos-db-indexing-policy
source_filename: azure-cosmos-db-indexing-policy-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IndexingPolicy\",\n  \"type\": \"object\",\n  \"description\": \"The indexing policy for a container.\",\n  \"properties\": {\n    \"automatic\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether indexing is automatic.\"\n    },\n    \"indexingMode\": {\n      \"type\": \"string\",\n      \"description\": \"The indexing mode.\"\n    },\n    \"includedPaths\": {\n      \"type\": \"array\",\n      \"description\": \"Paths to include in indexing.\"\n    },\n    \"excludedPaths\": {\n      \"type\": \"array\",\n      \"description\": \"Paths to exclude from indexing.\"\n    },\n    \"compositeIndexes\": {\n      \"type\": \"array\",\n      \"description\": \"Composite indexes for the container.\"\n    },\n    \"spatialIndexes\": {\n      \"type\": \"array\",\n      \"description\": \"Spatial indexes for the container.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-cosmos-db-indexing-policy-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: IndexingPolicy
---
