---
description: List of jobs
layout: schema
name: JobList
properties_list:
- description: ''
  name: jobs
  type: array
provider_name: Academy Software Foundation
provider_slug: academy-software-foundation
schema_file: json-schema/opencue-job-list-schema.json
slug: opencue-job-list
source_filename: opencue-job-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-job-list-schema.json\",\n  \"title\": \"JobList\",\n  \"description\": \"List of jobs\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobs\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Job\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/academy-software-foundation/refs/heads/main/json-schema/opencue-job-list-schema.json
tags:
- Animation
- Color Management
- Film
- Linux Foundation
- Open Source
- Rendering
- Standards
- Visual Effects
- VFX
title: JobList
---
