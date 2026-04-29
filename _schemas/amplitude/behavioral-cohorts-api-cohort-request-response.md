---
description: CohortRequestResponse schema from Amplitude Behavioral Cohorts API
layout: schema
name: CohortRequestResponse
properties_list:
- description: The ID of the export request for polling status.
  name: request_id
  type: string
- description: The ID of the cohort being exported.
  name: cohort_id
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/behavioral-cohorts-api-cohort-request-response-schema.json
slug: behavioral-cohorts-api-cohort-request-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/behavioral-cohorts-api-cohort-request-response-schema.json\",\n  \"title\": \"CohortRequestResponse\",\n  \"description\": \"CohortRequestResponse schema from Amplitude Behavioral Cohorts API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"request_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the export request for polling status.\"\n    },\n    \"cohort_id\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the cohort being exported.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/behavioral-cohorts-api-cohort-request-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: CohortRequestResponse
---
