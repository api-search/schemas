---
description: AsyncJobResponse schema from Availity API
layout: schema
name: AsyncJobResponse
properties_list:
- description: Job ID for polling
  name: id
  type: string
- description: ''
  name: status
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/claim-status-async-job-response-schema.json
slug: claim-status-async-job-response
source_filename: claim-status-async-job-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-async-job-response-schema.json\",\n  \"title\": \"AsyncJobResponse\",\n  \"description\": \"AsyncJobResponse schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Job ID for polling\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"PROCESSING\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/claim-status-async-job-response-schema.json
tags: []
title: AsyncJobResponse
---
