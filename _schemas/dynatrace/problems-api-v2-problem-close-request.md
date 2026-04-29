---
description: Request body for closing a problem.
layout: schema
name: ProblemCloseRequest
properties_list:
- description: An optional message explaining why the problem is being closed. This is stored as a closing comment on the problem.
  name: message
  type: string
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/problems-api-v2-problem-close-request-schema.json
slug: problems-api-v2-problem-close-request
source_filename: problems-api-v2-problem-close-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-api-v2-problem-close-request-schema.json\",\n  \"title\": \"ProblemCloseRequest\",\n  \"description\": \"Request body for closing a problem.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"An optional message explaining why the problem is being closed. This is stored as a closing comment on the problem.\",\n      \"example\": \"Example description.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-api-v2-problem-close-request-schema.json
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
title: ProblemCloseRequest
---
