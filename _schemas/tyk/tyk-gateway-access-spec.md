---
description: ''
layout: schema
name: AccessSpec
properties_list:
- description: ''
  name: methods
  type: array
- description: ''
  name: url
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-access-spec-schema.json
slug: tyk-gateway-access-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessSpec\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"methods\": {\n      \"type\": \"array\"\n    },\n    \"url\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-access-spec-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: AccessSpec
---
