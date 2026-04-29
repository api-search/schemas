---
description: ''
layout: schema
name: Scenario
properties_list:
- description: Unique scenario identifier
  name: id
  type: string
- description: Human-readable scenario name
  name: name
  type: string
- description: Scenario description
  name: description
  type: string
- description: Creation timestamp
  name: createdAt
  type: string
- description: Last modification timestamp
  name: modifiedAt
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-ai-core-scenario-schema.json
slug: sap-ai-core-scenario
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Scenario\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique scenario identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable scenario name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Scenario description\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"Creation timestamp\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"description\": \"Last modification timestamp\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-ai-core-scenario-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: Scenario
---
