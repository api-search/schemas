---
description: ''
layout: schema
name: PaginationStatus
properties_list:
- description: ''
  name: page_num
  type: integer
- description: ''
  name: page_size
  type: integer
- description: ''
  name: page_total
  type: integer
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-pagination-status-schema.json
slug: tyk-gateway-pagination-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PaginationStatus\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"page_num\": {\n      \"type\": \"integer\"\n    },\n    \"page_size\": {\n      \"type\": \"integer\"\n    },\n    \"page_total\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-pagination-status-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: PaginationStatus
---
