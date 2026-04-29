---
description: A candidate's resume in multiple formats. The file field contains the uploaded resume document, while text, html, and json fields provide parsed representations.
layout: schema
name: Resume
properties_list:
- description: Plain text representation of the resume content.
  name: text
  type: string
- description: HTML-formatted representation of the resume content.
  name: html
  type: string
- description: Structured JSON representation of the parsed resume, including sections for work experience, education, skills, and other fields.
  name: json
  type: object
provider_name: Indeed
provider_slug: indeed
schema_file: json-schema/indeed-employer-resume-schema.json
slug: indeed-employer-resume
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resume\",\n  \"type\": \"object\",\n  \"description\": \"A candidate's resume in multiple formats. The file field contains the uploaded resume document, while text, html, and json fields provide parsed representations.\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Plain text representation of the resume content.\"\n    },\n    \"html\": {\n      \"type\": \"string\",\n      \"description\": \"HTML-formatted representation of the resume content.\"\n    },\n    \"json\": {\n      \"type\": \"object\",\n      \"description\": \"Structured JSON representation of the parsed resume, including sections for work experience, education, skills, and other fields.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/indeed/refs/heads/main/json-schema/indeed-employer-resume-schema.json
tags:
- Careers
- Employment
- Hiring
- Job Search
- Jobs
- Recruiting
title: Resume
---
