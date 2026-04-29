---
description: ''
layout: schema
name: LoginRequest
properties_list:
- description: The name of the company database to connect to
  name: CompanyDB
  type: string
- description: The SAP Business One user name
  name: UserName
  type: string
- description: The user password
  name: Password
  type: string
provider_name: SAP
provider_slug: sap
schema_file: json-schema/sap-business-one-service-layer-login-request-schema.json
slug: sap-business-one-service-layer-login-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoginRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"CompanyDB\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the company database to connect to\"\n    },\n    \"UserName\": {\n      \"type\": \"string\",\n      \"description\": \"The SAP Business One user name\"\n    },\n    \"Password\": {\n      \"type\": \"string\",\n      \"description\": \"The user password\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/sap/refs/heads/main/json-schema/sap-business-one-service-layer-login-request-schema.json
tags:
- AI
- BTP
- Business Applications
- Cloud
- Data Management
- Enterprise
- ERP
- Integration
title: LoginRequest
---
