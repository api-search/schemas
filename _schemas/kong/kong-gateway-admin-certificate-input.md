---
description: ''
layout: schema
name: CertificateInput
properties_list:
- description: ''
  name: cert
  type: string
- description: ''
  name: key
  type: string
- description: ''
  name: cert_alt
  type: string
- description: ''
  name: key_alt
  type: string
- description: ''
  name: snis
  type: array
- description: ''
  name: tags
  type: array
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-certificate-input-schema.json
slug: kong-gateway-admin-certificate-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertificateInput\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cert\": {\n      \"type\": \"string\"\n    },\n    \"key\": {\n      \"type\": \"string\"\n    },\n    \"cert_alt\": {\n      \"type\": \"string\"\n    },\n    \"key_alt\": {\n      \"type\": \"string\"\n    },\n    \"snis\": {\n      \"type\": \"array\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-certificate-input-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: CertificateInput
---
