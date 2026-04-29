---
description: ''
layout: schema
name: OpenIDOptions
properties_list:
- description: ''
  name: providers
  type: array
- description: ''
  name: segregate_by_client
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-open-id-options-schema.json
slug: tyk-gateway-open-id-options
source_filename: tyk-gateway-open-id-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenIDOptions\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"providers\": {\n      \"type\": \"array\"\n    },\n    \"segregate_by_client\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-open-id-options-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: OpenIDOptions
---
