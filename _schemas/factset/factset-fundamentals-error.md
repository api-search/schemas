---
description: A single error detail object.
layout: schema
name: Error
properties_list:
- description: A UUID for this particular occurrence of the problem.
  name: id
  type: string
- description: Error status code description.
  name: code
  type: string
- description: The plain text error message.
  name: title
  type: string
- description: The endpoint path for reference.
  name: links
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-fundamentals-error-schema.json
slug: factset-fundamentals-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\",\n  \"type\": \"object\",\n  \"description\": \"A single error detail object.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"A UUID for this particular occurrence of the problem.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error status code description.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The plain text error message.\"\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"The endpoint path for reference.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-fundamentals-error-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: Error
---
