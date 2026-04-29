---
description: CohortStatusResponse schema from Amplitude Behavioral Cohorts API
layout: schema
name: CohortStatusResponse
properties_list:
- description: The ID of the export request.
  name: request_id
  type: string
- description: The status of the export job.
  name: status
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/behavioral-cohorts-api-cohort-status-response-schema.json
slug: behavioral-cohorts-api-cohort-status-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/behavioral-cohorts-api-cohort-status-response-schema.json\",\n  \"title\": \"CohortStatusResponse\",\n  \"description\": \"CohortStatusResponse schema from Amplitude Behavioral Cohorts API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the export request.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the export job.\",\n      \"enum\": [\n        \"queued\",\n        \"computing\",\n        \"complete\",\n        \"failed\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/behavioral-cohorts-api-cohort-status-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: CohortStatusResponse
---
