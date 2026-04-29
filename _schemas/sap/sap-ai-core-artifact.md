---
description: ''
layout: schema
name: Artifact
properties_list:
- description: Artifact identifier
  name: id
  type: string
- description: Artifact name
  name: name
  type: string
- description: Artifact kind
  name: kind
  type: string
- description: Storage URL for the artifact
  name: url
  type: string
- description: Associated scenario
  name: scenarioId
  type: string
- description: Execution that produced this artifact
  name: executionId
  type: string
- description: Artifact description
  name: description
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-ai-core-artifact-schema.json
slug: sap-ai-core-artifact
source_filename: sap-ai-core-artifact-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Artifact\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Artifact identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Artifact name\"\n    },\n    \"kind\": {\n      \"type\": \"string\",\n      \"description\": \"Artifact kind\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Storage URL for the artifact\"\n    },\n    \"scenarioId\": {\n      \"type\": \"string\",\n      \"description\": \"Associated scenario\"\n    },\n    \"executionId\": {\n      \"type\": \"string\",\n      \"description\": \"Execution that produced this artifact\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Artifact description\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-ai-core-artifact-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: Artifact
---
