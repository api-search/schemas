---
description: Result of file validation
layout: schema
name: ValidationResult
properties_list:
- description: Whether the file passed validation
  name: valid
  type: boolean
- description: List of validation errors (if any)
  name: errors
  type: array
- description: List of validation warnings (if any)
  name: warnings
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/source-code-api-validation-result-schema.json
slug: source-code-api-validation-result
source_filename: source-code-api-validation-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-validation-result-schema.json\",\n  \"title\": \"ValidationResult\",\n  \"description\": \"Result of file validation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"valid\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the file passed validation\",\n      \"example\": true\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of validation errors (if any)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A validation error\",\n        \"required\": [\n          \"message\",\n          \"line\"\n        ],\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Error description\",\n            \"example\": \"Syntax error: unexpected end of\
  \ template\"\n          },\n          \"line\": {\n            \"type\": \"integer\",\n            \"description\": \"Line number where the error occurred\",\n            \"example\": 42\n          },\n          \"column\": {\n            \"type\": \"integer\",\n            \"description\": \"Column number where the error occurred\",\n            \"example\": 15\n          },\n          \"category\": {\n            \"type\": \"string\",\n            \"description\": \"Error category\",\n            \"example\": \"HUBL_SYNTAX\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"message\": \"Syntax error: unexpected end of template\",\n          \"line\": 42,\n          \"column\": 15,\n          \"category\": \"HUBL_SYNTAX\"\n        }\n      ]\n    },\n    \"warnings\": {\n      \"type\": \"array\",\n      \"description\": \"List of validation warnings (if any)\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A validation warning\"\
  ,\n        \"required\": [\n          \"message\"\n        ],\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Warning description\",\n            \"example\": \"Deprecated function 'blog_recent_posts' used\"\n          },\n          \"line\": {\n            \"type\": \"integer\",\n            \"description\": \"Line number where the warning occurred\",\n            \"example\": 28\n          },\n          \"suggestion\": {\n            \"type\": \"string\",\n            \"description\": \"Suggested fix\",\n            \"example\": \"Use 'blog_posts' function instead\"\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"message\": \"Deprecated function 'blog_recent_posts' used\",\n          \"line\": 28,\n          \"suggestion\": \"Use 'blog_posts' function instead\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"valid\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/source-code-api-validation-result-schema.json
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
title: ValidationResult
---
