---
description: ''
layout: schema
name: CertificateList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: next
  type: string
- description: ''
  name: offset
  type: string
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-certificate-list-schema.json
slug: kong-gateway-admin-certificate-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\"\n    },\n    \"next\": {\n      \"type\": \"string\"\n    },\n    \"offset\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-certificate-list-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: CertificateList
---
