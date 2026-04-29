---
description: ''
layout: schema
name: JobPosting
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The title of the job posting.
  name: title
  type: string
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: jobDescription
  type: string
- description: ''
  name: isInternal
  type: boolean
- description: ''
  name: isExternal
  type: boolean
- description: ''
  name: postedOn
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/recruiting-job-posting-schema.json
slug: recruiting-job-posting
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobPosting\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The title of the job posting.\"\n    },\n    \"startDate\": {\n      \"type\": \"string\"\n    },\n    \"endDate\": {\n      \"type\": \"string\"\n    },\n    \"jobDescription\": {\n      \"type\": \"string\"\n    },\n    \"isInternal\": {\n      \"type\": \"boolean\"\n    },\n    \"isExternal\": {\n      \"type\": \"boolean\"\n    },\n    \"postedOn\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/recruiting-job-posting-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: JobPosting
---
