---
description: ''
layout: schema
name: Execution
properties_list:
- description: Execution identifier
  name: id
  type: string
- description: Configuration used for this execution
  name: configurationId
  type: string
- description: Associated scenario
  name: scenarioId
  type: string
- description: Current execution status
  name: status
  type: string
- description: Human-readable status message
  name: statusMessage
  type: string
- description: ''
  name: outputArtifacts
  type: array
- description: ''
  name: createdAt
  type: string
- description: ''
  name: modifiedAt
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-ai-core-execution-schema.json
slug: sap-ai-core-execution
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Execution\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Execution identifier\"\n    },\n    \"configurationId\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration used for this execution\"\n    },\n    \"scenarioId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated scenario\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current execution status\"\n    },\n    \"statusMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable status message\"\n    },\n    \"outputArtifacts\": {\n      \"type\": \"array\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-ai-core-execution-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: Execution
---
