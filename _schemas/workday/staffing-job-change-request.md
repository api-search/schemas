---
description: ''
layout: schema
name: JobChangeRequest
properties_list:
- description: The effective date of the job change.
  name: effectiveDate
  type: string
- description: ''
  name: proposedBusinessTitle
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/staffing-job-change-request-schema.json
slug: staffing-job-change-request
source_filename: staffing-job-change-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"JobChangeRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"description\": \"The effective date of the job change.\"\n    },\n    \"proposedBusinessTitle\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/staffing-job-change-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: JobChangeRequest
---
