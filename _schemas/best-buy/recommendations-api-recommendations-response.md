---
description: Response containing recommended product list.
layout: schema
name: RecommendationsResponse
properties_list:
- description: Metadata about the result set.
  name: metadata
  type: object
- description: Array of recommended product objects.
  name: results
  type: array
provider_name: Best Buy
provider_slug: best-buy
schema_file: json-schema/recommendations-api-recommendations-response-schema.json
slug: recommendations-api-recommendations-response
source_filename: recommendations-api-recommendations-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/recommendations-api-recommendations-response-schema.json\",\n  \"title\": \"RecommendationsResponse\",\n  \"description\": \"Response containing recommended product list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"metadata\": {\n      \"type\": \"object\",\n      \"description\": \"Metadata about the result set.\",\n      \"properties\": {\n        \"resultSet\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"count\": {\n              \"type\": \"integer\",\n              \"description\": \"Number of results returned.\",\n              \"example\": 10\n            }\n          }\n        }\n      }\n    },\n    \"results\": {\n      \"type\": \"array\",\n      \"description\": \"Array of recommended product objects.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RecommendedProduct\"\
  \n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/best-buy/refs/heads/main/json-schema/recommendations-api-recommendations-response-schema.json
tags:
- Retail
- Consumer Electronics
- E-Commerce
- Products
- Stores
title: RecommendationsResponse
---
