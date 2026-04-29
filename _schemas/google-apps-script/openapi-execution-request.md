---
description: ''
layout: schema
name: ExecutionRequest
properties_list:
- description: ''
  name: function
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: sessionState
  type: string
- description: ''
  name: devMode
  type: boolean
provider_name: Google Apps Script
provider_slug: google-apps-script
schema_file: json-schema/openapi-execution-request-schema.json
slug: openapi-execution-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ExecutionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"function\": {\n      \"type\": \"string\"\n    },\n    \"parameters\": {\n      \"type\": \"array\"\n    },\n    \"sessionState\": {\n      \"type\": \"string\"\n    },\n    \"devMode\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-apps-script/refs/heads/main/json-schema/openapi-execution-request-schema.json
tags:
- Apps Script
- Automation
- Deployments
- Google
- Google Workspace
- Scripting
title: ExecutionRequest
---
