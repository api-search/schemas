---
description: ServiceReviewResponse schema from Availity API
layout: schema
name: ServiceReviewResponse
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: certificationNumber
  type: string
- description: ''
  name: effectiveDate
  type: string
- description: ''
  name: expirationDate
  type: string
provider_name: availity
provider_slug: availity
schema_file: json-schema/service-reviews-service-review-response-schema.json
slug: service-reviews-service-review-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-service-review-response-schema.json\",\n  \"title\": \"ServiceReviewResponse\",\n  \"description\": \"ServiceReviewResponse schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"PENDING\",\n        \"APPROVED\",\n        \"DENIED\",\n        \"PARTIALLY_APPROVED\",\n        \"PENDING_ADDITIONAL_INFO\"\n      ],\n      \"example\": \"APPROVED\"\n    },\n    \"certificationNumber\": {\n      \"type\": \"string\",\n      \"example\": \"AUTH-2025-001234\"\n    },\n    \"effectiveDate\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-04-01\"\n    },\n    \"expirationDate\": {\n   \
  \   \"type\": \"string\",\n      \"format\": \"date\",\n      \"example\": \"2025-10-01\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-service-review-response-schema.json
tags: []
title: ServiceReviewResponse
---
