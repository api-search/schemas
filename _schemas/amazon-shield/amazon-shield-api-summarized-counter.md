---
description: SummarizedCounter schema from api
layout: schema
name: SummarizedCounter
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: Max
  type: number
- description: ''
  name: Average
  type: number
- description: ''
  name: Sum
  type: number
- description: ''
  name: N
  type: integer
- description: ''
  name: Unit
  type: string
provider_name: Amazon Shield
provider_slug: amazon-shield
schema_file: json-schema/amazon-shield-api-summarized-counter-schema.json
slug: amazon-shield-api-summarized-counter
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-summarized-counter-schema.json\",\n  \"title\": \"SummarizedCounter\",\n  \"description\": \"SummarizedCounter schema from api\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"Max\": {\n      \"type\": \"number\"\n    },\n    \"Average\": {\n      \"type\": \"number\"\n    },\n    \"Sum\": {\n      \"type\": \"number\"\n    },\n    \"N\": {\n      \"type\": \"integer\"\n    },\n    \"Unit\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-shield/refs/heads/main/json-schema/amazon-shield-api-summarized-counter-schema.json
tags:
- AWS
- DDoS Protection
- Networking
- Security
title: SummarizedCounter
---
