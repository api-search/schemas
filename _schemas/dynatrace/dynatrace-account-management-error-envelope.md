---
description: Error response envelope returned when a request fails.
layout: schema
name: ErrorEnvelope
properties_list:
- description: Details of an API error.
  name: error
  type: object
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/dynatrace-account-management-error-envelope-schema.json
slug: dynatrace-account-management-error-envelope
source_filename: dynatrace-account-management-error-envelope-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Error response envelope returned when a request fails.\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"object\",\n      \"description\": \"Details of an API error.\",\n      \"properties\": {\n        \"code\": {\n          \"type\": \"integer\",\n          \"description\": \"The HTTP status code of the error.\",\n          \"example\": 500\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable description of the error.\",\n          \"example\": \"Example description.\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorEnvelope\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-account-management-error-envelope-schema.json
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
title: ErrorEnvelope
---
