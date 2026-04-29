---
description: CohortListResponse schema from Amplitude Behavioral Cohorts API
layout: schema
name: CohortListResponse
properties_list:
- description: Array of cohort metadata objects.
  name: cohorts
  type: array
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/behavioral-cohorts-api-cohort-list-response-schema.json
slug: behavioral-cohorts-api-cohort-list-response
source_filename: behavioral-cohorts-api-cohort-list-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/behavioral-cohorts-api-cohort-list-response-schema.json\",\n  \"title\": \"CohortListResponse\",\n  \"description\": \"CohortListResponse schema from Amplitude Behavioral Cohorts API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cohorts\": {\n      \"type\": \"array\",\n      \"description\": \"Array of cohort metadata objects.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"The unique identifier for the cohort.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the cohort.\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"description\": \"A description of the cohort.\"\
  \n          },\n          \"size\": {\n            \"type\": \"integer\",\n            \"description\": \"The number of users in the cohort.\"\n          },\n          \"lastComputed\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"The date and time the cohort was last computed.\"\n          },\n          \"archived\": {\n            \"type\": \"boolean\",\n            \"description\": \"Whether the cohort is archived.\"\n          },\n          \"owner\": {\n            \"type\": \"string\",\n            \"description\": \"The email of the cohort owner.\"\n          },\n          \"appId\": {\n            \"type\": \"integer\",\n            \"description\": \"The Amplitude project ID the cohort belongs to.\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/behavioral-cohorts-api-cohort-list-response-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: CohortListResponse
---
