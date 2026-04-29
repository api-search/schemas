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
schema_file: json-schema/dynatrace-problems-v2-problem-close-result-schema.json
slug: dynatrace-problems-v2-problem-close-result
source_filename: dynatrace-problems-v2-problem-close-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"The result returned after closing a problem.\",\n  \"properties\": {\n    \"problemId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the closed problem.\",\n      \"example\": \"abc123\"\n    },\n    \"closing\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the problem is in the process of closing. The problem may take a short time to fully transition to RESOLVED status.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProblemCloseResult\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dynatrace/refs/heads/main/json-schema/dynatrace-problems-v2-problem-close-result-schema.json
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
