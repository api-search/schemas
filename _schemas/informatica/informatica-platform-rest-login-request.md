---
description: Request body for the login endpoint.
layout: schema
name: LoginRequest
properties_list:
- description: The resource type identifier. Must be set to "login".
  name: '@type'
  type: string
- description: The Informatica Intelligent Cloud Services username.
  name: username
  type: string
- description: The account password.
  name: password
  type: string
provider_name: Informatica
provider_slug: informatica
schema_file: json-schema/informatica-platform-rest-login-request-schema.json
slug: informatica-platform-rest-login-request
source_filename: informatica-platform-rest-login-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LoginRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for the login endpoint.\",\n  \"properties\": {\n    \"@type\": {\n      \"type\": \"string\",\n      \"description\": \"The resource type identifier. Must be set to \\\"login\\\".\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The Informatica Intelligent Cloud Services username.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"The account password.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/informatica/refs/heads/main/json-schema/informatica-platform-rest-login-request-schema.json
tags:
- Address Verification
- B2B Gateway
- Cloud Services
- Data Governance
- Data Integration
- Data Profiling
- Data Quality
- Enterprise Software
- ETL
- IDMC
- IICS
- Master Data Management
- Reference Data Management
title: LoginRequest
---
