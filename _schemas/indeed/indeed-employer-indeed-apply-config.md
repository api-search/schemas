---
description: Configuration for Indeed Apply integration on the job posting.
layout: schema
name: IndeedApplyConfig
properties_list:
- description: Whether Indeed Apply is enabled for this job posting.
  name: enabled
  type: boolean
- description: The URL where Indeed sends application data when a candidate applies through Indeed Apply.
  name: postUrl
  type: string
- description: Screener questions to present to candidates during application.
  name: screenerQuestions
  type: array
- description: Whether EEO compliance questions are enabled. Available for US employers only.
  name: eeoEnabled
  type: boolean
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-indeed-apply-config-schema.json
slug: indeed-employer-indeed-apply-config
source_filename: indeed-employer-indeed-apply-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"IndeedApplyConfig\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for Indeed Apply integration on the job posting.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether Indeed Apply is enabled for this job posting.\"\n    },\n    \"postUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL where Indeed sends application data when a candidate applies through Indeed Apply.\"\n    },\n    \"screenerQuestions\": {\n      \"type\": \"array\",\n      \"description\": \"Screener questions to present to candidates during application.\"\n    },\n    \"eeoEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether EEO compliance questions are enabled. Available for US employers only.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-indeed-apply-config-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: IndeedApplyConfig
---
