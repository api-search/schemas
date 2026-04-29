---
description: Details of an API error.
layout: schema
name: Error
properties_list:
- description: The HTTP status code of the error.
  name: code
  type: integer
- description: A human-readable description of the error.
  name: message
  type: string
- description: A list of constraint violations for validation errors (HTTP 400).
  name: constraintViolations
  type: array
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-entities-v2-error-schema.json
slug: dynatrace-entities-v2-error
source_filename: dynatrace-entities-v2-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Details of an API error.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code of the error.\",\n      \"example\": 500\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error.\",\n      \"example\": \"Example description.\"\n    },\n    \"constraintViolations\": {\n      \"type\": \"array\",\n      \"description\": \"A list of constraint violations for validation errors (HTTP 400).\",\n      \"example\": [\n        {\n          \"path\": \"example-value\",\n          \"message\": \"Example description.\",\n          \"parameterLocation\": \"example-value\",\n          \"location\": \"example-value\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Details of a single constraint violation in a request.\",\n        \"properties\": {\n          \"\
  path\": {\n            \"type\": \"string\",\n            \"description\": \"The JSON path to the field that caused the violation.\",\n            \"example\": \"example-value\"\n          },\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"A description of the constraint violation.\",\n            \"example\": \"Example description.\"\n          },\n          \"parameterLocation\": {\n            \"type\": \"string\",\n            \"description\": \"The location of the violating parameter (QUERY, PATH, BODY).\",\n            \"example\": \"example-value\"\n          },\n          \"location\": {\n            \"type\": \"string\",\n            \"description\": \"The location detail for the violation.\",\n            \"example\": \"example-value\"\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-entities-v2-error-schema.json
tags:
- AI Operations
- Analytics
- APM
- Application Performance Monitoring
- Application Security
- Automation
- Cloud Monitoring
- Digital Experience Management
- Intelligence
- Observability
title: Error
---
