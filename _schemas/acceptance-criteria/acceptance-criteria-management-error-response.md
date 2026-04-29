---
description: Standard error response
layout: schema
name: ErrorResponse
properties_list:
- description: Machine-readable error code
  name: code
  type: string
- description: Human-readable error description
  name: message
  type: string
- description: Additional error context or troubleshooting information
  name: details
  type: string
provider_name: Acceptance Criteria
provider_slug: acceptance-criteria
schema_file: json-schema/acceptance-criteria-management-error-response-schema.json
slug: acceptance-criteria-management-error-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.example.com/schemas/error-response.json\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"description\": \"Standard error response\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error description\"\n    },\n    \"details\": {\n      \"type\": \"string\",\n      \"description\": \"Additional error context or troubleshooting information\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acceptance-criteria/refs/heads/main/json-schema/acceptance-criteria-management-error-response-schema.json
tags:
- Agile
- Behavior Driven Development
- Gherkin
- Quality Assurance
- Requirements
- Testing
- User Stories
title: ErrorResponse
---
