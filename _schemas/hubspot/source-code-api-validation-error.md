---
description: A validation error
layout: schema
name: ValidationError
properties_list:
- description: Error description
  name: message
  type: string
- description: Line number where the error occurred
  name: line
  type: integer
- description: Column number where the error occurred
  name: column
  type: integer
- description: Error category
  name: category
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/source-code-api-validation-error-schema.json
slug: source-code-api-validation-error
source_filename: source-code-api-validation-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-validation-error-schema.json\",\n  \"title\": \"ValidationError\",\n  \"description\": \"A validation error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error description\",\n      \"example\": \"Syntax error: unexpected end of template\"\n    },\n    \"line\": {\n      \"type\": \"integer\",\n      \"description\": \"Line number where the error occurred\",\n      \"example\": 42\n    },\n    \"column\": {\n      \"type\": \"integer\",\n      \"description\": \"Column number where the error occurred\",\n      \"example\": 15\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Error category\",\n      \"example\": \"HUBL_SYNTAX\"\n    }\n  },\n  \"required\": [\n    \"message\",\n    \"\
  line\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-validation-error-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: ValidationError
---
