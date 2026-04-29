---
description: CohortUploadRequest schema from Amplitude Behavioral Cohorts API
layout: schema
name: CohortUploadRequest
properties_list:
- description: The name of the cohort to create or update.
  name: name
  type: string
- description: Array of user_id or amplitude_id values to include in the cohort.
  name: ids
  type: array
- description: The email address of the cohort owner.
  name: owner
  type: string
- description: If provided, updates the existing cohort with this ID instead of creating a new one.
  name: existing_cohort_id
  type: string
provider_name: Amplitude
provider_slug: amplitude
schema_file: json-schema/behavioral-cohorts-api-cohort-upload-request-schema.json
slug: behavioral-cohorts-api-cohort-upload-request
source_filename: behavioral-cohorts-api-cohort-upload-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/behavioral-cohorts-api-cohort-upload-request-schema.json\",\n  \"title\": \"CohortUploadRequest\",\n  \"description\": \"CohortUploadRequest schema from Amplitude Behavioral Cohorts API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the cohort to create or update.\"\n    },\n    \"ids\": {\n      \"type\": \"array\",\n      \"description\": \"Array of user_id or amplitude_id values to include in the cohort.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"The email address of the cohort owner.\"\n    },\n    \"existing_cohort_id\": {\n      \"type\": \"string\",\n      \"description\": \"If provided, updates the existing cohort with\
  \ this ID instead of creating a new one.\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"ids\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amplitude/refs/heads/main/json-schema/behavioral-cohorts-api-cohort-upload-request-schema.json
tags:
- A/B Testing
- Analytics
- Experimentation
- Feature Flags
- Product Analytics
- User Behavior
title: CohortUploadRequest
---
