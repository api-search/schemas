---
description: ''
layout: schema
name: ClientCertificates
properties_list:
- description: ''
  name: allowlist
  type: array
- description: ''
  name: enabled
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-client-certificates-schema.json
slug: tyk-gateway-client-certificates
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientCertificates\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"allowlist\": {\n      \"type\": \"array\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-client-certificates-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ClientCertificates
---
