---
description: ''
layout: schema
name: MutualTLS
properties_list:
- description: ''
  name: domainToCertificateMapping
  type: array
- description: ''
  name: enabled
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-mutual-tls-schema.json
slug: tyk-gateway-mutual-tls
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MutualTLS\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domainToCertificateMapping\": {\n      \"type\": \"array\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-mutual-tls-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: MutualTLS
---
