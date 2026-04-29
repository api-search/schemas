---
description: An HTTP header to include in webhook notification requests.
layout: schema
name: WebhookHeader
properties_list:
- description: The HTTP header name.
  name: name
  type: string
- description: The HTTP header value.
  name: value
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/problems-webhook-header-schema.json
slug: problems-webhook-header
source_filename: problems-webhook-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-webhook-header-schema.json\",\n  \"title\": \"WebhookHeader\",\n  \"description\": \"An HTTP header to include in webhook notification requests.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP header name.\",\n      \"example\": \"Authorization\"\n    },\n    \"value\": {\n      \"type\": \"string\",\n      \"description\": \"The HTTP header value.\",\n      \"example\": \"Bearer my-secret-token\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"value\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-webhook-header-schema.json
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
title: WebhookHeader
---
