---
description: Input for creating one or more job postings on Indeed via the Job Sync API.
layout: schema
name: CreateJobPostingInput
properties_list:
- description: Array of job posting objects to create.
  name: jobPostings
  type: array
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-create-job-posting-input-schema.json
slug: indeed-employer-create-job-posting-input
source_filename: indeed-employer-create-job-posting-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateJobPostingInput\",\n  \"type\": \"object\",\n  \"description\": \"Input for creating one or more job postings on Indeed via the Job Sync API.\",\n  \"properties\": {\n    \"jobPostings\": {\n      \"type\": \"array\",\n      \"description\": \"Array of job posting objects to create.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-create-job-posting-input-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: CreateJobPostingInput
---
