---
description: ''
layout: schema
name: PinnedPublicKey
properties_list:
- description: ''
  name: domain
  type: string
- description: ''
  name: publicKeys
  type: array
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-pinned-public-key-schema.json
slug: tyk-gateway-pinned-public-key
source_filename: tyk-gateway-pinned-public-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PinnedPublicKey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"domain\": {\n      \"type\": \"string\"\n    },\n    \"publicKeys\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-pinned-public-key-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: PinnedPublicKey
---
