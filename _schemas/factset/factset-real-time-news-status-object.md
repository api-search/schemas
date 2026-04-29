---
description: The status member contains the status code of the response.
layout: schema
name: StatusObject
properties_list:
- description: The HTTP status code of the response, mirroring the code from the Status-Line of the HTTP response message (see [RFC2616] section 6.1).
  name: code
  type: number
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-real-time-news-status-object-schema.json
slug: factset-real-time-news-status-object
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StatusObject\",\n  \"type\": \"object\",\n  \"description\": \"The status member contains the status code of the response.\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"number\",\n      \"description\": \"The HTTP status code of the response, mirroring the code from the Status-Line of the HTTP response message (see [RFC2616] section 6.1).\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-real-time-news-status-object-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: StatusObject
---
