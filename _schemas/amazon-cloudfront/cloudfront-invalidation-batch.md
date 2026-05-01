---
description: InvalidationBatch schema
layout: schema
name: InvalidationBatch
properties_list:
- description: ''
  name: Paths
  type: object
- description: A unique value that ensures the request can't be replayed.
  name: CallerReference
  type: string
provider_name: Amazon CloudFront
provider_slug: amazon-cloudfront
schema_file: json-schema/cloudfront-invalidation-batch-schema.json
slug: cloudfront-invalidation-batch
source_filename: cloudfront-invalidation-batch-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-invalidation-batch-schema.json\",\n  \"title\": \"InvalidationBatch\",\n  \"description\": \"InvalidationBatch schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Paths\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Quantity\": {\n          \"type\": \"integer\",\n          \"description\": \"The number of invalidation paths specified.\"\n        },\n        \"Items\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"A list of paths to invalidate (e.g., /images/image1.jpg, /images/*).\"\n        }\n      }\n    },\n    \"CallerReference\": {\n      \"type\": \"string\",\n      \"description\": \"A unique value that ensures the request can't be replayed.\"\n    }\n  },\n\
  \  \"required\": [\n    \"Paths\",\n    \"CallerReference\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-cloudfront/refs/heads/main/json-schema/cloudfront-invalidation-batch-schema.json
tags:
- CloudFront
- CDN
- Content Delivery
- Edge
title: InvalidationBatch
---
