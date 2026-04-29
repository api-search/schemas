---
description: ''
layout: schema
name: TerminationRequest
properties_list:
- description: ''
  name: terminationDate
  type: string
- description: ''
  name: lastDayOfWork
  type: string
- description: ''
  name: regrettable
  type: boolean
- description: ''
  name: notifyEmployee
  type: boolean
provider_name: Workday
provider_slug: workday
schema_file: json-schema/staffing-termination-request-schema.json
slug: staffing-termination-request
source_filename: staffing-termination-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TerminationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"terminationDate\": {\n      \"type\": \"string\"\n    },\n    \"lastDayOfWork\": {\n      \"type\": \"string\"\n    },\n    \"regrettable\": {\n      \"type\": \"boolean\"\n    },\n    \"notifyEmployee\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/staffing-termination-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TerminationRequest
---
