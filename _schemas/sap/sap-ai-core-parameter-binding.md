---
description: ''
layout: schema
name: ParameterBinding
properties_list:
- description: Parameter name
  name: key
  type: string
- description: Parameter value
  name: value
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-ai-core-parameter-binding-schema.json
slug: sap-ai-core-parameter-binding
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParameterBinding\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter name\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"Parameter value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-ai-core-parameter-binding-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: ParameterBinding
---
