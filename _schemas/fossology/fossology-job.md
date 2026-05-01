---
description: A FOSSology scanning or report job.
layout: schema
name: FOSSologyJob
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: queueDate
  type: string
- description: ''
  name: uploadId
  type: integer
- description: ''
  name: userId
  type: integer
- description: ''
  name: groupId
  type: integer
- description: Estimated remaining seconds.
  name: eta
  type: integer
- description: ''
  name: status
  type: string
provider_name: FOSSology
provider_slug: fossology
schema_file: json-schema/fossology-job.json
slug: fossology-job
source_filename: fossology-job.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/json-schema/fossology-job.json\",\n  \"title\": \"FOSSologyJob\",\n  \"description\": \"A FOSSology scanning or report job.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": { \"type\": \"integer\" },\n    \"name\": { \"type\": \"string\" },\n    \"queueDate\": { \"type\": \"string\", \"format\": \"date-time\" },\n    \"uploadId\": { \"type\": \"integer\" },\n    \"userId\": { \"type\": \"integer\" },\n    \"groupId\": { \"type\": \"integer\" },\n    \"eta\": { \"type\": \"integer\", \"description\": \"Estimated remaining seconds.\" },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"Completed\", \"Processing\", \"Queued\", \"Failed\"]\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/fossology/refs/heads/main/json-schema/fossology-job.json
tags:
- Compliance
- Licensing
- Linux Foundation
- Scanning
- SPDX
- Open Source
title: FOSSologyJob
---
