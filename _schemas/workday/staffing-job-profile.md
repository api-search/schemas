---
description: ''
layout: schema
name: JobProfile
properties_list:
- description: The Workday ID of the job profile.
  name: id
  type: string
- description: A display descriptor for the job profile.
  name: descriptor
  type: string
- description: The name of the job profile.
  name: jobProfileName
  type: string
- description: ''
  name: isInactive
  type: boolean
- description: The job code identifier.
  name: jobCode
  type: string
- description: Summary description of the job profile.
  name: summary
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/staffing-job-profile-schema.json
slug: staffing-job-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobProfile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the job profile.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the job profile.\"\n    },\n    \"jobProfileName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the job profile.\"\n    },\n    \"isInactive\": {\n      \"type\": \"boolean\"\n    },\n    \"jobCode\": {\n      \"type\": \"string\",\n      \"description\": \"The job code identifier.\"\n    },\n    \"summary\": {\n      \"type\": \"string\",\n      \"description\": \"Summary description of the job profile.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/staffing-job-profile-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: JobProfile
---
