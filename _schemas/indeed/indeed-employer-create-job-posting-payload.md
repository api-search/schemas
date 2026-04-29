---
description: Response payload from a job posting creation operation.
layout: schema
name: CreateJobPostingPayload
properties_list:
- description: ''
  name: results
  type: array
- description: Total number of job postings successfully created.
  name: totalCreated
  type: integer
- description: Total number of job postings that failed to create.
  name: totalFailed
  type: integer
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-create-job-posting-payload-schema.json
slug: indeed-employer-create-job-posting-payload
source_filename: indeed-employer-create-job-posting-payload-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateJobPostingPayload\",\n  \"type\": \"object\",\n  \"description\": \"Response payload from a job posting creation operation.\",\n  \"properties\": {\n    \"results\": {\n      \"type\": \"array\"\n    },\n    \"totalCreated\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of job postings successfully created.\"\n    },\n    \"totalFailed\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of job postings that failed to create.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-create-job-posting-payload-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: CreateJobPostingPayload
---
