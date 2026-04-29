---
description: CreateAllowedOriginRequest schema from Adyen API
layout: schema
name: CreateAllowedOriginRequest
properties_list:
- description: References to resources linked to the allowed origin.
  name: _links
  type: object
- description: Domain of the allowed origin.
  name: domain
  type: string
- description: Unique identifier of the allowed origin.
  name: id
  type: string
provider_name: Adyen
provider_slug: adyen
schema_file: json-schema/management-create-allowed-origin-request-schema.json
slug: management-create-allowed-origin-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-allowed-origin-request-schema.json\",\n  \"title\": \"CreateAllowedOriginRequest\",\n  \"description\": \"CreateAllowedOriginRequest schema from Adyen API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_links\": {\n      \"description\": \"References to resources linked to the allowed origin.\",\n      \"$ref\": \"#/components/schemas/Links\"\n    },\n    \"domain\": {\n      \"description\": \"Domain of the allowed origin.\",\n      \"example\": \"https://adyen.com\",\n      \"type\": \"string\"\n    },\n    \"id\": {\n      \"description\": \"Unique identifier of the allowed origin.\",\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"domain\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adyen/refs/heads/main/json-schema/management-create-allowed-origin-request-schema.json
tags:
- Payments
- Financial Services
- Fintech
title: CreateAllowedOriginRequest
---
