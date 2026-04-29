---
description: ''
layout: schema
name: WorkerSummary
properties_list:
- description: The Workday ID of the worker.
  name: id
  type: string
- description: A display descriptor for the worker (typically full name).
  name: descriptor
  type: string
- description: A link to the full worker resource.
  name: href
  type: string
- description: The primary work email address.
  name: primaryWorkEmail
  type: string
- description: The primary work phone number.
  name: primaryWorkPhone
  type: string
- description: Whether this is the primary job for the worker.
  name: isPrimaryJob
  type: boolean
- description: The business title for the worker.
  name: businessTitle
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/hcm-worker-summary-schema.json
slug: hcm-worker-summary
source_filename: hcm-worker-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WorkerSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the worker.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\",\n      \"description\": \"A display descriptor for the worker (typically full name).\"\n    },\n    \"href\": {\n      \"type\": \"string\",\n      \"description\": \"A link to the full worker resource.\"\n    },\n    \"primaryWorkEmail\": {\n      \"type\": \"string\",\n      \"description\": \"The primary work email address.\"\n    },\n    \"primaryWorkPhone\": {\n      \"type\": \"string\",\n      \"description\": \"The primary work phone number.\"\n    },\n    \"isPrimaryJob\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the primary job for the worker.\"\n    },\n    \"businessTitle\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The business title for the worker.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/hcm-worker-summary-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: WorkerSummary
---
