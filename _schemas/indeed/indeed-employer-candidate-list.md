---
description: A paginated list of candidates.
layout: schema
name: CandidateList
properties_list:
- description: ''
  name: candidates
  type: array
- description: Total number of candidates matching the query.
  name: totalCount
  type: integer
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-candidate-list-schema.json
slug: indeed-employer-candidate-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CandidateList\",\n  \"type\": \"object\",\n  \"description\": \"A paginated list of candidates.\",\n  \"properties\": {\n    \"candidates\": {\n      \"type\": \"array\"\n    },\n    \"totalCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of candidates matching the query.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-candidate-list-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: CandidateList
---
