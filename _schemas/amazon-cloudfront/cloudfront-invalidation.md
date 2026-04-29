---
description: Invalidation schema
layout: schema
name: Invalidation
properties_list:
- description: The identifier for the invalidation request.
  name: Id
  type: string
- description: The status of the invalidation request.
  name: Status
  type: string
- description: The date and time the invalidation request was created.
  name: CreateTime
  type: string
- description: ''
  name: InvalidationBatch
  type: object
provider_name: Amazon CloudFront
provider_slug: amazon-cloudfront
schema_file: json-schema/cloudfront-invalidation-schema.json
slug: cloudfront-invalidation
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-invalidation-schema.json\",\n  \"title\": \"Invalidation\",\n  \"description\": \"Invalidation schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the invalidation request.\"\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the invalidation request.\"\n    },\n    \"CreateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The date and time the invalidation request was created.\"\n    },\n    \"InvalidationBatch\": {\n      \"$ref\": \"#/components/schemas/InvalidationBatch\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-invalidation-schema.json
tags:
- AWS
- CloudFront
- CDN
- Content Delivery
- Edge
title: Invalidation
---
