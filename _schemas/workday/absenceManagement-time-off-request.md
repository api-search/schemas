---
description: ''
layout: schema
name: TimeOffRequest
properties_list:
- description: The list of days included in the time-off request.
  name: days
  type: array
provider_name: Workday
provider_slug: workday
schema_file: json-schema/absenceManagement-time-off-request-schema.json
slug: absenceManagement-time-off-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TimeOffRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"days\": {\n      \"type\": \"array\",\n      \"description\": \"The list of days included in the time-off request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/absenceManagement-time-off-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: TimeOffRequest
---
