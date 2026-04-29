---
description: ''
layout: schema
name: Configuration
properties_list:
- description: Configuration identifier
  name: id
  type: string
- description: Configuration name
  name: name
  type: string
- description: Associated scenario ID
  name: scenarioId
  type: string
- description: Associated executable ID
  name: executableId
  type: string
- description: ''
  name: parameterBindings
  type: array
- description: ''
  name: inputArtifactBindings
  type: array
- description: ''
  name: createdAt
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-ai-core-configuration-schema.json
slug: sap-ai-core-configuration
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Configuration\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration name\"\n    },\n    \"scenarioId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated scenario ID\"\n    },\n    \"executableId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated executable ID\"\n    },\n    \"parameterBindings\": {\n      \"type\": \"array\"\n    },\n    \"inputArtifactBindings\": {\n      \"type\": \"array\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-ai-core-configuration-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: Configuration
---
