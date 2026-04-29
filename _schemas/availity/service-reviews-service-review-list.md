---
description: ServiceReviewList schema from Availity API
layout: schema
name: ServiceReviewList
properties_list:
- description: ''
  name: data
  type: array
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
provider_name: availity
provider_slug: availity
schema_file: json-schema/service-reviews-service-review-list-schema.json
slug: service-reviews-service-review-list
source_filename: service-reviews-service-review-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-service-review-list-schema.json\",\n  \"title\": \"ServiceReviewList\",\n  \"description\": \"ServiceReviewList schema from Availity API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ServiceReviewResponse\"\n      }\n    },\n    \"total\": {\n      \"type\": \"integer\",\n      \"example\": 15\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/availity/refs/heads/main/json-schema/service-reviews-service-review-list-schema.json
tags: []
title: ServiceReviewList
---
