---
description: Error details returned by the API.
layout: schema
name: ErrorCollection
properties_list:
- description: The list of error messages.
  name: errorMessages
  type: array
- description: Field-specific errors.
  name: errors
  type: object
- description: The HTTP status code.
  name: status
  type: integer
provider_name: Jira
provider_slug: jira
schema_file: json-schema/jira-cloud-platform-rest-error-collection-schema.json
slug: jira-cloud-platform-rest-error-collection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorCollection\",\n  \"type\": \"object\",\n  \"description\": \"Error details returned by the API.\",\n  \"properties\": {\n    \"errorMessages\": {\n      \"type\": \"array\",\n      \"description\": \"The list of error messages.\"\n    },\n    \"errors\": {\n      \"type\": \"object\",\n      \"description\": \"Field-specific errors.\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"description\": \"The HTTP status code.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jira/refs/heads/main/json-schema/jira-cloud-platform-rest-error-collection-schema.json
tags:
- Agile
- Issue Tracking
- ITSM
- Project Management
- Service Management
title: ErrorCollection
---
