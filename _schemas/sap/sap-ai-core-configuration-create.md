---
description: ''
layout: schema
name: ConfigurationCreate
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: scenarioId
  type: string
- description: ''
  name: executableId
  type: string
- description: ''
  name: parameterBindings
  type: array
- description: ''
  name: inputArtifactBindings
  type: array
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-ai-core-configuration-create-schema.json
slug: sap-ai-core-configuration-create
source_filename: sap-ai-core-configuration-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConfigurationCreate\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"scenarioId\": {\n      \"type\": \"string\"\n    },\n    \"executableId\": {\n      \"type\": \"string\"\n    },\n    \"parameterBindings\": {\n      \"type\": \"array\"\n    },\n    \"inputArtifactBindings\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-ai-core-configuration-create-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: ConfigurationCreate
---
