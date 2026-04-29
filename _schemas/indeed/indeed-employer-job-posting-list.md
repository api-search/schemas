---
description: A paginated list of job postings.
layout: schema
name: JobPostingList
properties_list:
- description: ''
  name: jobPostings
  type: array
- description: Total number of job postings matching the query.
  name: totalCount
  type: integer
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-job-posting-list-schema.json
slug: indeed-employer-job-posting-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobPostingList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of job postings.\",\n  \"properties\": {\n    \"jobPostings\": {\n      \"type\": \"array\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of job postings matching the query.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-job-posting-list-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: JobPostingList
---
