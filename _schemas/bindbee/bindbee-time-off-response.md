---
description: List of time-off requests.
layout: schema
name: TimeOffResponse
properties_list:
- description: Array of time-off requests.
  name: data
  type: array
provider_name: Bindbee
provider_slug: bindbee
schema_file: json-schema/bindbee-time-off-response-schema.json
slug: bindbee-time-off-response
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"title\": \"TimeOffResponse\",\n  \"type\": \"object\",\n  \"description\": \"List of time-off requests.\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"Array of time-off requests.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TimeOffRequest\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/json-schema/bindbee-time-off-response-schema.json
tags:
- ATS
- HR Integration
- HRIS
- Workforce
title: TimeOffResponse
---
