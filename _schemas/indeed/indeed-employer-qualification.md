---
description: A qualification required or preferred for the job position, such as education level, years of experience, certifications, or skills.
layout: schema
name: Qualification
properties_list:
- description: The category of the qualification.
  name: type
  type: string
- description: Description of the qualification.
  name: description
  type: string
- description: Whether this qualification is required or preferred.
  name: required
  type: boolean
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-qualification-schema.json
slug: indeed-employer-qualification
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Qualification\",\n  \"type\": \"object\",\n  \"description\": \"A qualification required or preferred for the job position, such as education level, years of experience, certifications, or skills.\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the qualification.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the qualification.\"\n    },\n    \"required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this qualification is required or preferred.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-qualification-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: Qualification
---
