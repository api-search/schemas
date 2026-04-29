---
description: ''
layout: schema
name: Metrics
properties_list:
- description: ''
  name: activeUsers
  type: array
- description: ''
  name: totalExecutions
  type: array
- description: ''
  name: failedExecutions
  type: array
provider_name: Google Apps Script
provider_slug: google-apps-script
schema_file: json-schema/openapi-metrics-schema.json
slug: openapi-metrics
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Metrics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"activeUsers\": {\n      \"type\": \"array\"\n    },\n    \"totalExecutions\": {\n      \"type\": \"array\"\n    },\n    \"failedExecutions\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-apps-script/refs/heads/main/json-schema/openapi-metrics-schema.json
tags:
- Apps Script
- Automation
- Deployments
- Google
- Google Workspace
- Scripting
title: Metrics
---
