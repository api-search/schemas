---
description: Request Body
layout: schema
name: PostBasicTimezoneListRequest
properties_list:
- description: The data member contains the request's primary data.
  name: data
  type: object
- description: The meta member contains the meta information of the request.
  name: meta
  type: object
provider_name: Factset
provider_slug: factset
schema_file: json-schema/factset-real-time-quotes-post-basic-timezone-list-request-schema.json
slug: factset-real-time-quotes-post-basic-timezone-list-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PostBasicTimezoneListRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request Body\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"The data member contains the request's primary data.\"\n    },\n    \"meta\": {\n      \"type\": \"object\",\n      \"description\": \"The meta member contains the meta information of the request.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/factset/refs/heads/main/json-schema/factset-real-time-quotes-post-basic-timezone-list-request-schema.json
tags:
- Financial
- Financial Data
- Investment Analytics
- Market Data
- Portfolio Analytics
- Research
title: PostBasicTimezoneListRequest
---
