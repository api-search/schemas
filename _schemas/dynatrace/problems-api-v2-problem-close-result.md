---
description: The result returned after closing a problem.
layout: schema
name: ProblemCloseResult
properties_list:
- description: The ID of the closed problem.
  name: problemId
  type: string
- description: Whether the problem is in the process of closing. The problem may take a short time to fully transition to RESOLVED status.
  name: closing
  type: boolean
provider_name: Dynatrace
provider_slug: dynatrace
schema_file: json-schema/problems-api-v2-problem-close-result-schema.json
slug: problems-api-v2-problem-close-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-api-v2-problem-close-result-schema.json\",\n  \"title\": \"ProblemCloseResult\",\n  \"description\": \"The result returned after closing a problem.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"problemId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the closed problem.\",\n      \"example\": \"abc123\"\n    },\n    \"closing\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the problem is in the process of closing. The problem may take a short time to fully transition to RESOLVED status.\",\n      \"example\": true\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/problems-api-v2-problem-close-result-schema.json
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
title: ProblemCloseResult
---
