---
description: Information about the source system for the job posting, used to identify the originating ATS or job board.
layout: schema
name: JobSource
properties_list:
- description: The name of the source system. Must remain consistent across all job postings from the same source.
  name: sourceName
  type: string
- description: The URL of the original job posting on the source system.
  name: sourceUrl
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-job-source-schema.json
slug: indeed-employer-job-source
source_filename: indeed-employer-job-source-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobSource\",\n  \"type\": \"object\",\n  \"description\": \"Information about the source system for the job posting, used to identify the originating ATS or job board.\",\n  \"properties\": {\n    \"sourceName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the source system. Must remain consistent across all job postings from the same source.\"\n    },\n    \"sourceUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL of the original job posting on the source system.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-job-source-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: JobSource
---
