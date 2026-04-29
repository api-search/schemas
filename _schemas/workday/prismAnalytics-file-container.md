---
description: ''
layout: schema
name: FileContainer
properties_list:
- description: The Workday ID of the file container.
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: ''
  name: expirationTime
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/prismAnalytics-file-container-schema.json
slug: prismAnalytics-file-container
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FileContainer\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The Workday ID of the file container.\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"expirationTime\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/prismAnalytics-file-container-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: FileContainer
---
