---
description: ''
layout: schema
name: Deployment
properties_list:
- description: Deployment identifier
  name: id
  type: string
- description: Configuration used for this deployment
  name: configurationId
  type: string
- description: Associated scenario
  name: scenarioId
  type: string
- description: Current deployment status
  name: status
  type: string
- description: URL for sending inference requests
  name: deploymentUrl
  type: string
- description: ''
  name: createdAt
  type: string
- description: ''
  name: modifiedAt
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-ai-core-deployment-schema.json
slug: sap-ai-core-deployment
source_filename: sap-ai-core-deployment-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Deployment\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Deployment identifier\"\n    },\n    \"configurationId\": {\n      \"type\": \"string\",\n      \"description\": \"Configuration used for this deployment\"\n    },\n    \"scenarioId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated scenario\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current deployment status\"\n    },\n    \"deploymentUrl\": {\n      \"type\": \"string\",\n      \"description\": \"URL for sending inference requests\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-ai-core-deployment-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: Deployment
---
