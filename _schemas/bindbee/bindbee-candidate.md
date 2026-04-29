---
description: A job candidate from a connected ATS system.
layout: schema
name: Candidate
properties_list:
- description: Candidate ID.
  name: id
  type: string
- description: Candidate first name.
  name: first_name
  type: string
- description: Candidate last name.
  name: last_name
  type: string
- description: Candidate email.
  name: email
  type: string
- description: Job ID the candidate applied for.
  name: job_id
  type: string
- description: Current hiring stage.
  name: stage
  type: string
- description: Application creation timestamp.
  name: created_at
  type: string
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-candidate-schema.json
slug: bindbee-candidate
source_filename: bindbee-candidate-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"Candidate\",\n  \"type\": \"object\",\n  \"description\": \"A job candidate from a connected ATS system.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Candidate ID.\",\n      \"example\": \"cand-abc123\"\n    },\n    \"first_name\": {\n      \"type\": \"string\",\n      \"description\": \"Candidate first name.\",\n      \"example\": \"John\"\n    },\n    \"last_name\": {\n      \"type\": \"string\",\n      \"description\": \"Candidate last name.\",\n      \"example\": \"Doe\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"description\": \"Candidate email.\",\n      \"example\": \"jdoe@example.com\"\n    },\n    \"job_id\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID the candidate applied for.\",\n      \"example\": \"job-abc123\"\n    },\n    \"stage\": {\n      \"type\": \"string\",\n      \"description\": \"Current\
  \ hiring stage.\",\n      \"enum\": [\n        \"applied\",\n        \"screening\",\n        \"interview\",\n        \"offer\",\n        \"hired\",\n        \"rejected\"\n      ],\n      \"example\": \"interview\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Application creation timestamp.\",\n      \"example\": \"2024-04-13T00:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-candidate-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: Candidate
---
