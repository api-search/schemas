---
description: IsAuthRequiredResponse schema from Availity API
layout: schema
name: IsAuthRequiredResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: authRequired
  type: string
- description: ''
  name: payerMessage
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/service-reviews-is-auth-required-response-schema.json
slug: service-reviews-is-auth-required-response
source_filename: service-reviews-is-auth-required-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-is-auth-required-response-schema.json\",\n  \"title\": \"IsAuthRequiredResponse\",\n  \"description\": \"IsAuthRequiredResponse schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"authRequired\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Auth Required\",\n        \"No Auth Required\"\n      ],\n      \"example\": \"Auth Required\"\n    },\n    \"payerMessage\": {\n      \"type\": \"string\",\n      \"example\": \"Prior authorization required for this procedure\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-is-auth-required-response-schema.json
tags: []
title: IsAuthRequiredResponse
---
