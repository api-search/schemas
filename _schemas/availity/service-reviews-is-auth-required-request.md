---
description: IsAuthRequiredRequest schema from Availity API
layout: schema
name: IsAuthRequiredRequest
properties_list:
- description: Authorization details to check
  name: serviceReview
  type: object
provider_name: availity
provider_slug: availity
schema_file: json-schema/service-reviews-is-auth-required-request-schema.json
slug: service-reviews-is-auth-required-request
source_filename: service-reviews-is-auth-required-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-is-auth-required-request-schema.json\",\n  \"title\": \"IsAuthRequiredRequest\",\n  \"description\": \"IsAuthRequiredRequest schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"serviceReview\": {\n      \"type\": \"object\",\n      \"description\": \"Authorization details to check\",\n      \"properties\": {\n        \"payerId\": {\n          \"type\": \"string\",\n          \"example\": \"BCBS001\"\n        },\n        \"procedureCode\": {\n          \"type\": \"string\",\n          \"example\": \"99213\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-is-auth-required-request-schema.json
tags: []
title: IsAuthRequiredRequest
---
