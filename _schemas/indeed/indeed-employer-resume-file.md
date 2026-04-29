---
description: An uploaded resume file.
layout: schema
name: ResumeFile
properties_list:
- description: The original filename of the uploaded resume.
  name: fileName
  type: string
- description: The MIME type of the resume file.
  name: contentType
  type: string
- description: The raw binary content of the resume file, Base64-encoded.
  name: data
  type: string
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-resume-file-schema.json
slug: indeed-employer-resume-file
source_filename: indeed-employer-resume-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResumeFile\",\n  \"type\": \"object\",\n  \"description\": \"An uploaded resume file.\",\n  \"properties\": {\n    \"fileName\": {\n      \"type\": \"string\",\n      \"description\": \"The original filename of the uploaded resume.\"\n    },\n    \"contentType\": {\n      \"type\": \"string\",\n      \"description\": \"The MIME type of the resume file.\"\n    },\n    \"data\": {\n      \"type\": \"string\",\n      \"description\": \"The raw binary content of the resume file, Base64-encoded.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-resume-file-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: ResumeFile
---
