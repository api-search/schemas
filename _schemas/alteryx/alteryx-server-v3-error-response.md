---
description: Standard error response
layout: schema
name: ErrorResponse
properties_list:
- description: Human-readable error message
  name: message
  type: string
- description: Detailed error information
  name: errors
  type: array
provider_name: Alteryx
provider_slug: alteryx
schema_file: json-schema/alteryx-server-v3-error-response-schema.json
slug: alteryx-server-v3-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed error information\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/alteryx/refs/heads/main/json-schema/alteryx-server-v3-error-response-schema.json
tags:
- Analytics
- Automation
- Data Engineering
- Data Preparation
- Data Science
- ETL
- Machine Learning
- Predictive Analytics
title: ErrorResponse
---
