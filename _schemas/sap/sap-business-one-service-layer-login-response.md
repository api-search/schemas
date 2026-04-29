---
description: ''
layout: schema
name: LoginResponse
properties_list:
- description: The session identifier for subsequent requests
  name: SessionId
  type: string
- description: The Service Layer version
  name: Version
  type: string
- description: Session timeout in minutes
  name: SessionTimeout
  type: integer
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-login-response-schema.json
slug: sap-business-one-service-layer-login-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoginResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SessionId\": {\n      \"type\": \"string\",\n      \"description\": \"The session identifier for subsequent requests\"\n    },\n    \"Version\": {\n      \"type\": \"string\",\n      \"description\": \"The Service Layer version\"\n    },\n    \"SessionTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Session timeout in minutes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-login-response-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: LoginResponse
---
