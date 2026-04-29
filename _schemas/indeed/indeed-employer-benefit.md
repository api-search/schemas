---
description: A benefit offered with the job position.
layout: schema
name: Benefit
properties_list:
- description: The type of benefit.
  name: type
  type: string
- description: Additional details about the benefit.
  name: description
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-benefit-schema.json
slug: indeed-employer-benefit
source_filename: indeed-employer-benefit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Benefit\",\n  \"type\": \"object\",\n  \"description\": \"A benefit offered with the job position.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of benefit.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details about the benefit.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-benefit-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: Benefit
---
