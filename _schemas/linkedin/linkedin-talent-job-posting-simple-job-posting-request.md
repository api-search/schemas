---
description: Request body for creating or updating job postings
layout: schema
name: SimpleJobPostingRequest
properties_list:
- description: ''
  name: elements
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-simple-job-posting-request-schema.json
slug: linkedin-talent-job-posting-simple-job-posting-request
source_filename: linkedin-talent-job-posting-simple-job-posting-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-simple-job-posting-request-schema.json\",\n  \"title\": \"SimpleJobPostingRequest\",\n  \"description\": \"Request body for creating or updating job postings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/JobPostingElement\"\n      }\n    }\n  },\n  \"required\": [\n    \"elements\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-simple-job-posting-request-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: SimpleJobPostingRequest
---
