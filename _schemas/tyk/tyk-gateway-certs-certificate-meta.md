---
description: ''
layout: schema
name: CertsCertificateMeta
properties_list:
- description: ''
  name: dns_names
  type: array
- description: ''
  name: fingerprint
  type: string
- description: ''
  name: has_private
  type: boolean
- description: ''
  name: id
  type: string
- description: ''
  name: is_ca
  type: boolean
- description: ''
  name: not_after
  type: string
- description: ''
  name: not_before
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-certs-certificate-meta-schema.json
slug: tyk-gateway-certs-certificate-meta
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CertsCertificateMeta\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"dns_names\": {\n      \"type\": \"array\"\n    },\n    \"fingerprint\": {\n      \"type\": \"string\"\n    },\n    \"has_private\": {\n      \"type\": \"boolean\"\n    },\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"is_ca\": {\n      \"type\": \"boolean\"\n    },\n    \"not_after\": {\n      \"type\": \"string\"\n    },\n    \"not_before\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-certs-certificate-meta-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: CertsCertificateMeta
---
