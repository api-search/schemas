---
description: Response from job posting creation
layout: schema
name: JobPostingResponse
properties_list:
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-job-posting-response-schema.json
slug: linkedin-talent-job-posting-job-posting-response
source_filename: linkedin-talent-job-posting-job-posting-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-job-posting-response-schema.json\",\n  \"title\": \"JobPostingResponse\",\n  \"description\": \"Response from job posting creation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobPostingResult\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-job-posting-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: JobPostingResponse
---
